# GRASP (General Responsibility Assignment Software Patterns)

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|:---:|:---:|:---:|:---:|
|05/05/2019|0.1| Adicionando o template, introdução e tópico **controlador** | Rômulo Souza |
|05/05/2019|0.2| Adicionando tópicos **criador**, **baixo acoplamento**, **polimorfismo**, **fabricação pura** e **referências** | Rômulo Souza |

## 1. Introdução

Os GRASP são padrões criados para manter os padrões de qualidade e organização do código de um projeto, pode ser considerado como a essência do paradigma de Orientação a Objetos. A partir destes, é possível analisar quais são as responsibilidades de uma classe, um objeto, um componente, dentre outros, além de idendificar como objetos podem interagir entre si. Os GRASP são divididos em nove padrões, que serão analisados a seguir, para o estudo da viabilidade de suas aplicações no projeto

## 2. Viabilidade de Aplicação

### 2.1. Controlador

#### 2.1.1. Definição

Atribui a responsabilidade de manipular eventos do sistema para uma classe externa ao usuário; funciona como uma interface para a interação com o sistema. 

#### 2.1.2. Análise

A arquitetura do projeto é orientada a microsserviços. Haja vista o desacoplamento das funcionalidades, foi definido que não haverá um serviço centralizador e, portanto, o uso do controlador torna-se inviável em uma visão macroscópica do projeto.

Cada microsserviço seguirá a arquitetura do _django rest framework_, que realiza uma boa separação das funcionalidades. Dentre essas funcionalidades, a camada controladora é realizada internamente ao _framework_. Desse modo, não será aplicado o padrão no projeto.

### 2.2. Criador

#### 2.2.1 Definição

Define o responsável pela criação de objetos através do relacionamento entre as classes. Para isso, deve-se cumprir pelo menos um dos seguintes requisitos:

* B agrega objetos da classe A.
* B contém objetos da classe A.
* B registra instâncias da classe A.
* B usa muitos objetos da classe A.
* B possui os dados usados para inicializar A.

#### 2.2.2 Análise

Ao realizar a análise dos requisitos para a utilização do creator, vê-se que é viável sua implementação para o projeto. Uma possível aplicação será a criação de fragmentos de texto. No projeto, haverá uma classe TEXTO que será composta por uma classe FRAGMENTO. A classe TEXTO será responsável por instanciar os objetos do tipo FRAGMENTO, haja vista que possui os dados necessários para a inicialização destes. Utilizando o padrão criador, somente a classe TEXTO será responsável por instanciar FRAGMENTO, mantendo assim certo encapsulamento do código.

### 2.3. Indireção

### 2.4. Especialista na Informação

### 2.5. Alta Coesão

#### 2.5.1. Definição

Coesão é um conceito que indica quão relacionadas estão as responsibilidades de determinado elemento do projeto, isto é, o nível de pertencimento das partes de algum elemento àquele escopo específico.

#### 2.5.2. Análise

A aplicação da alta coesão no projeto se dará em diversos contextos. Um dele é a distribuição de responsabilidades específicas entre os microserviços do back-end. Ao se utilizar um serviço independente para gerenciar a autenticação, por exemplo, mantém-se o foco da classe que lida com a autenticação apenas na criação de novos usuários, administradores ou comuns, e na geração e validação dos tokens dos mesmos, atribuindo a função de modificar o perfil desses usuários à outro microserviço, o de perfis.

### 2.6. Baixo Acoplamento

#### 2.6.1. Definição

O baixo acomplamento visa manter a independência de elementos no código, assegurando que não estejam fortemente conectados. Por conseguinte, obtêm-se maior manutenibilidade do sistema e reutilização de código.

#### 2.6.2. Análise

Será aplicado o conceito de baixo acoplamento em algumas partes do projeto. Uma aplicação visível no projto é no padrão composite, que poderá ser utilizado com a parte de fragmentação de texto e com as mensagens do chat. O composite permitirá que a classe composta esteja diretamente associada somente a uma interface, ao invés de se associar a todas as classes concretas que a implementam.

### 2.7. Polimorfismo

#### 2.7.1. Definição

Polimorfismo é um conceito que permite a declaração de uma  interface para ser utilizada por diferentes tipos de dados. No polimorfismo, não há a preocupação com os detalhes de implementação de quem a está usando. Em suma, o polimorfismo nos permite exercer diferentes comportamentos em estruturas de mesmo nome.

#### 2.7.2. Análise

O polimorfismo pode ser aplicado na linguagem escolhida para o backend (python). Torna-se viável sua utilização em alguns dos padrões desejados pela equipe, como o composite, que poderá ser usado na criação de fragmentos ou na criação de mensagens para o chat.

### 2.8. Fabricação Pura

#### 2.8.1 Definição

O padrão Fabricação Pura é representado por uma classe que não apresenta um conceito bem definido no domínio do problema. Pode ser exemplificado como uma classe que realiza um papel similar à prestação de serviços. O uso desse padrão auxilia no baixo acoplamento e na alta coesão do sistema, além de facilitar a manutenção e a reutilização do código.

#### 2.8.2 Análise


### 2.9. Variações Protegidas

## 3. Referências

* [GRASP Design Principles](https://www.cs.colorado.edu/~kena/classes/5448/f12/presentation-materials/rao.pdf)
* [GRASP – General Responsibility Assignment Software Patterns Explained](http://www.kamilgrzybek.com/design/grasp-explained/)
* [Ramom Silva - Padrão Creator](http://ramonsilva.net/boas-praticas/grasp/creator-padroes-grasp/)
* [Object Oriented Programming](https://medium.com/from-the-scratch/oop-everything-you-need-to-know-about-object-oriented-programming-aee3c18e281b)
* [Herança e Polimorfismo Python](https://www.caelum.com.br/apostila-python-orientacao-objetos/heranca-e-classes-abstratas/#exerccios---classes-abstratas)
