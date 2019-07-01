# GoFs Estruturais

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
|21/05|0.1|Adicionar decorator, extension e facade| João Robson|
| 23/05 | 0.2 | Inclusão do Adapter, Composite e Bridge | Helena Goulart |
| 23/05 | 0.3 | Inclusão da análise do Facade | Helena Goulart |
| 28/05 | 0.4 | Adiciona Front Controller | Gabriela Guedes|
| 18/05 | 0.5 | Adição dos topicos | Davi Alves e Victor Hugo |
| 18/05 | 0.6 | Adição do twin | Davi Alves e Victor Hugo |
| 17/06 | 0.7 | Unindo os documentos de GoFs estruturais em um só | Helena Goulart |


## 1. Introdução  

GoFs estruturais são conhecidos por se preocuparem na forma na qual os objetos e classes se organizam na composição de uma estrutura maior. Se dividem entre padrões de classe e padrões de herança. Desse modo, os padrões de classe focam na utilização de heranças para composição de interfaces e implementações, enquanto o os de objetos propõe formas de utilização de modo a conseguir novas funcinoalidades.

## 2. GoFs Estruturais

### 2.1 Decorator

#### 2.1.1 Definição

Padrão que permite atribuir comportamentos ou estados a determinados objetos em tempo de execução,
diferentemente de uma herança, por exemplo, que é estática e se aplica à uma classe inteira.

Deve ser usado nas seguintes situações:

* Uma estrutura formada por um objeto principal e vários componentes opcionais com um interface comum a todos;
* Herança é inviável porque definição da classe base está encapsulada/escondida;

#### 2.1.2 Análise

Esse padrão pode ser aplicado no projeto. Uma classe interessante
para sua aplicação, por exemplo, é a do Perfil do usuário. Além de poder atribuir
certificados e línguas a um perfil por meio de decorators, badges e prêmios obtidos
como parte da gamificção do site podem ser associados a uclasse do usuário
por meio de decorator também.

#### 2.1.3 Estrutura mínima

