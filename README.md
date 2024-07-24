# Validador de E-mail e Senha (caracteres)

Projeto de estudo criando validações de caracteres para treinar expressões regulares e tratamentos de erros. Neste projeto para validação precisa digitar o padrão do e-mail (nome@mail.com) e na senha precisa conter pelo menos uma letra maiúscula, um carácter especial, um número e totalizar mais de 8 caracteres.

![validator](https://github.com/user-attachments/assets/6278197e-b897-48a8-94e2-c21045d3fdfb)


## 📖 Aprendizados

- Expressões Regulares
- Tratamento de Erros

- Validador do e-mail
```javascript
function validateEmail(email) {
    if (!email.match(/\w{2,}@[a-zA-Z]{2,}\.[a-zA-Z]{2,}/)) {
        const err = new Error('Email inválido.')
        err.input = 'email'
        throw err
    }
}
```
- Validador da Senha
```javascript
function validatePassword(password) {
    if (
        password.length < 8 || 
        !password.match(/[a-z]/) || 
        !password.match(/[A-Z]/) || 
        !password.match(/[0-9]/) ||
        !password.match(/[^a-zA-Z0-9\s]/)
    ) {
        const err = new Error('Senha inválida.')
        err.input = 'password'
        throw err
    }
}
```
## 📡 Tecnologias utilizadas

<img src="https://github.com/user-attachments/assets/5bfb3e0f-06a8-46fe-99bf-3a3a9a3ed9d2" width="25px" />  <img src="https://github.com/user-attachments/assets/b530d801-8a35-4b37-9e07-8decf480cacb" width="25px" />  <img src="https://github.com/user-attachments/assets/11388035-3088-45ae-bdb2-ebc672bdc0be" width="25px" />

## 🔎 Link para acessar

https://phlgoncalves.github.io/email-password--validator_JS/

## 📑 Referências

[OneBitCode cursos](https://onebitcode.com/lp/) 

