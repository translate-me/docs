# GoFs Estruturais

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---| |
| 23/05/2019 | 0.1 | Inclusão do GoF Adapter | Helena Goulart |

## Adapter

### Definição

Trata-se de um padrão que converte a interface de uma classe para outra interface. Isso normalmente ocorre quando classes precisam trabalhar mas possuem interfaces incompatíveis entre si.

### Análise

Pode ser utilizado no translate.me, contudo não soa como uma boa prática: uma vez que o projeto terá seu início e fim acompanhando a disciplina Desenho e Arquitetura de Software, escopo reduzido e conter diagrama de classes e de arquitetura bem definidos, não tende a ser um sistema que vai adotar novas bibliotecas e que passará por adaptações a serem implementadas pelo _Adapter_.

### Estrutura mínima

![AdapterPattern](/assets/desenho/padroes/Padro_Adapter.jpg)

## Bridge

### Definição

### Análise

### Estrutura mínima

## Composite

### Definição
Trata-se do agrupamento de objetos de modo a representar hierarquias parte-todo, permitindo tratar objetos individuais e composições uniformemente.

### Análise

Pode ser utilizado no translate.me, inclusive é um padrão recomendado que o utilizem pois ele se encaixa com o escopo do projeto, uma vez que contempla a estrutura de editor de texto. Editores são compostos por elementos individuais, tais como palavras e letras, enquanto o texto é um elemento parte-todo, pois contém várias palavras dentro dele.  

### Estrutura mínima

![Composite](/assets/desenho/padroes/Composite.png)




## Referências

### Links de sites
[1] Para conferir as referências do Adapter, [clique aqui](https://www.devmedia.com.br/padrao-de-projeto-adapter-em-java/26467). <br>
[3] Para conferir as referências do Composite [clique aqui](http://www.dsc.ufcg.edu.br/~jacques/cursos/map/html/pat/composite.htm).

### Livros e artigos
[1] HUMMEL, Oliver; ATKINSON, Colin. The managed adapter pattern: Facilitating glue code generation for component reuse. In: International Conference on Software Reuse. Springer, Berlin, Heidelberg, 2009. p. 211-224.