![decorator](https://sourcemaking.com/files/v2/content/patterns/Decorator__1.png)

### 2.2 Extension Objets

#### 2.2.1 Definição

Padrão que permite extender a interface de um objeto no futuro.
Como em algumas abstrações é complicado antecipar completamente
seu funcionamento e determinar se determinada interface será realmente
usada em um cojunto de componentes relacionados, o padrão Extension Objects
provê uma estrutura que antecipa essas etensões opcionais.

Um exemplo disso é um checador gramatical em um editor de texto. Nem todos
componentes (imagens, gráficos, fórmulas, texto em si, etc.)
que podem ser inseridos podem ou necessitam dessa checagem. Nesse contexto,
haveria uma classe abstrata para os componentes, incluindo o checador.
Porém, em vez de adicionar a interface responsável por acessar o texto e
contar as palavras, por exemplo, em todos componentes e deiar sua implementação
vazia para componentes sem texto, o componente do checador se torna independente
e quando necessita ser usado, é chamado pelos componentes.

Deve ser usado nas seguintes situações:

* Necessidade de adicionar funcionalidades novas ou imprevistas a determinadas classes
e não impactar classes que não necessitam dessas novas interfaces.

#### 2.2.2 Análise

Esse padrão não possui uma aplicabilidade clara no projeto, pelo menos por enquanto.

#### 2.2.3 Estrutura

![extension](images/extension.png)

### 2.3 Facade

#### 2.3.1 Definição

O padrão facade serve como um facilitador, interfaceando um conjunto de componentes
que pssuem relacionamentos e funcionalidades complexas. Isso ocorre por meio de uma classe
que encapsula esse subsistema complexo em uma única interface mais simplificada, reduzindo a curva de
aprendizado necessária para compreeder esse pedaço do sistema.

Deve ser usado nas seguintes situações:

* Necessidade de prover uma interface simplificada que abstrai e torna mais fácil
o uso de funcionalidades de outros subsistemas mais complexos;

#### 2.3.2 Análise


Sim, é possível aplicar o Facade no translate.me nos seguintes contextos:

* Serviço de tradução de texto: ao ser submetido, o texto do autor passa por várias etapas que, como cliente, ele não tem acesso. Logo, se o usário tivesse acesso à todo processo de fragmentação do texto, distribuição dos fragmentos para tradutores, revisão e alterações, seria um processo bastante complexo. Com a aplicação do Facade, ele tem uma entrada simples (o texto) e uma única saída (o texto traduzido);

* Serviço de pagamento pela tradução: uma vez que o translate.me recebe o texto realiza o processo de fragmentação, distribuição, tradução e revisão, o pagamento pelo serviço é atribuído a cada tradutor de acordo com a quantidade de palavras interpretadas. Esse cálculo exige que percorra por toda o processo de submissão do texto, porém o usuário autor enxerga apenas um valor a ser pago pelo serviço. O que ele não tem contato é que esse valor é dividido entre vários tradutores, que por sua vez também possuem acesso a somente um dado: o valor pago pelo serviço de tradução de uma quantidade 'x' de palavras.

#### 2.3.3 Estrutura mínima

![facade](https://sourcemaking.com/files/v2/content/patterns/Facade1.png)

### 2.4 Adapter

#### 2.4.1 Definição

Trata-se de um padrão que converte a interface de uma classe para outra interface. Isso normalmente ocorre quando classes precisam trabalhar mas possuem interfaces incompatíveis entre si.

#### 2.4.2 Análise

Pode ser utilizado no translate.me, contudo não soa como uma boa prática: uma vez que o projeto terá seu início e fim acompanhando a disciplina Desenho e Arquitetura de Software, escopo reduzido e conter diagrama de classes e de arquitetura bem definidos, não tende a ser um sistema que vai adotar novas bibliotecas e que passará por adaptações a serem implementadas pelo _Adapter_.

#### 2.4.3 Estrutura mínima

![AdapterPattern](../../../assets/desenho/padroes/Padro_Adapter.jpg)

### 2.5 Bridge

#### 2.5.1 Definição
Este padrão é utilizado para separar uma abstração de sua implementação, possibilitando que ambas atuem independentemente. O termo _"bridge"_ (ponte) é justamente essa ligação estabelecida entre a abstração e sua implementação.

Essa separação permite:
* Acoplamento de funcionalidades;
* Redução da complexidade da arquitetura.

#### 2.5.2 Análise
É cabível de se utilizar o _Bridge_ no projeto translate.me, de modo a separar e agrupar responsabilidades que um usuário tradutor pode ter por exemplo, uma vez que atua tanto como tradutor como revisor, e pode ser também o autor de algum texto.

#### 2.5.3 Estrutura mínima

![BridgePattern](../../../assets/desenho/padroes/bridge.png)

### 2.6 Composite

#### 2.6.1 Definição
Trata-se do agrupamento de objetos de modo a representar hierarquias parte-todo, permitindo tratar objetos individuais e composições uniformemente.

#### 2.6.2 Análise

Pode ser utilizado no translate.me, inclusive é um padrão recomendado que o utilizem pois ele se encaixa com o escopo do projeto, uma vez que contempla a estrutura de editor de texto. Editores são compostos por elementos individuais, tais como palavras e letras, enquanto o texto é um elemento parte-todo, pois contém várias palavras dentro dele.  

#### 2.6.3 Estrutura mínima

![Composite](../../../assets/desenho/padroes/Composite.jpg)

### 2.7 Front Controller

#### 2.7.1 Definição
O front controller é um padrão de projeto que se comporta como um controlador para todas as requisições web da aplicação. Sua funcionalidade se deve para evitar duplicação de código, uma vez que as solicitações de um site são muito similares com passos que devem ser seguidos, como checar a segurança e fornecer uma página de resposta. Ao utilizar o front controller, a duplicação do código será então diminuida, uma vez que todas as requisições serão feitas por esse objeto que será instanciado pela classe do front controller.

Com o front controller, a aplicação possui um único ponto de entrada que trata de todas as requisições. Esse código e responsável por carregar as dependências, fazer o processamento da requisição e levar a resposta para o navegador, chamando a página correta de acordo com a requisição feita.

O front controller é dividido em 2 partes:

* __Manipulador Web:__ Trata as requisições da aplicação. Extrai as informações necessárias da URL e então decide as ações que serão tomadas, o manipulador delega essas ações para serem executadas por um objeto Comando.

* __Comando:__ Executa as ações e escolhe qual página utilizar para a resposta.

#### 2.7.2 Análise
Este padrão não pode ser aplicado no projeto. O front-end do translate.me é feito com React JS, que não segue o padrão MVC, segue um padrão próprio,  onde não há a separação de View e Controller, todas as Views são "controller-views". Como esse padrão exige a separação de uma controller para fazer a manipulação das requisições e as views chamadas, não é possível utilizá-lo com este framework.

#### 2.7.3 Estrutura mínima
![](../../../assets/desenho/padroes/front-controller.png)


### 2.8 Proxy

#### 2.8.1 Definição
Permite o controle de acesso em nível de objeto, agindo como uma passagem através da entidade ou de um objeto de espaço reservado.

**Subject** - Interface implementada pelo RealSubject e representando seus serviços. A interface também deve ser implementada pelo proxy para que o proxy possa ser usado em qualquer local onde o RealSubject possa ser usado.

**Proxy** -
* Mantém uma referência que permite ao proxy acessar o RealSubject.
* Implementa a mesma interface implementada pelo RealSubject para que o proxy possa ser substituído pelo RealSubject.
* Controla o acesso ao RealSubject e pode ser responsável por sua criação e exclusão.
* Outras responsabilidades dependem do tipo de proxy.

**RealSubject** - Objeto real que o proxy representa.

#### 2.8.2 Análise

Pode ser usado nas seguintes situações:
* O objeto sendo representado é externo ao sistema.
* Objetos precisam ser criados sob demanda.
* Controle de acesso para o objeto original é necessário.
* Funcionalidade adicionada é necessária quando um objeto é acessado.

#### 2.8.3 Estrutura Mínima

![](https://circle.visual-paradigm.com/wp-content/uploads/2017/08/GoF-Design-Patterns-Structural-Patterns-Proxy.png)

Exemplo de diagrama de classe UML para o desenho de padrão do modelo "Proxy"

### 2.9 Twin

#### 2.9.1 Definição

Twin é um padrão no qual apenas algumas linguagem que não aceitam multiplas heranças para uma mesma classe utilizam. Como por exemplo java, neste caso, se divide a classe ,que irá herdar as outras classes, em n classes onde n é o npumero de classes que serão herdadas, nesse caso cada uma dessas classes irão herdar de apenas uma classe especifica e depois as classes que foram dividias são ligadas com agregassões entre si.

#### 2.9.2 Análise

Pode ser usado nas seguintes situações:
* Quando tiver que fazer herança de várias classes a uma classe só e que a linguagem não tenha suporte para esse tipo de operação.

#### 2.9.3 Estrutura mínima

![alt](https://upload.wikimedia.org/wikipedia/commons/2/28/Iker_minta.png)

### 2.9 Module

#### 2.9.1 Definição

O padrão de design de software do módulo fornece os recursos e a estrutura sintática definida pelo paradigma de programação modular para linguagens de programação que têm suporte incompleto para o conceito.

#### 2.9.2 Análise

Pode ser usado nas seguintes situações:
* Uma parte do código deve ter acesso global ou público e ser projetada para uso como código global / público. Código privado ou protegido adicional pode ser executado pelo código público principal.
* Um módulo deve ter uma função de finalizador equivalente ou complementar a um método de destruição de objeto. Esse recurso não é suportado por namespaces regulares.
* Os membros de suporte podem exigir código de inicialização / finalização executado pela função inicializador / finalizador do módulo.
* A maioria dos membros são funções que executam operações em elementos externos à classe, fornecidos como argumentos, chamando funções. Essas funções são "utilitários", "ferramentas" ou "bibliotecas".

#### 2.9.3 Estrutura mínima
![](https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/Module-software-design-pattern.png/500px-Module-software-design-pattern.png)

Exemplo de diagrama de classe UML para o desenho de padrão do modelo "Module"


## 3. Referências

### 3.1 Links de sites

* [Klevas - Extension Objects Pattern](https://klevas.mif.vu.lt/~plukas/resources/Extension%20Objects/ExtensionObjectsPattern%20Gamma96.pdf) <br>
* [SourceMaking - Design Patterns](https://sourcemaking.com/design_patterns)
* [DevMedia - Adapter](https://www.devmedia.com.br/padrao-de-projeto-adapter-em-java/26467). <br>
* [UFCG - Composite](http://www.dsc.ufcg.edu.br/~jacques/cursos/map/html/pat/composite.htm).
* [SourceMaking - Bridge Java](https://sourcemaking.com/design_patterns/bridge/java/1)
* [DevMedia - Front Controller](https://www.devmedia.com.br/padroes-de-projetos-introducao-aos-padroes-front-controller-e-command/30644)
* [Klevas - Extension Objects](https://klevas.mif.vu.lt/~plukas/resources/Extension%20Objects/ExtensionObjectsPattern%20Gamma96.pdf)
* [SourceMaking - Design Patterns](https://sourcemaking.com/design_patterns)

### 3.2 Livros e artigos
[1] HUMMEL, Oliver; ATKINSON, Colin. The managed adapter pattern: Facilitating glue code generation for component reuse. In: International Conference on Software Reuse. Springer, Berlin, Heidelberg, 2009. p. 211-224.
