# Definição de Tema

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
| 12/04/2019 | 1.0 | Primeira versão do documento | Gabriela Guedes |
| 02/05/2019 | 1.1 | Refatoração do documento, adição dos tópicos 3 e 4 | Renan Schadt |


## 1. Introdução

## 2. Design Sprint

## 3. Artefatos Construídos
Para idealização e elucidação das propostas de tema, foram construídos diversos artefatos, abaixo estão descritos quais são, o que são, seu propósito e porque o fizemos. Uma descrição mais detalhada dos artefatos do tema escolhido, pode ser encontrada na pasta "Requisitos", sub-pasta "Modelagem".

### 3.1 Rich Picture
Um rich picture é um desenho de uma situação ou fluxo, que ilustra seus elementos e relacionamentos. Pode conter imagens, textos, símbolos, ícones, entre outros elementos usados para ilustrar algo graficamente. Ele ajuda a entender e desmantelar processos complexos, se baseando no fato de que nosso cerébro consegue absorver melhor imagens do que palavras.

### 3.2 5W2H
O 5W2H é um método simples e de fácil aplicação para elucidar a visão dos stakeholders sobre o produto, respondendo sete questões fundamentais, que dão o nome ao método.
1. O que será feito? Descrição do produto (What).
2. Por que será feito? Razão de existência do produto (Why).
3. Onde será feito? Local onde é feito o desenvolvimento (Where).
4. Quando será feito? Datas, prazos (When).
5. Quem irá fazer? Responsáveis pelo produto (Who).
6. Como será feito? Metodologia, processos envolvidos (How).
7. Quanto irá custar? Custo de desenvolvimento, despesas envolvidas (How much).

### 3.3 Mapa Mental
Um mapa mental é uma ilustração de diversos objetos e suas conexões, tem o propósito de elucidar o entendimento de um tema e conectar seus elementos. Pode ser aplicado em diversas áreas do conhecimento, mapeando este assunto, fixando e amadurecendo o conhecimento dos indivíduos neste.

### 3.4 Protótipo
Um protótipo de software, é uma previsão de como a aplicação será visualmente, quando terminado seu período de desenvolvimento. Seu principal propósito é ser mostrado aos __stakeholders__, para que avaliem o direcionamento do produto e determinem possíveis oportunidades de melhora.


## 4. Propostas de Tema

### 4.1 Marketplace de Video Aulas

#### 4.1.1 Definição
Uma das ideias do grupo, foi a construção de um marketplace de vídeo aulas, onde é possível adquirir cursos e criar seus próprios para a venda. Foi pensado, tendo em mente plataformas como a Udemy, com um incentivo a alunos para criarem cursos das suas áreas de domínio. Conta com diversas funcionalidades extras para dar suporte ao produto, como busca inteligente, listas de desejo, cupons de desconto, foruns de dúvida, entre outros.

Os artefatos abaixo mostram mais detalhes sobre o produto e caracterizam as fases de __sketch__ e __prototype__ do Design Sprint.

#### 4.1.2 Mapas Mentais
Mapa mental mostrando conexão entre áreas da aplicação e algumas regras de negócio.
![Marketplace2](assets/definicao_tema/mapa_mental_marketplace2.jpg)

Mapa mental mostrando parte do conteúdo das principais áreas da aplicação.
![Marketplace](assets/definicao_tema/mapa_mental_marketplace.png)

#### 4.1.3 Rich Picture
Rich picture desenhado a mão ilustrando pequenos protótipos das áreas principais da aplicação.
![richpicture](assets/definicao_tema/richpicture_marketplace.jpg)

### 4.2 Crawler para Mineração de Dados

#### 4.2.1 Definição
Uma das ideias do grupo, foi a construção de um crawler para mineração de dados, embasada pela experiência de alguns membros, na dificuldade de se obter bases de dados para uso em algoritmos de inteligência artificial. 

"Os crawlers coletam documentos de base de dados para que estes possam ser analisados, indexados, procurados e extraídos (IBM)". A aplicação prevista, iria vender diferentes crawlers para diferentes propósitos, como crawlers para extração em bancos não relacionais, arquivos de texto, entre outros. 

Seguindo os princípios do Design Sprint, os artefatos abaixo caracterizam as fases de __sketch__ e __prototype__.

#### 4.2.2 5W2H
1. What ?
	* O produto a ser feito é um marketplace que venderá dados que serão gerados através de um crawler ou, como é dito no meio de DataScience, será feito um data mining.
	* O produto também vai funcionar como um sistema de requisições de dados, ou seja, conforme a necessidade dos clientes que usaram o site, um crawler específico será feito para aquela pessoa caso seja assinado o pacote premium do site.
2. When ?
	* Tudo será produzido no tempo da disciplina, de no mínimo um MVP do escopo feito no começo do semestre e o máximo de entrega final dos seminários ao final da matéria, sendo este o prazo total de produção.
3. Who ?
	* Todo o serviço será feito pelo grupo que foi determinado no começo da matéria.
4. Where ?
	* Todo o trabalho será feito na UnB, campus do Gama, nos locais predeterminados pelo grupo, nos pareamentos e nas reuniões.
