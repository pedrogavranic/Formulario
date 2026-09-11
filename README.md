# 🔐 Sistema de Cadastro de Usuários

Projeto Full Stack desenvolvido com Flask, SQLite, HTML, CSS e JavaScript para gerenciamento de usuários. O sistema permite criar contas, armazenar usuários em banco de dados, visualizar registros cadastrados e realizar recuperação e redefinição de senha por meio de token de segurança.

## 🚀 Funcionalidades

✅ Cadastro de usuários

✅ Validação de campos obrigatórios

✅ Verificação de confirmação de senha

✅ Controle de e-mails duplicados

✅ Armazenamento de dados em banco SQLite

✅ Listagem de usuários cadastrados

✅ Recuperação de senha

✅ Geração de token de redefinição

✅ Redefinição de senha com validação de token

✅ Interface responsiva e intuitiva

---

## 🛠️ Tecnologias Utilizadas

### Back-end
- Python
- Flask
- SQLite3

### Front-end
- HTML5
- CSS3
- JavaScript

### Bibliotecas
- Flask
- SQLite
- UUID
- Datetime

---

## 📂 Estrutura do Projeto

```bash
📦 projeto
├── app.py
├── database.db
├── index.html
├── recuperar_senha.html
├── redefinir_senha.html
├── usuarios.html
└── src/
    ├── styles/
    └── scripts/
```

---

## 📋 Funcionalidades do Sistema

### Cadastro de Usuários

O sistema permite cadastrar:

- Nome
- Sobrenome
- Data de nascimento
- E-mail
- Senha
- Gênero

Todos os dados são armazenados no banco SQLite.

---

### Visualização de Usuários

A página de usuários exibe:

- ID
- Nome
- Sobrenome
- Data de nascimento
- E-mail
- Gênero
- Data de criação

---

### Recuperação de Senha

O usuário pode informar seu e-mail para solicitar a recuperação de senha.

O sistema:

1. Verifica se o e-mail existe.
2. Gera um token único.
3. Define prazo de expiração.
4. Redireciona para a página de redefinição.

---

### Redefinição de Senha

Com o token válido o usuário pode:

- Criar uma nova senha
- Confirmar a nova senha
- Atualizar o registro no banco de dados

Após a alteração o token é removido automaticamente.

---

## ⚙️ Como Executar o Projeto

### 1. Clonar o Repositório

```bash
git clone https://github.com/seuusuario/seu-repositorio.git
```

### 2. Entrar na Pasta

```bash
cd seu-repositorio
```

### 3. Instalar Dependências

```bash
pip install flask
```

### 4. Executar o Projeto

```bash
python app.py
```

### 5. Acessar no Navegador

```bash
http://localhost:5000
```

---

## 🗄️ Banco de Dados

O projeto utiliza SQLite para armazenamento local dos dados.

Tabela principal:

```sql
users
```

Campos:

```sql
id
name
last_name
birthdate
email
password
gender
recovery_token
recovery_expires_at
created_at
```

---

## 📸 Telas do Sistema

- Cadastro de Usuários
- Recuperação de Senha
- Redefinição de Senha
- Listagem de Usuários

---

## 🎯 Objetivo do Projeto

Este projeto foi desenvolvido com fins acadêmicos e de aprendizado para praticar:

- Desenvolvimento Full Stack
- Criação de APIs REST
- Integração Front-end e Back-end
- Manipulação de Banco de Dados
- Autenticação e Segurança
- Flask Framework
- JavaScript Assíncrono (Fetch API)

---

## 👨‍💻 Autor

João Pedro Santiago Martins Rodrigues

Estudante de Sistemas de Informação – Universidade Anhembi Morumbi

GitHub: https://github.com/pedrogavranic
