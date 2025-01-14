#React 

O ```useState()``` é um **hook** do **React** que permite gerenciamento de estados, alterar ou/e "salvar" a forma como algo se comporta. 
### Exemplo:

```
const [comments, setComments] = useState([1, 2]);
```

Nesse exemplo é possível ver o uso do ```useState()```, o caso apresentado era que eu necessitava de alguma forma que sempre que eu escrevesse meu texto na pagina e apertasse enter, ou clicasse no botão de publicar, que um comentário fosse adicionado, foi ai que eu utilizei esse hook. 

Ele possui essa estrutura, primeiro o que ele vai receber é a variável ```comments``` como o valor que vou usar para ver os comentários na minha tela e em seguida a variável ```setComents```que recebe uma função para eu alterar o valor da minha variável de comentário.

```
function handleCreateNewComment() {
	event.preventDefault();
	
	setComments([...comments, comments.length + 1])
}
```

Criei essa função para adicionar um comentario, esse ```event.preventDefault()``` serve para preservar a pagina quando o usuário clique em algum elemento que possa dar um refresh ou te levar para outra pagina, mantendo o conceito de **SPA**, e em seguida utilizo o ```setComments``` recebendo os ```comments``` com um **spread operator** ```...``` que copia o que ja esta armazenado anteriormente no array e em seguida, verifico o tamanho da variável ```comments``` adiciono 1, agora podemos adicionar comentários livremente fazendo com que o valor dos ```comments``` seja alterado sempre que eu dar **submit** no formulário. 

## Próximo: [[]]
