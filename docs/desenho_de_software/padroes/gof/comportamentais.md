# GoFs Comportamentais

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
| 27/05/2019 | 0.1 | Adicionando Mediator | Renan Schadt e Rômulo Souza |
| 27/05/2019 | 0.2 | Adicionando Observer | Renan Schadt |
| 27/05/2019 | 0.3 | Adição dos tópicos 2.3 e 2.4 | Davi Alves e Luiz Guilherme |
| 28/05/2019 | 0.4 | Adição do Command | Victor Hugo |
| 27/05/2019 | 0.3 | Adição dos topicos 2.3 e 2.4 | Davi Alves e Luiz Guilherme |
| 30/05/2019 | 0.4 | Inclusão do Iterator | Helena Goulart |


## 1. Introdução

## 2. GoFs Comportamentais

### 2.1 Mediator

#### 2.1.1 Definição
Mediator é um padrão de design comportamental que impede a comunicação direta entre objetos, tem a função de evitar uma rede caótica de dependências, para fazê-lo o Mediator força os objetos a se comunicar indiretamente, usando de um objeto "mediador".

Ao se chamar um objeto Mediator ele redireciona as requisições para os componentes apropriados, como resultado os componentes dependem apenas do Mediator ao invés de estarem ligados a diversas outras classes.

Este padrão permite encapsular uma complexa rede de relações entre componentes dentro de um objeto, tornando o sistema mais legível e fácil de modificar.

O padrão Mediator contém os seguintes elementos:

1. Diversos componentes, que são classes que contém lógica de negócio. Cada componente tem uma referência ao mediador, declarado com o tipo da interface do mediador.

2. Uma interface Mediator que declara métodos de comunicação entre componentes.

3. Uma classe Concrete Mediator que encapsula a relação entre vários componentes, guardando as suas referências e gerenciando seus ciclos de vida.

#### 2.1.2 Análise
Após avaliação dos Requisitos chegamos a conclusão que o padrão Mediator se aplica a uma área de nossa aplicação, onde uma classe mediadora organizaria os tradutores e revisores responsáveis por algum fragmento de texto específico.

O Django possui formas já definidas de realizar essa tarefa, que correspondem a lógica do Mediator, usaremos dessas funções.

#### 2.1.3 Estrutura Mínima
![](../../../assets/desenho/padroes/mediator.png)

### 2.2 Observer

#### 2.2.1 Definição
Observer é um padrão de design comportamental, que define um mecanismo que notifica múltiplos objetos sobre qualquer evento que ocorra com o objeto que estão observando.

O objeto observado é normalmente definido como Publisher, pois divulga suas mudanças de estado. Os objetos que desejam acompanhar essas mudanças são chamados de Subscribers.

O padrão Observer sugere adicionar um mecanismo de inscrição a classe Publisher, para que outros objetos possam se inscrever ou desinscrever dos sinais disparados por aquele Publisher. É crucial que os Subscribers implementem a mesma interface do Publisher.

Assim que ocorre um novo evento, o Publisher itera sobre a lista de inscritos e chama o método de notificação declarado na interface do Subscriber, em cada objeto Subscriber presente na lista.

O padrão Observer contém os seguintes elementos:

1. Um Publisher, que é o elemento observado, contendo um sistema de inscrição, que permite que Subscribers o acompanhem ou deixem de acompanhá-lo.

2. Uma interface Subscriber, que declara a interface de notificação.

3. Classes de Concrete Subscribers, que realizam ações em resposta a eventos disparados pelo Publisher.

#### 2.2.2 Análise
Após a análise da documentação do Django chegamos a conclusão que este framework já aplica o Observer nativamente, não sendo necessária a construção da estrutura mínima descrita abaixo, visto que ela já está pronta.

#### 2.2.3 Estrutura Mínima
![](../../../assets/desenho/padroes/observer.png)

### 2.3 Visitor Pattern

#### 2.3.1 Definição

No _Visitor Pattern_, usamos uma classe de visitante que altera o algoritmo de execução de uma classe de elemento. Por este caminho, o algoritmo de execução do elemento pode variar como e quando o visitante varia. Esse padrão está na categoria de padrão de comportamento. Conforme o padrão, o objeto de elemento precisa aceitar o objeto de visitante para que o objeto de visitante manipule a operação no objeto de elemento.

