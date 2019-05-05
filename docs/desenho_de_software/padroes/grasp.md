# GRASP (General Responsibility Assignment Software Patterns)

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|:---:|:---:|:---:|:---:|
|05/05/2019|0.1| Adicionando o template, introdução e tópico 'controlador' | Rômulo Souza |

## 1. Introdução

Os GRASP são padrões criados para manter os padrões de qualidade e organização do código de um projeto, pode ser considerado como a essência do paradigma de Orientação a Objetos. A partir destes, é possível analisar quais são as responsibilidades de uma classe, um objeto, um componente, dentre outros, além de idendificar como objetos podem interagir entre si. Os GRASP são divididos em nove padrões, que serão analisados a seguir, para o estudo da viabilidade de suas aplicações no projeto

## 2. Viabilidade de Aplicação

### 2.1. Controlador

#### 2.1.1. Definição

Atribui a responsabilidade de manipular eventos do sistema para uma classe externa ao usuário; funciona como uma fachada para a interação com o sistema. 

#### 2.1.2. Análise

A arquitetura do projeto é orientada a microsserviços. Haja vista o desacoplamento das funcionalidades, foi definido que não haverá um serviço centralizador e, portanto, o uso do controlador torna-se inviável em uma visão macroscópica do projeto.

Cada microsserviço seguirá a arquitetura do _django rest framework_, que realiza uma boa separação das funcionalidades. Dentre essas funcionalidades, a camada controladora é realizada internamente ao _framework_. Desse modo, não será aplicado o padrão no projeto.

### 2.2. Criador

### 2.3. Indireção

### 2.4. Especialista na Informação

### 2.5. Alta Coesão

### 2.6. Baixo Acoplamento

### 2.7. Polimorfismo

### 2.8. Invenção Pura

### 2.9. Variações Protegidas
