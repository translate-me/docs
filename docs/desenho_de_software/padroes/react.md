# Padrões do React JS

## 1. Composition

O aspecto principal no desenvolvimento com React é a composição de componentes.
Componentes diferentes podem ser integrados para criar um componente maior ou mais
complexo e essa junção deve funcionar bem. Assim, a existência dessa
característica tem como objetivo evitar que a adição de alguma funcionalidade
em algum componente cause "side-effects" em outras partes do projeto, ou seja,
toda a arquitetura é baseada em um padrão que prioriza o baixo acoplamento.

No translate-me, por exemplo, as páginas que compõem o fluxo de envio de texto
para tradução são compostas de diversos formulários que se encontram em funções
independentes. Ao juntá-los em uma classe, que gerencia o estado, isto é, os dados
inseridos pelo usuário nos campos, estamos usando da composição para criar um
componente maior.

### 1.1 Props

Mesmo sem herança em si, o React propõe o uso de props, que é uma maneira de compartilhar
informações entre componentes que mantém uma hierarquia entre si e são chamados
de pai e filho. Isso permite independência em relação a esses componentes que se
relacionam, pois a passagem de prop é como uma passagem de parâmetro comum a uma
função e o comportamento interno da mesma não precisa necessariamente ser conhecido
por quem a chama.

### 1.2 High-order component

Outra maneira interessante que o React apresenta para compor componentes é o HOC.
Essa estratégia, bastante similar ao design pattern conhecido como decorator, permite
incrementar um componente com características ou funcionalidades novas, mantendo o componente
original e a função/classe que incrementa-o independentes, caso se queira utilizá-los
separadamente ou incrementar algum outro componente.

## 2. Fluxo de dados unidirecional

Manter um fluxo de dados unidirecional em uma aplicação que gerencia a interface
de um software é de grande ajuda, pois aumenta a coesão e permite a apicção t se comportar
consistentemente, além de facilitar as tarefas de debug e testes.

No caso do translate-me, foi utilizado o Redux para gerenciar o fluxo dos dados entre
os componentes. Essa biblioteca funciona baseada em três componentes básicos:

* A Store, que é um Singleton, ou seja, um objeto que possui apenas uma intância em toda a
aplicação e armazena o estado dos componentes;
* As Actions, que também são objetos, que descrevem alguma mudança a ser realizada
na Store;
* E os Reducers, que são funções responsáveis por receber Actions e gerenciar as
mudanças providas por elas na Store.

Abaixo, um diagrama representando esse funcionamento:

![](https://cdn-images-1.medium.com/max/1600/1*BcmtHcMHN6PT7IniIWniHg.png)
Imagem extraída de [Integrating Semantic Ui Modal with Redux](https://itnext.io/integrating-semantic-ui-modal-with-redux-4df36abb755c)


# Referências

TSONEV, Krasimir. React in Patterns. Disponível em [React in Patterns](https://github.com/krasimir/react-in-patterns).
Acesso em 01/07/2019.

React patterns. Disponível em [React patterns](https://reactpatterns.com/). Acesso em 01/07/2019.
