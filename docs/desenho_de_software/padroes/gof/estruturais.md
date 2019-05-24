# GoFs Estruturais

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
|21/05|0.1|Adicionar decorator, extension e facade| João Robson|


### Decorator


#### Definição 

Padrão que permite atribuir comportamentos ou estados a determinados objetos em tempo de execução,
diferentemente de uma herança, por exemplo, que é estática e se aplica à uma classe inteira.

##### Quando deve ser usado

* Uma estrutura formada por um objeto principal e vários componentes opcionais com um interface comum a todos;
* Herança é inviável porque definição da classe base está encapsulada/escondida;

#### Estrutura

![decorator](https://sourcemaking.com/files/v2/content/patterns/Decorator__1.png)

#### Análise

Esse padrão pode ser aplicado no projeto. Uma classe interessante
para sua aplicação, por exemplo, é a do Perfil do usuário. Além de poder atribuir
certificados e línguas a um perfil por meio de decorators, badges e prêmios obtidos
como parte da gamificção do site podem ser associados a uclasse do usuário
por meio de decorator também.

### Extension Objets


#### Definição 

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

#### Estrutura

![extension](images/extension.png)

#### Análise

Esse padrão não possui uma aplicabilidade clara no projeto, pelo menos por enquanto.

### Facade


#### Definição 

O padrão facade serve como um facilitador, interfaceando um conjunto de componentes
que pssuem relacionamentos e funcionalidades complexas. Isso ocorre por meio de uma classe
que encapsula esse subsistema complexo em uma única interface mais simplificada, reduzindo a curva de
aprendizado necessária para compreeder esse pedaço do sistema.

##### Quando deve ser usado

* Necessidade de prover uma interface simplificada que abstrai e torna mais fácil
o uso de funcionalidades de outros subsistemas mais complexos;

#### Estrutura

![facade](https://sourcemaking.com/files/v2/content/patterns/Facade1.png)

#### Análise


# Referências

* [https://klevas.mif.vu.lt/~plukas/resources/Extension%20Objects/ExtensionObjectsPattern%20Gamma96.pdf](https://klevas.mif.vu.lt/~plukas/resources/Extension%20Objects/ExtensionObjectsPattern%20Gamma96.pdf)

* [https://sourcemaking.com/design_patterns](https://sourcemaking.com/design_patterns)