5. Why?
	* Esse produto será feito graças a uma necessidade em obter dados para aprendizado de máquina e estudos de mercados no geral, relatados em artigos como:   

    |Tipo|Assunto|Link|
    |	---	| ---	 | --- |
    |Fórum|O que é mais importante? Bons dados ou Bons algoritmos?|https://www.quora.com/Is-good-data-or-good-algorithm-more-important-in-machine-learning
    |Artigo| Desmitificando aprendizado de máquina: A importancia de dados|https://www.quora.com/Is-good-data-or-good-algorithm-more-important-in-machine-learning|
    |Artigo| A importancia da coleta de dados para seu negócio|https://www.simplybusiness.co.uk/knowledge/articles/2010/06/2010-06-03-why-marketing-data-is-important-to-a-growing-business/|
    |Artigo Científico|Reality Check: Combinando Experiências de Escolha com Dados de Mercado para Estimar a Importância dos Atributos do Produto.|https://pubsonline.informs.org/doi/pdf/10.1287/mnsc.1090.1136|
    |Artigo científico|Sistemas e métodos para aprendizado de máquina e gerenciamento de dados|https://patentimages.storage.googleapis.com/21/3d/63/eaa0b260547816/US6845340.pdf|
    |Artigo científico|Tecnicas de aprendizado de máquina para mineração de dados: A pesquisa|https://ieeexplore.ieee.org/abstract/document/6724149/|

6. How ?
	* Esse produto será feito em Django e React com banco de dados não relacional. Terá um estudo de requisitos dentro de mercado, o qual será exposto pelo grupo, como dispor os dados da melhor maneira para os pesquisadores e as empresas que os necessitem para a realização e desenvolvimento de suas próprias pesquisas internas.
	* Será usado um método misto para o gerenciamento da equipe usando documentos essenciais do RUP, gerenciamento do scrum, algumas documentações e estilo de pareamento do extreme programing.

7. How much?
	* A precificação será realizada após a escolha do tema do grupo.

#### 4.2.3 Protótipo
Protótipo de baixa fidelidade ilustrando a tela inicial do marketplace de crawlers.
![Prototipo Crawler](assets/definicao_tema/prototipo_crawler.png)


### 4.3 WebApp para Tradução de Artigos

#### 4.3.1 Definição 
Um dos projetos pensados pelo grupo foi uma aplicação web que serve como uma ferramenta de aproximação entre um cliente que precisa de uma tradução profissional e tradutores freelancers que buscam uma alternativa extra de renda. A ideia do projeto se originou a partir da dificuldade de se traduzir um texto acadêmico e do preço elevado cobrado por profissionais da área. 

A plataforma pensada pelo grupo descentraliza a tradução, para que não seja feita por somente um tradutor, permitindo a tradução de textos privados, estudos não-publicados, patentes e demais propriedades intelectuais que poderiam ter seu conteúdo exposto se a tradução é realizada somente por um profissional.

#### 4.3.2 Mapa Mental
Mapa mental com foco nos dois tipos de usuários da aplicação, mostrando algumas de suas ações.
![mapa_mental_traducao](assets/requisitos/elicitacao/mapa_mental_traducao.png)

#### 4.3.3 Rich Pictures
Rich picture ilustrando caminho do artigo ao ser traduzido.
![richpicture_traducao_1](assets/requisitos/elicitacao/richpicture_traducao_1.png)

Rich picture com foco na interação entre usuário e tradutor.
![richpicture_traducao_2](assets/requisitos/elicitacao/richpicture_traducao_2.jpg)

Rich picture ilustrando a divisão do texto original em fragmentos, distribuídos entre tradutores.
![richpicture_traducao_3](assets/requisitos/elicitacao/richpicture_traducao_3.jpg)

## 5. Conclusão
**Tema:** Com todas as ideias apresentadas, realizamos uma votação que buscava enfim decidir qual projeto seria o executado no decorrer da disciplina.

![votacao](assets/definicao_tema/votacao.png)

Assim, o tema escolhido foi o da **Plataforma para Tradução de Artigos**

## 6. Referências
* [Crawler](https://www.ibm.com/support/knowledgecenter/pt-br/SS5RWK_3.5.0/com.ibm.discovery.es.nav.doc/iiysaovcompc.htm)
* [5W2H](https://www.heflo.com/blog/action-plan/5w2h-method/)
* [Desmitificando aprendizado de máquina: A importancia de dados](https://www.quora.com/Is-good-data-or-good-algorithm-more-important-in-machine-learning)
* [A importancia da coleta de dados para seu negócio](https://www.simplybusiness.co.uk/knowledge/articles/2010/06/2010-06-03-why-marketing-data-is-important-to-a-growing-business/)
* [Reality Check: Combinando Experiências de Escolha com Dados de Mercado para Estimar a Importância dos Atributos do Produto](https://pubsonline.informs.org/doi/pdf/10.1287/mnsc.1090.1136)
* [Sistemas e métodos para aprendizado de máquina e gerenciamento de dados](https://patentimages.storage.googleapis.com/21/3d/63/eaa0b260547816/US6845340.pdf)
* [Tecnicas de aprendizado de máquina para mineração de dados: A pesquisa](https://ieeexplore.ieee.org/abstract/document/6724149/)

* [Rich Picture](http://www.mspguide.org/tool/rich-picture)
