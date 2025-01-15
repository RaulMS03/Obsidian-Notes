#React 

O conceito de ``key``  no react é muito importante, principalmente quando estamos utilizando componentes que possuem algum grau de "parentesco", onde (exemplo) usamos um ``.map`` em **array** de qualquer coisa. O **React** não consegue entender a diferença em cada item daquele array, pois, sempre que ele renderizar o mesmo componente ele precisa verificar se aquele item já existe, seja no estado ou em qualquer lugar. 

Existem 3 momentos em que o componente renderiza novamente, sendo eles:

- 1. Quando o estado do componente altera.
- 2. Quando a propriedade altera.
- 3. Quando um componente pai renderiza novamente.

É bom lembrar que o uso da ``key`` é o mais adequado em varias questoes. Exemplo: não podemos usar o **índice do array**, pois em aplicações grandes, quando algum componente que recebe muitas informações distintas renderiza de novo, o **React** não consegue saber se aquela informação já exista antes ou não, pois o que pode mudar é apenas a posição no **array**, mas não seu **id** e com isso, acaba tirando toda performance da aplicação e fazendo com que as informações possam chegar incorretas.
## Próximo: [[]]