📝 Sistema de Inscrição MINDTECH

📌 Descrição do Projeto

O Sistema de Inscrição MINDTECH é uma aplicação web que permite que usuários se cadastrem enviando seus dados (nome, e-mail e senha).

O projeto possui:

Front-end moderno e responsivo, inspirado na tela de inscrição da MINDTECH.

Backend em Node.js com Express, que recebe os dados do usuário e salva em um banco SQLite.

Mensagens de sucesso ou erro exibidas diretamente no formulário.

🎨 Tecnologias Utilizadas
Front-end	Backend	Banco de Dados
HTML5	Node.js	SQLite
CSS3	Express	
JavaScript	Body-Parser	
Google Fonts (Roboto)	CORS	
📂 Estrutura do Projeto
newsletter-proje/
│
├─ backend/
│   └─ server.js          # Servidor Node.js + API
│
├─ frontend/
│   ├─ index.html         # Tela de inscrição
│   └─ logo.png           # Logo MINDTECH
│
└─ README.md              # Este arquivo

⚙️ Requisitos

Node.js (recomendo LTS 18.x)

Navegador moderno (Chrome, Edge, Firefox)

Editor de código (VS Code recomendado)

🚀 Como Rodar o Projeto
1️⃣ Configurar o Backend

Abra o terminal no VS Code dentro da pasta backend.

Inicialize o projeto Node.js (se ainda não tiver feito):

npm init -y


Instale as dependências:

npm install express body-parser sqlite3 cors


Inicie o servidor:

node server.js


Você verá:

Servidor rodando em http://localhost:3000
Conectado ao SQLite.

2️⃣ Configurar o Frontend

Abra a pasta frontend.

Abra o arquivo index.html em um navegador.

Preencha os campos do formulário e clique em Inscrever-se.

O formulário envia os dados para o backend (http://localhost:3000/inscricao).

Mensagem de sucesso ou erro será exibida logo abaixo do formulário.

3️⃣ Testar a API (Opcional)

Você pode testar a API com Postman ou Insomnia:

Método: POST

URL: http://localhost:3000/inscricao

Body (JSON):

{
  "nome": "Otávio Silva",
  "email": "otavio@example.com",
  "senha": "123456"
}


Resposta esperada:

{
  "message": "Inscrição realizada com sucesso!",
  "id": 1
}

📌 Funcionalidades

Cadastro de usuário com nome, email e senha

Mensagem de sucesso ou erro após envio do formulário

Armazenamento seguro no banco SQLite

Layout moderno, com logo MINDTECH e gradiente de fundo

💡 Dicas

Para reiniciar o servidor: CTRL + C e depois node server.js.

O banco inscricoes.db será criado automaticamente na pasta backend.

É recomendável criar um .gitignore para não subir pastas pesadas:

node_modules/
*.db
*.log


Para atualizar o GitHub após alterações:

git add .
git commit -m "Descrição da alteração"
git push

🎉 Resultado Esperado

Tela centralizada com logo MINDTECH à esquerda

Campos de nome, e-mail e senha estilizados

Botão “Inscrever-se” com efeito hover

Mensagem de sucesso/erro dinâmica
