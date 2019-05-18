# Documentação de viabilidade do uso de GoFs estruturais

### Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
|18/05/2019|0.1|Adição dos topicos| Davi Alves e Victor Hugo|
|18/05/2019|0.2|Adição do twin| Davi Alves e Victor Hugo|

## Introdução

Um padrão de projeto é uma solução geral e reutilizável para um problema comum de software. Eles são modelos que podem ser reutilizados e personalizados para resolver um problema específico de design em muitas situações diferentes.

### 1. Proxy
![](https://circle.visual-paradigm.com/wp-content/uploads/2017/08/GoF-Design-Patterns-Structural-Patterns-Proxy.png)

Exemplo de diagrama de classe UML para o desenho de padrão do modelo "Proxy"

#### Explicação
Permite o controle de acesso em nível de objeto, agindo como uma passagem através da entidade ou de um objeto de espaço reservado.

**Subject** - Interface implementada pelo RealSubject e representando seus serviços. A interface também deve ser implementada pelo proxy para que o proxy possa ser usado em qualquer local onde o RealSubject possa ser usado.

**Proxy** - 
* Mantém uma referência que permite ao proxy acessar o RealSubject.
* Implementa a mesma interface implementada pelo RealSubject para que o proxy possa ser substituído pelo RealSubject.
* Controla o acesso ao RealSubject e pode ser responsável por sua criação e exclusão.
* Outras responsabilidades dependem do tipo de proxy.

**RealSubject** - Objeto real que o proxy representa.

#### Quando deve ser usado
* O objeto sendo representado é externo ao sistema.
* Objetos precisam ser criados sob demanda.
* Controle de acesso para o objeto original é necessário.
* Funcionalidade adicionada é necessária quando um objeto é acessado.

### 2. Twin

![alt](https://upload.wikimedia.org/wikipedia/commons/2/28/Iker_minta.png)
   
#### Explicação
Twin é um padrão no qual apenas algumas linguagem que não aceitam multiplas heranças para uma mesma classe utilizam. Como por exemplo java, neste caso, se divide a classe ,que irá herdar as outras classes, em n classes onde n é o npumero de classes que serão herdadas, nesse caso cada uma dessas classes irão herdar de apenas uma classe especifica e depois as classes que foram dividias são ligadas com agregassões entre si.

#### Quando deve ser usado
* Quando tiver que fazer herança de várias classes a uma classe só e que a linguagem não tenha suporte para esse tipo de operação.

### 3. Module

![](https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/Module-software-design-pattern.png/500px-Module-software-design-pattern.png)

Exemplo de diagrama de classe UML para o desenho de padrão do modelo "Module"

#### Explicação

O padrão de design de software do módulo fornece os recursos e a estrutura sintática definida pelo paradigma de programação modular para linguagens de programação que têm suporte incompleto para o conceito. 

#### Quando deve ser usado
* Uma parte do código deve ter acesso global ou público e ser projetada para uso como código global / público. Código privado ou protegido adicional pode ser executado pelo código público principal.
* Um módulo deve ter uma função de finalizador equivalente ou complementar a um método de destruição de objeto. Esse recurso não é suportado por namespaces regulares.
* Os membros de suporte podem exigir código de inicialização / finalização executado pela função inicializador / finalizador do módulo.
* A maioria dos membros são funções que executam operações em elementos externos à classe, fornecidos como argumentos, chamando funções. Essas funções são "utilitários", "ferramentas" ou "bibliotecas".

