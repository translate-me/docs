# GoFs Estruturais

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
|21/05|0.1|Adicionar decorator, extension e facade| João Robson|
| 23/05 | 0.2 | Inclusão do Adapter, Composite e Bridge | Helena Goulart |
| 23/05 | 0.3 | Inclusão da análise do Facade | Helena Goulart |

## 1. Introdução  

GoFs estruturais são conhecidos por se preocuparem na forma na qual os objetos e classes se organizam na composição de uma estrutura maior. Se dividem entre padrões de classe e padrões de herança. Desse modo, os padrões de classe focam na utilização de heranças para composição de interfaces e implementações, enquanto o os de objetos propõe formas de utilização de modo a conseguir novas funcinoalidades.

## 2. GoFs Estruturais

## 2.1 Decorator

#### 2.1.1 Definição

Padrão que permite atribuir comportamentos ou estados a determinados objetos em tempo de execução,
diferentemente de uma herança, por exemplo, que é estática e se aplica à uma classe inteira.

##### Quando deve ser usado

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

## 2.2 Extension Objets

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

##### Quando deve ser usado
* Necessidade de adicionar funcionalidades novas ou imprevistas a determinadas classes
e não impactar classes que não necessitam dessas novas interfaces.

#### 2.2.2 Análise

Esse padrão não possui uma aplicabilidade clara no projeto, pelo menos por enquanto.

#### 2.2.3 Estrutura

![extension](images/extension.png)

## 2.3 Facade

#### 2.3.1 Definição

O padrão facade serve como um facilitador, interfaceando um conjunto de componentes
que pssuem relacionamentos e funcionalidades complexas. Isso ocorre por meio de uma classe
que encapsula esse subsistema complexo em uma única interface mais simplificada, reduzindo a curva de
aprendizado necessária para compreeder esse pedaço do sistema.

##### Quando deve ser usado

* Necessidade de prover uma interface simplificada que abstrai e torna mais fácil
o uso de funcionalidades de outros subsistemas mais complexos;

#### 2.3.2 Análise
Pode ser utilizado no translate.me, mas não é o mais recomendado, uma vez que é comumente utilizado em projetos complexos e com o escopo maior, o que não é o caso do projeto em questão. 

#### 2.3.3 Estrutura mínima

![facade](https://sourcemaking.com/files/v2/content/patterns/Facade1.png)

## 2.4 Adapter

### 2.4.1 Definição

Trata-se de um padrão que converte a interface de uma classe para outra interface. Isso normalmente ocorre quando classes precisam trabalhar mas possuem interfaces incompatíveis entre si.

### 2.4.2 Análise

Pode ser utilizado no translate.me, contudo não soa como uma boa prática: uma vez que o projeto terá seu início e fim acompanhando a disciplina Desenho e Arquitetura de Software, escopo reduzido e conter diagrama de classes e de arquitetura bem definidos, não tende a ser um sistema que vai adotar novas bibliotecas e que passará por adaptações a serem implementadas pelo _Adapter_.

### 2.4.3 Estrutura mínima

![AdapterPattern](../../../assets/desenho/padroes/Padro_Adapter.jpg)

## 2.5 Bridge

### 2.5.1 Definição
Este padrão é utilizado para separar uma abstração de sua implementação, possibilitando que ambas atuem independentemente. O termo _"bridge"_ (ponte) é justamente essa ligação estabelecida entre a abstração e sua implementação.

Essa separação permite:
* Acoplamento de funcionalidades;
* Redução da complexidade da arquitetura.

### 2.5.2 Análise
É cabível de se utilizar o _Bridge_ no projeto translate.me, de modo a separar e agrupar responsabilidades que um usuário tradutor pode ter por exemplo, uma vez que atua tanto como tradutor como revisor, e pode ser também o autor de algum texto.

### 2.5.3 Estrutura mínima

![BridgePattern](../../../assets/desenho/padroes/bridge.png)

## 2.6 Composite

### 2.6.1 Definição
Trata-se do agrupamento de objetos de modo a representar hierarquias parte-todo, permitindo tratar objetos individuais e composições uniformemente.

### 2.6.2 Análise

Pode ser utilizado no translate.me, inclusive é um padrão recomendado que o utilizem pois ele se encaixa com o escopo do projeto, uma vez que contempla a estrutura de editor de texto. Editores são compostos por elementos individuais, tais como palavras e letras, enquanto o texto é um elemento parte-todo, pois contém várias palavras dentro dele.  

### 2.6.4 Estrutura mínima

![Composite](../../../assets/desenho/padroes/Composite.jpg)

## 3. Referências

### Links de sites

* [Klevas - Extension Objects Pattern](https://klevas.mif.vu.lt/~plukas/resources/Extension%20Objects/ExtensionObjectsPattern%20Gamma96.pdf) <br>
* [SourceMaking - Design Patterns](https://sourcemaking.com/design_patterns)
* [DevMedia - Adapter](https://www.devmedia.com.br/padrao-de-projeto-adapter-em-java/26467). <br>
* [UFCG - Composite](http://www.dsc.ufcg.edu.br/~jacques/cursos/map/html/pat/composite.htm).
* [SourceMaking - Bridge Java](https://sourcemaking.com/design_patterns/bridge/java/1)

### Livros e artigos
[1] HUMMEL, Oliver; ATKINSON, Colin. The managed adapter pattern: Facilitating glue code generation for component reuse. In: International Conference on Software Reuse. Springer, Berlin, Heidelberg, 2009. p. 211-224.
