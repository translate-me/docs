# Documentação de viabilidade do uso de GoFs criacionais

### Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
|11/05/2019|0.1|Adição dos topicos| Davi Alves e Luiz Guilherme|

## Introdução

Um padrão de projeto é uma solução geral e reutilizável para um problema comum de software. Eles são modelos que podem ser reutilizados e personalizados para resolver um problema específico de design em muitas situações diferentes.

### 1. Prototype
![](https://circle.visual-paradigm.com/wp-content/uploads/2017/08/GoF-Design-Patterns-Creational-Patterns-Prototype.png)

Exemplo de diagrama de classe UML para o desenho de padrão do modelo "Prototype"

#### Explicação
Criar objetos com base em um modelo de um objeto existente por meio de clonagem, ou seja, ele é usado quando o tipo de objeto a ser criado é determinado por uma instância prototípica, que é clonada para produzir novos objetos.

#### Quando deve ser usado
* Quando a composição, criação e representação de objetos devem ser dissociadas de um sistema.
* As classes a serem criadas são especificadas no tempo de execução.
* Um número limitado de combinações de estados existe em um objeto.
* Objetos ou estruturas de objeto são requeridos que são idênticos ou se assemelham a outros objetos ou estruturas de objetos existentes.
* A criação inicial de cada objeto é uma operação custosa.

### 2. Object Pool

![](https://www.oodesign.com/images/stories/objectpool%20implementation%20-%20uml%20class%20schema.gif)

Exemplo de diagrama de classe UML para o desenho de padrão do modelo "Object Pool"

#### Explicação
O agrupamento de objetos pode oferecer um aumento de desempenho significativo em situações em que o custo de inicializar uma instância de classe é alto, a taxa de instanciação de uma classe é alta e o número de instâncias em uso a qualquer momento é baixo. O "object pool" é obtido em tempo previsível, o que torna esse padrão útil para sistemas em tempo real.

#### Quando deve ser usado
* A criação inicial de cada objeto é uma operação custosa.
* A frequência de criação de outros objetos também é alta.
* O número de objetos em uso é pequeno.


### 3. Builder

![](https://circle.visual-paradigm.com/wp-content/uploads/2017/08/GoF-Design-Patterns-Creational-Patterns-Builder.png)

Exemplo de diagrama de classe UML para o desenho de padrão do modelo "builder"

#### Explicação
Permite a criação dinâmica de objetos com base em algoritmos facilmente intercambiáveis.Esse padrão permite que um objeto cliente construa um objeto complexo especificando apenas seu tipo e conteúdo, sendo protegido dos detalhes relacionados à representação de objetos.

#### Quando deve ser usado

* Algoritmos de criação de objetos devem ser desacoplados do sistema.
* Várias representações de algoritmos de criação são necessárias.
* A adição de nova funcionalidade de criação sem alterar o código principal é necessária.
* O controle de tempo de execução sobre o processo de criação é necessário.

### 4. Abstract Factory

![AbstractMethodAplication](http://www.dsc.ufcg.edu.br/~jacques/cursos/map/html/pat/abstractfactory2.gif)

Exemplo de diagrama de classe UML para o desenho de padrão do modelo _"Abstract Factory"._

#### Explicação
Trata-se da criação de famílias de objetos relacionados ou dependentes por meio de apenas uma interface gráfica e sem que a classe concreta seja especificada. Logo, a estrutura mínima de um _Abstract Factory_ exige as estruturas da imagem acima.

#### Quando deve ser usado
- É utilizado quando um sistema deve ser independente de como seus produtos relacionados são criados e representados;
- É aplicável em casos onde uma família de produtos foi projetada para uso conjunto e é necessária implementar uma restrição;

É interessante ressaltar que ambos os pontos acima são aplicáveis no seguinte exemplo: um _software_ precisa ser utilizado em dois sistemas operacionais distintos, Windows e Ubuntu. Para isso, ele possui uma parte

### Singleton

![](https://cdn-images-1.medium.com/max/1200/1*WXXQZp1glrQxLqrQ_TDN7Q.png)

#### Explicação

Conforme incita o próprio nome, os padrões de projeto do tipo _Singleton_ possibilitam criar objetos únicos para os quais há apenas uma instância, permitindo acesso a ela através de um ponto global. Dessa forma, uma classe gerencia sua própria instância e nenhuma outra classe poderá gerenciá-la.

#### Quando deve ser usado

- O _Singleton_ é recomendado quando é necessário conhecer bem o ponto de acesso à classe de um objeto;
- Quando é necessário controlar como e quando a instância será acessada.

## Conclusão

A implementação destes GOFs dentro do projeto se aplicam em diversos aspectos, que vão desde uma implementação relacionada as linguagens escolhidas, quanto a complexidade de criação de instâncias de objetos. Para o 'Prototype', pode ser aplicado devido a utilização do Javascript. No Javascript, a principal classe é a 'Object' e todas as demais classes à herdam. Portanto, todas as classes do Javascript possuem disponíveis um atributo chamado 'prototype' e portanto, toda classe criada, pode implementar este padrão de projeto, permitindo a clonagem de uma classe e adicionar um determinado atributo ou função, através do seu protótipo.

Já para a implementação do Object Pool, não é tão simples, pois requere um grau de complexidade ainda não alcançado na aplicação e de acordo com o escopo determinado, também não deve alcançar. Tal padrão de projeto, pode ser implementado, porém sem uma real necessidade e portanto, não sera implementado até o momento.

Diferentemente, o Builder é um padrão de projeto essencial e pode ser aplicado em diversos aspectos do software, como existem diferentes categorias de texto disponíveis, recomenda-se a implementação criando um construtor de textos e uma especificação em cada uma das categorias de texto. Além disso, o construtor pode ser implementado para efeitos comparativos sobre performance, analisando em um possível benchmarking, a velocidade da criação de um objeto desacoplado com e sem um construtor aplicado.

## Referencias

[1] https://circle.visual-paradigm.com/category/uml-diagrams/gof-design/ <br>
[2] https://www.oodesign.com/object-pool-pattern.html <br>
[3] https://medium.com/@sawomirkowalski/design-patterns-object-pool-e8269fd45e10 <br>
[4] https://circle.visual-paradigm.com/builder/ <br>
[5] https://www.oodesign.com/builder-pattern.html <br>
[6] http://www.dsc.ufcg.edu.br/~jacques/cursos/map/html/pat/abstractfactory.htm <br>
[7] https://www.devmedia.com.br/padrao-de-projeto-singleton-em-java/26392 <br>
