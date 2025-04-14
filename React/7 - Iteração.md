#React 

Vou usar de exemplo o que aprendi estudando. Basicamente um iteração é pegar um **array** e percorrer por cada item dele, no **React**, é possível ( por exemplo ) receber um **array** com vários **objetos/arrays de objetos** e por meio de uma chave ( **id** ) fazer uma iteração para um componente só receber varias informações sem precisar repetir. A forma mais simples de fazer isso é utilizando o método **```.map()```** que vai percorrer por todo **array** e retornar o que existe dentro dele

### Exemplo:

```
const posts = [
  {
    id: 1,
    author: {
      avatarUrl: "https://github.com/RaulMS03.png",
      name: "Raul Mascarenhas",
      role: "Web Developer",
  },
    content: [
      { type: "paragraph", content: "Fala galeraa 👋" },
      {
        type: "paragraph",
        content:
          "Acabei de subir mais um projeto no meu portifa. É um projeto que fiz no NLW Return, evento da Rocketseat. O nome do projeto é DoctorCare 🚀",
      },
      { type: "link", content: "👉 jane.design/doctorcare" },
    ],
    publishedAt: new Date("2025-01-14 09:30:00"),
  },
  {
    id: 2,
    author: {
      avatarUrl: "https://github.com/ericcarvlh.png",
      name: "Eric Carvalho",
      role: "Backend Engineer SR",
    },
    content: [
      { type: "paragraph", content: "" },
      { type: "paragraph", content: "" },
      { type: "link", content: "👉 jane.design/doctorcare" },
    ],
    publishedAt: new Date("2025-01-12 10:27:00"),
  },
];
```

Isso é um **array** de posts que estou utilizando em meu projeto, ele esta localizado no arquivo **```App.jsx```** e como é possível ver,  o array possui um **id** e isso permite ajudar na iteração. 

Em seguida, posso começar a iteração: 

```
<main>
	{posts.map((posts) => {
		return (
			<Post
				author={posts.author}
				content={posts.content}
				publishedAt={posts.publishedAt}
			/>
		);
	})}
</main>
```

Nesse caso, eu estou chamando meu **array** de posts com as respectivas informações, só que mesmo fazendo isso nesse caso eu ainda não vou visualizar nada em minha tela, pois nesse caso em especifico eu preciso agora passar essas informações para outro arquivo, que é o **```Post.jsx```**. Isso vai funcionar por meio das **Propriedades**

```
export function Post({ author }) {
	  return (
		<div>
			<Avatar src={author.avatarUrl} />
			<div>
				<strong>{author.name}</strong>
				<span>{author.role}</span>
			</div>
		</div>
	);
}
```

 Como é possível ver, as **props** foram desestruturadas, assim recebendo suas informações diretamente, mas se eu quisesse, poderia passar como **Post(props)** e chamar como **{props.author.name}**. agora minhas informações estão sendo exibidas e se o array possuir mais de um item, ira ser exibido também
 ![[Pasted image 20250114111153.png]]

## Próximo: [[8 - Hooks - useState()]]