O objetivo principal do _Visitor Pattern_ é abstrair a funcionalidade que pode ser aplicada a uma hierarquia agregada de elementos de objetos. A abordagem incentiva a criação de classes de elementos leves - porque a funcionalidade de processamento é removida de sua lista de responsabilidades. Novas funcionalidades podem ser facilmente adicionadas à hierarquia de herança original, criando uma nova subclasse Visitante.

#### 2.3.2 Análise

Foi verificado que a aplicação do padrão Visitor Pattern não reflete a complexidade para o nosso projeto pois não possuímos uma estrutura de objetos como muitas interfaces diferentes, não realizamos muitas operações distintas e não relacionadas e não ocorre a adição frequente de novas operações da classe.

#### 2.3.3 Estrutura mínima

![](https://www.oodesign.com/images/behavioral/visitor-pattern.png)

### 2.4 Null Object

#### 2.4.1 Definição
No padrão Objeto Nulo, um objeto nulo substitui a verificação da instância do objeto NULL. Em vez de colocar se verificar um valor nulo, o objeto nulo reflete uma relação de não fazer nada. Esse objeto Nulo também pode ser usado para fornecer um comportamento padrão caso os dados não estejam disponíveis.

No padrão Objeto Nulo, criamos uma classe abstrata especificando várias operações a serem executadas, classes concretas estendendo essa classe e uma classe de objeto nulo fornecendo nada implementando dessa classe e serão usadas de maneira aparentemente inexistente onde precisamos verificar o valor nulo.

#### 2.4.2 Análise

Foi verificado que o uso do padrão Null Object no projeto não é necessário pois não existem diversos fluxos alternativos em tratamentos de expressões condicionais. O que se assemelharia a utilização desse padrão seria melhor implementado utilizando o proxy, pois, referem-se a tratamentos que não envolvem nulidade.


#### 2.4.3 Estrutura mínima
![](https://www.oodesign.com/images/design_patterns/behavioral/null_object_implementation_-_uml_class_diagram.gif)


### 2.5 Command   
#### 2.5.1 Definição  

O padrão _command_ adiciona um nível de abstração para as ações executados pelas classes e adiciona um objeto que é responsável por invocar essas ações. Normalmente esse tipo de padrão funciona de seguinte forma:

1. O cliente cria um objeto comando a ser executado e que possui uma lista de comandos.
2. Esse objeto comando implementa sua própria interface específica para suas ações.

Dessa forma temos um desacoplamento entre o invocador do método e seu receptor. E também, temos um melhor encapsulamento da aplicação.

#### 2.5.2 Análise
É possível usar esse padrão de projeto dentro do nosso escopo atual desde que não force seu uso dentro das próprias classes do django, ou seja, use ela apenas em um arquivo separado chamado utils e utilize apenas sua chamada dentro da view que você deseja utilizar daquele método.

#### 2.5.3 Estrutura mínima
![](../../../assets/desenho/padroes/architecture_of_command_pattern.jpg)


### 2.6 Iterator

#### 2.6.1 Definição
Trata-se de um meio de acessar sequencialmente os elementos de um objeto agregado sem expor sua representação subjacente. Desse modo, não é de importância se está sendo tratado com um _array_ ou com um _hash_.

#### 2.6.2 Análise
É um padrão possível de ser utilizado no translate.me, como por exemplo para acessar uma lista de línguas estrangeiras que o tradutor domina, ou até mesmo uma lista de trechos já traduzidos pelo tradutor.

#### 2.6.3 Estrutura mínima

![Iterator](../../../assets/desenho/padroes/iterator_pattern.jpg)

### 2.7 Interpreter

#### 2.7.1 Definição
Trata-se de um padrão no qual realiza a interpretação de um código, ou seja, é responsável por processar e interpretar parâmetros.

#### 2.7.2 Análise
O interpreter pode ser utilizado no translate.me. Apesar de que seu uso é bastante comum em compiladores, também possui outras aplicações, tais como  montagem de calculadoras para serviços e preços. Contudo, não é o mais recomendado, uma vez que seria necessário forçar muito o seu uso.


#### 2.7.3 Estrutura mínima

![](../../../assets/desenho/padroes/interpreter.png)


### 2.8 Chain of Responsability

#### 2.8.1 Definição

O Padrão Chain of Responsability é focado na delegação de funções para diferentes instâncias de uma mesma classe abstrata. Isto é, esse padrão configura a declaração de uma classe abstrata que é montada com métodos genéricos, bem como a funcionalidade de delegar a o funcionamento para uma outra instância de um elemento que herda dessa classe abstrata, seguindo uma ordem hierárquica.

A um primeiro momento, o conceito pode parecer complexo, mas é fundamental compreender que a implementação do padrão busca facilitar a execução de atividades sequências em um sistema, transformando comportamentos específicos em objetos que desempenham uma função específica. Assim, após crar uma classe abstrata com métodos base, incluindo um método que instancia um outro objeto do mesmo tipo dessa classe abstrata, é necessário implementar classes que herdam dessa primeira, visando tratar as requisições de forma linear, permitindo ainda que a requisição não prossiga na cadeia de objetos dependendo do contexto dos objetos que gerenciam.

Assim o padrão Chain of Responsability contém os seguintes elementos:

1. Uma interface *Handler* responsável por implementar a lógica básica das outras classes e a função de identificar a próxima instância, hierarquicamente;

2. Classes que herdam da interface, tidas como *Receivers* e que implementam, suas lógicas próprias;

3. Uma lógica externa, tida como *Sender* que faz a requisição para a cadeia implementada.

#### 2.8.2 Análise

O Padrão é uma boa saída para modularizar fluxos que seriam muito longos e acoplados no caso de uma cadeia de **if ... else if ... else** entretanto sua aplicação no projeto não se demonstrou viável a um primeiro momento, dado que os possívels fluxos para um dado estado não se encaixam em uma cadeia sequencial, tampouco se faz necesário pelas estruturas comparativas que existem no contexto da aplicação do projeto em Django.  
Uma vantagem evidente em relação ao uso de uma cadeia de if é a possibilidade de duas saídas possíveis para uma etapa, conforme a instância de um objeto permite, como no caso do cancelamento da continuidade da hirarquia.   
Um outro ponto positivo é a possibilidade da alteração da ordem de execução dos objetos sem mudanças extremas no fluxo, mantendo a conectividade entre os módulos (ou objetos).


#### 2.8.3  Estrutura Mínima

##### 2.8.3.1 Diagrama de Classes

![chain_diagram](../../../assets/desenho/padroes/gof_chain_of_responsability_class.jpg)

##### 2.8.3.2 Diagrama de Sequência

![chain_sequence](../../../assets/desenho/padroes/gof_chain_of_responsability_sequence.jpg)

#### 2.8.4 Exemplo Conceitual


Um exemplo interessante que ilustra essa cadeia é o processo de autenticação por etapas em uma aplicação, de forma que um usuário primeiro tenha que possuir um nome cadastrado na aplicação, posteriormente possuir uma senha válida e, em alguns casos, ocorre uma etapa de veriicação com questões específicas, sendo que em cada uma dessas etapas é possível uma falha do usuário bem como a completudo e prosseguimento do fluxo. No exemplo, cada etapa atuaria como *Receiver* de uma mesma classe abstrata.


## 3. Referências
* [Guru Design Patterns - Mediator](https://refactoring.guru/design-patterns/mediator)
* [Guru Design Patterns - Observer](https://refactoring.guru/design-patterns/observer)
* [DevMedia - Iterator](https://www.devmedia.com.br/padrao-de-projeto-iterator-em-java/26733)
* [Interpreter - Blog do Matheus](https://blog.matheuscastiglioni.com.br/interpreter-padroes-de-projeto-em-java/)
* [Guru Design Patterns - Chain of Responsability](https://refactoring.guru/design-patterns/chain-of-responsibility)
* [Chain of Responsability Implementation](https://www.tutorialspoint.com/design_pattern/chain_of_responsibility_pattern.htm)
* [OO Design - Visitor Pattern](https://www.oodesign.com/visitor-pattern.html). <br>
* [OO Design - Null Object](https://www.oodesign.com/null-object-pattern.html).
* [Python Design Patterns - Command](https://www.tutorialspoint.com/python_design_patterns/python_design_patterns_command.htm)
* [Command in Python](https://sourcemaking.com/design_patterns/command/python/1)
* [Strategy and Command Design Patterns — Wizards and Sandwiches — Applications in Python](https://medium.com/@rrfd/strategy-and-command-design-patterns-wizards-and-sandwiches-applications-in-python-d1ee1c86e00f)
* [DESIGN PATTERNS - COMMAND PATTERN](https://www.bogotobogo.com/DesignPatterns/command.php)
