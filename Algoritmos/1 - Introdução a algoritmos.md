 #algoritmos
### Logaritmos

Basicamente os logaritmos são o oposto de exponenciais, exemplo: 

A expressão $\mathrm{log}_{10}$ 100 basicamente diz: "Quantos 10s conseguimos multiplicar para chegar a 100?". A resposta é 2:10 * 10. Então $\mathrm{log}_{10}$ 100 = 2.

- 10² = 100 <---> $\mathrm{log}_{10}$ 100 = 2
- 10³ = 1000 <---> $\mathrm{log}_{10}$ 1000 = 3
- 2³ = 8 <---> $\mathrm{log}_{2}$ 8 = 3
- 2⁴ = 16 <---> $\mathrm{log}_{2}$ 16 = 4
- 2⁵ = 32 <--->  $\mathrm{log}_{2}$ 32 = 5 

Ou seja, para uma lista de 8 elementos , log 8 == 3, porque 2³ == 8. Então precisaria de no máximo 3 tentativas. Para uma lista de 1.024 elementos, log 1024 elementos, log 1024 == 10, porque 2¹⁰ == 1.024. Logo, para uma lista de 1.024 números, precisaria verificar no máximo 10 deles.
### Pesquisa Simples e Binaria

A pesquisa Simples não é nada eficaz comparada a binaria em grande escala, por exemplo:

Supondo que temos uma Lista de números ordenados de 0 a 240.000, no pior dos casos na pesquisa simples o numero desejado seja 240.000, em uma pesquisa simples teríamos:

- 1, 2, 3, 4, 5, 6, 7, ... 240k, ou seja 240k de palpites só  pra achar o ultimo numero 

Na pesquisa binaria economia de tempo de execução é gigantesca, porque cortamos a quantidade de itens na lista pela metade:

- 240k, 120k, 60k, 30k, 15k, 7.5k, 3750, 1875, 938, 469, 235, 118, 59, 30, 15, 8, 4, 2, 1 -> 18 palpites

- Pesquisa binaria só funciona em listas ordenadas

### Exercícios

1.1 Suponha que você tenha uma lista com 128 nomes e esteja fazendo uma pesquisa binaria. Qual seria o numero máximo de etapas que você levaria para encontrar o nome desejado?

- 64, 32, 16, 8, 4, 2, 1 ->  7 palpites para 128 nomes

1.2  Suponha que você duplique o tamanho da lista. Qual seria o numero máximo de etapas agora?

- 128 * 2 = 256
- 128, 64, 32, 16, 8, 4, 2, 1 -> 8 palpites para 256 nomes