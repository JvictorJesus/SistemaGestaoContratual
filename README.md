# 📚 Dicionário de Dados — Sistema de Gestão Contratual e Processos

> Portfólio acadêmico de modelagem de banco de dados com dicionário de dados interativo em HTML.

![MySQL](https://img.shields.io/badge/MySQL-8.4%20LTS-4479A1?style=flat&logo=mysql&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![InnoDB](https://img.shields.io/badge/Engine-InnoDB-orange?style=flat)
![LGPD](https://img.shields.io/badge/LGPD-Compliant-green?style=flat)

---

## 📌 Sobre o Projeto

Este repositório apresenta o **Dicionário de Dados Governado** do **Sistema de Gestão Contratual e Processos**, desenvolvido para a **Juliana Campos de Jesus Sociedade Individual de Advogados**.

O projeto contempla a modelagem conceitual (DER), o modelo lógico normalizado até a **3ª Forma Normal** e o script físico em **MySQL 8.4 LTS** (InnoDB + utf8mb4), além de uma página interativa em HTML/CSS/JS com busca, dark mode e visualização do DER.

O sistema gerencia clientes, contratos de honorários, processos judiciais, partes, audiências, prazos processuais, metadados de documentos, pagamentos, usuários, advogados, consentimento LGPD e trilha de auditoria.

---

## ✨ Funcionalidades da Página

- 🔍 Busca em tempo real por tabelas e colunas
- 🌙 Modo claro / escuro
- 🗺️ Visualização interativa do DER (zoom + pan)
- 📋 Tabelas completas com descrição, regras de negócio, constraints, classificação de privacidade, linhagem e controle de acesso (RBAC)
- 📱 Layout responsivo (desktop e mobile)
- 📥 Download da Especificação de Requisitos (PDF)

---

## 🗂️ Estrutura do Repositório

```text
├── index.html                  # Página principal do Dicionário de Dados
├── style.css                   # Estilos (tema claro/escuro)
├── script.js                   # Interatividade (busca, modal DER, theme)
├── assets/
│   └── der.png                 # Diagrama Entidade-Relacionamento
├── docs/
│   └── Especificacao_Requisitos_Regras_Negocio_BD.pdf
└── README.md
```

---

## 🛠️ Tecnologias Utilizadas

| Camada              | Tecnologia                          |
|---------------------|-------------------------------------|
| Banco de Dados      | MySQL 8.4 LTS (InnoDB, utf8mb4)     |
| Modelagem           | DER + Modelo Lógico 3FN             |
| Frontend            | HTML5, CSS3, JavaScript (Vanilla)   |
| Visualização DER    | Panzoom                             |
| Segurança / LGPD    | Criptografia (AES), Hash (Argon2id), exclusão lógica |

---

## 🚀 Como visualizar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```

2. Abra o arquivo `index.html` no navegador  
   **ou** utilize um servidor local:
   ```bash
   python -m http.server 8000
   ```

3. Acesse: [http://localhost:8000](http://localhost:8000)

---

## 👥 Equipe

| Função              | Nome                              | RA        |
|---------------------|-----------------------------------|-----------|
| Data Owner          | João Victor de Jesus Silva        | 48134872  |
| Data Steward        | Wendel Alves Viana                | 46049169  |
| Orientador          | Prof. Dr. Diego Marques de Carvalho | —       |

**Instituição:** Universidade Cidade de São Paulo — Análise e Desenvolvimento de Sistemas  
**Disciplina:** Modelagem de Banco de Dados  
**Ano:** 2026

---

## 📄 Documentação

- [Especificação de Requisitos e Regras de Negócio (PDF)](docs/Especificacao_Requisitos_Regras_Negocio_BD.pdf)
- Diagrama Entidade-Relacionamento disponível na própria página (botão **Visualizar DER**)

---

## 📝 Observações

- O banco de dados utiliza **exclusão lógica** (`ativo`) em vez de exclusão física.
- Dados sensíveis (CPF/CNPJ) são armazenados cifrados + hash para unicidade.
- Senhas utilizam **Argon2id**.
- O conteúdo binário de documentos **não** é armazenado no banco (apenas metadados).

---

**Desenvolvido para fins acadêmicos**  
Universidade Cidade de São Paulo — 2026
