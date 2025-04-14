#React
# Rendering Patterns

## Single Page Application 

Quando o usuário faz algum acesso a uma rota, o back-end busca no banco de dados ou alguma API, porem, ele não tem todas as instruções de construir o front-end da pagina, ele apenas retorna os dados dos usuários no modelo JSON que vai para uma ou mais aplicações separadas que são responsáveis por converter o JSON para HTML/CSS/JS.

![[Pasted image 20241106205728.png]]
## Server Side Rendering

Toda vez que o usuário requisita uma pagina da aplicação, essa página é recebida pelo servidor, o servidor contem todo código, tanto back-end quanto front-end da aplicação, no caso, ele recebe uma informação do browser, nisso ele faz as buscas e retorna todo o HTML/CSS/JS ( Do servidor para o Navegador ).

![[Pasted image 20241106210129.png]]
### - Próximo: [[2 - Bundlers & Compilers]]
