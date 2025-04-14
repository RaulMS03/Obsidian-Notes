#TypeScript

**TypeScript** é uma linguagem de programação que é um **superconjunto do JavaScript**. Isso significa que tudo o que você pode fazer em **JavaScript** também pode ser feito em **TypeScript**, mas com algumas melhorias.

A principal diferença é que o **TypeScript** adiciona **tipagem estática** ao **JavaScript**. Isso ajuda a evitar erros, pois você pode definir o tipo das variáveis, funções e objetos, tornando o código mais seguro e previsível.

### Para que serve?

- **Evitar erros**: Se você tentar usar uma variável de um tipo errado, o **TypeScript** avisa antes mesmo de rodar o código.
- **Melhor organização**: Com a tipagem, o código fica mais claro e fácil de entender.
- **Facilitar manutenção**: Projetos grandes se beneficiam, pois é mais difícil cometer erros ao modificar o código.
- **Compatibilidade com JavaScript**: Como **TypeScript** vira **JavaScript** no final, ele pode ser usado em qualquer projeto JavaScript normal.

### Exemplo rápido:

Em **JavaScript**:
```
function soma(a, b) {
  return a + b;
}

console.log(soma(5, "10")); // Retorna "510" (erro inesperado)
```

Em **TypeScript**:
```
function soma(a: number, b: number): number {
  return a + b;
}

console.log(soma(5, "10")); // Erro! "10" deveria ser um número
```

Nesse caso, o **TypeScript** já avisa que algo está errado antes mesmo de rodar o código!

Ou seja, **TypeScript** ajuda a escrever códigos **mais seguros, organizados e fáceis de manter**. 

## Próximo: [[]]