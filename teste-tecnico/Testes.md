
Teste de atomicidade, como fazer. 

melhorias:

- Campos recebendo string vazia
- cache redis
- testes com pytest

Já feitos:

- Modelo de Dados (ERD) 
- Criação do banco de dados
- validação do banco, se existe ou não
- DockerFile
- Docker-Compose.yml
- requirements.txt
- fix recursividade, banco está normal
- PGAdmin online para ver o banco
- nova estrutura dos models
- arquivo para criar as tabelas de forma simples via Docker
- JWT token
- Enpoints protegidos
- autenticação via JWT
- POST agora valida string vazia
- Estoques tem localização
- Cria equipamentos
- Cria Localizações
- Cria Categorias
- Registra Movimento

Rotas:

- GET /estoques
- GET /estoques/{id}
- GET /localizacoes
- GET /categorias
- GET /tipos-equipamentos
- GET /equipamentos
- GET /movimentacoes
- POST /estoques
- POST /auth/register
- POST /auth/login
- POST /localizacoes
- POST /categorias
- POST /tipos-equipamentos
- POST /equipamentos
- POST /movimentacoes
- PATCH /estoques/{id}/desativar
- PATCH /equipamentos/{id}/desativar
- PUT /equipamentos/{id}