# GoFs Criacionais

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---| |
| 21/05/2019 | 0.1 | Inclusão dos GoFs Abstract Factory e Singleton| Helena Goulart |

## Abstract Factory  

### Definição

Trata-se da criação de famílias de objetos relacionados ou dependentes por meio de apenas uma interface gráfica e sem que a classe concreta seja especificada. Logo, a estrutura mínima de um _Abstract Factory_ exige todas as estruturas da imagem acima: <br>
- <b> ProdutoAbstratoA e ProdutoAbstratoB: </b> classe abstrata para seus respectivos tipos de produtos;
- <b> ProdutoA1, ProdutoA2, ProdutoB1 e ProdutoB2: </b> definem produtos criados pela fábrica concreta, que implementa a interface declarada em ProdutoAbstratoA (para ProdutoA1 e ProdutoA2) e em ProdutoAbstratoB (para ProdutoB1 e ProdutoB2);
- <b> FabricaAbstrata: </b> classe ou interface abstrata para operações de criação de produtos;
- <b> FabricaConcreta1 e FabricaConcreta2: </b> Implementam as operações para criar objetos para produtos concretos.

### Análise

- É utilizado quando um sistema deve ser independente de como seus produtos relacionados são criados e representados;
- É aplicável em casos onde uma família de produtos foi projetada para uso conjunto e é necessária implementar uma restrição;

É interessante ressaltar que ambos os pontos acima são aplicáveis no seguinte exemplo: um mesmo usuário pode ser tradutor e usário a ter seu texto traduzido. Logo, ambos possuem características em comum, mas também características específicas que precisam ser desenvolvidas separadamente.

### Estrutura mínima

![Abstract](/assets/desenho/padroes/abstract_factory.png)


## Singleton


### Definição

Conforme incita o próprio nome, os padrões de projeto do tipo _Singleton_ possibilitam criar objetos únicos para os quais há apenas uma instância, permitindo acesso a ela através de um ponto global. Dessa forma, uma classe gerencia sua própria instância e nenhuma outra classe poderá gerenciá-la.

### Análise

O _Singleton_ é recomendado quando é necessário controlar como e quando a instância será acessada, como por exemplo dados de pagamento que incluem informações pessoais de cartão de cŕedito.


### Estrutura mínima

![Singleton](/assets/desenho/padroes/Singleton.png)

## Referências

### Links de sites

[1] Para conferir as referências do Abstract Factory [clique aqui](http://www.dsc.ufcg.edu.br/~jacques/cursos/map/html/pat/abstractfactory.htm).  <br>
[2] Para conferir as referências do Singleton [clique aqui](https://www.devmedia.com.br/padrao-de-projeto-singleton-em-java/26392). <br>

### Livros e artigos

[1] NOBLE, James. GOF patterns for GUI Design. preprint of Macquarie University, Sydney Australia, 1997. <br>
[2] ELLIS, Brian; STYLOS, Jeffrey; MYERS, Brad. The factory pattern in API design: A usability evaluation. In: Proceedings of the 29th international conference on Software Engineering. IEEE Computer Society, 2007. p. 302-312
