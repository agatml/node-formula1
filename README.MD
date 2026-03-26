🏎️ Fastify Minimal API — Formula 1 Example

Uma API simples construída com Fastify para disponibilizar informações de equipes e pilotos da Fórmula 1.

Projeto criado com fins de estudo utilizando uma estrutura minimalista de API REST.

🚀 Tecnologias
Node.js
Fastify
TypeScript
📦 Instalação

Clone o repositório:

git clone https://github.com/agatml/node-formula1.git

Entre na pasta do projeto:

cd node-formula1

Instale as dependências:

npm install
▶️ Executando o projeto

Inicie o servidor:

npm run start

O servidor será iniciado em:

http://localhost:3333
📌 Endpoints
✅ Listar equipes
GET /teams

Resposta:

{
  "teams": [
    { "id": 1, "name": "McLaren", "base": "Working, UK" }
  ]
}
✅ Listar pilotos
GET /drivers

Resposta:

{
  "drivers": [
    { "id": 1, "name": "Max Verstappen", "team": "Red Bull Racing" }
  ]
}
✅ Buscar piloto por ID
GET /drivers/:id

Exemplo:

GET /drivers/1

Resposta (200):

{
  "driver": {
    "id": 1,
    "name": "Max Verstappen",
    "team": "Red Bull Racing"
  }
}

Resposta (404):

{
  "message": "Driver Not Found"
}

📂 Estrutura do Projeto
src/
 └── server.ts
🎯 Objetivo

Este projeto demonstra:

criação de API REST minimalista
rotas com Fastify
parâmetros de rota
respostas HTTP com status code
organização simples para aprendizado
🧠 Autor

Desenvolvido para estudos de Node.js + Fastify.