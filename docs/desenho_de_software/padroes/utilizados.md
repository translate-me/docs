# Padrões Utilizados

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|:---:|:---:|:---:|:---:|
| 30/06/2019 | 0.1 | Adicionando definição dos padrões utilizados pelo framework | Alexandre Miguel |

## Padrões Implementados pelo Grupo

Os seguintes padrões foram implementados no Backend do produto gerado, utilizando o Django REST Framework.

### Composite

O Padrão **Composite** foi implementado para a criação dos tipos de elementos textuais na aplicação, dado que foi implementada uma classe abstrata TextComponent que serviu pa

### Iterator

### Observer

Dada a necessidade de criação de Notificações de acordo com a transição de estados, foi utilizada a implementação de um padrão **Observer** que identifica a transição de estados de tradução do texto, permitindo comportamentos diferentes para a criação de notificações de acordo com o usuário alvo daquela notificação (como Autores, Tradutores e Revisores). Em uma primeira versão, o padrão foi aplicado individualmente e, em uma versão posterior, seu funcionamento foi associado ao funcionamento do padrão State.

#### Estrutura Padrão

##### Diagrama de Sequência

![observer_sequence_diagram](../../assets/desenho/padroes/observer-sequence-diagram.png)

#### Estrutura Adaptada

![observer_sequence_diagram_real](../../assets/desenho/padroes/observer-sequence-diagram-real.png)

### State



### Front Controller


## Padrões Implementados pelo Django REST Framework

## Referências

- [Padrão Observer](https://refactoring.guru/design-patterns/composite)
