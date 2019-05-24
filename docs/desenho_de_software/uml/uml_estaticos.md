# UMLs Estáticos

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
| 14/04/2019 | 0.1 | Adicionando diagrama de pacotes | Gabriela Guedes|
| 03/05/2019 | 0.2 | Estruturando padrão do documento | Victor Hugo|
| 05/05/2019 | 0.3 | Adicionando introdução e referências nos artefatos| Victor Hugo|
| 20/05/2019 | 0.4 | Adicionando nova versão do diagrama de classe | Letícia Meneses, Rômulo Vinicius|

## Introdução

**UML** é um acrônimo para a expressão *Unified Modeling Language*. Pela definição de seu nome, vemos que a UML é uma linguagem que define uma série de artefatos que nos ajuda na tarefa de modelar e documentar os sistemas orientados a objetos que desenvolvemos. Para o *Translate.me* foi feito uma série de modelos *UMLs* para orientação no decorrer do projeto.

## UMLs Estáticos
Diagramas umls estáticos são diagramas que tratam da parte estrutural do projeto tanto do ponto de vista do sistema quanto o das classes. Existem para visualizar e especificar aspectos estáticos da aplicação, ou seja, sua estrutua estática ou estável. Geralmente aspectos estáticos de um sistema está atrelado as definições de classes, interfaces, colaborações e componentes.

### Diagrama de Classes
Diagrama de classe mostra as diferentes classes que existem na aplicação e como ela se relacionam. Além disso, este diagrama é considerado estático pois, mostram todos os métodos e atributos das classes bem como os relacionamentos estáticos entre elas, ou seja, quais classes conhecem quais classes ou quais classes são parte das outras classes. Esse tipo de diagrama não mostram as mensagens entre elas. Nesse diagrama os retângulos são a representação das classes e dentro dos retângulos menores existem atributos e métodos que são diferenciados com a utilização de "()" para diferenciar os tipos.
### CD01 
#### Versão 1.0
![diagrama_classes](../../assets/desenho/uml/diagrama_classes.png)

#### Versão 2.0
![diagrama_classes](../../assets/desenho/uml/diagrama_classes_v2.jpg)

### Diagrama de Pacotes
Diagrama de pacotes é básicamente o empacotamento das classes da aplicação. Apesar dos critérios de empacotamento ser subjetivo tendem a ser empacotados classes que tem relacionamento é ou modificação conjunta na aplicação. Pode ser usado para mostrar a arquitetura do sistema em questão. Nesse diagrama os retângulos em volta das classes representam o pacote, ou seja, conjunto de classes correlacionadas. Os retângulos menores são as classes pertecentes e as ligações representam a comunicação entre as classes.
### SD01
![diagrama_pacotes](../../assets/desenho/uml/diagrama_pacotes1.jpg)

### SD02
![diagrama_pacotes](../../assets/desenho/uml/diagrama_pacotes2.png)

### Diagrama de implantação
No contexto do UML o diagrama de implantação está relacionada a classificação de diagramas estruturais, pois descreve aspectos do sistema da aplicação em si. Esse diagrama é relacionado a parte física da aplicação, ou seja, a parte do hardware em que essa aplicação será implantada. Nesse diagrama as caixas em 3d são os nós da aplicação e os retângulos estão relacionados as classes da aplicação, no nosso caso os serviços, e a ligação entre elas são os protocolos de comunicação que fazem a ponte entre nós ou classes.
### ID01
![implementacao1](../../assets/desenho/uml/diagrama_implementacao1.png)
### ID02
![implantacao2](https://i.imgur.com/oFSxr4I.png)


## Referências
WIKIPEDIA, Diagrama de pacotes. Disponível em:
<https://pt.wikipedia.org/wiki/Diagrama_de_pacotes> Acesso em: 3 de maio de 2019  

Zanandrea, Pietro. Diagramas Estruturais da UML: Diagrama de pacotes. Disponível em: <http://micreiros.com/diagrama-de-pacotes/> Acesso em: 3 de maio de 2019

Macêdo, Diego. Introdução a UML e seus diagramas. Disponível em: <https://www.diegomacedo.com.br/introducao-a-uml-e-seus-diagramas/> Acesso em: 3 de maio de 2019

Ha Ilky, Kang Byungguk. " Cross Checking Rules to Improve Consistency between UML Static Diagram and Dynamic Diagram ".

M. Genero, M. Piatini, E. Manso, "Finding early indicators of UML class diagrams understandability and modifiability", Empirical Software Engineering 2004. ISESE '04. Proceedings. 2004 International Symposium on, pp. 207-216, 2004.

LUCIDCHART, O que é um diagrama de implementação. Disponível em: <https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml> Acesso em: 3 de maio de 2019

IBM, Diagrama de Implementação. Disponível em: <https://www.ibm.com/support/knowledgecenter/pt-br/SS4JE2_7.5.5/com.ibm.xtools.modeler.doc/topics/cdepd.html> Acesso em: 3 de maio de 2019
