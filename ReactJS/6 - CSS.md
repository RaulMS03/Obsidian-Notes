#React
# CSS Modules

- **CSS Modules** é nativo do #vite 

Dentro do React existem inúmeras formas de estilizar as aplicações, mas por padrão podemos utilizar **CSS**. Porém, é importante lembrar que as importações não são feitas pelo **HTML** e sim pelos arquivos **JavaScript**.

Basicamente, o **CSS Modules** é muito útil para aplicações de grande escala, no caso, você cria um arquivo na estrutura **Componente.module.css** para que esse estilo fique atrelado ao componente especifico e importa ele o nomeando: **import styles from './Componente.module.css'**, e como visto anteriormente, o **styles** fica como uma **prop** e é possível utiliza-lo em seu código onde deseja estilizar.

# CSS Global

É um arquivo **CSS** que armazena estilos globais que vão servir para aplicação toda dependendo de onde ele for importado, muito útil para padronização e também é utilização de variáveis no **CSS**.
## Próximo: [[7 - Iteração]]
