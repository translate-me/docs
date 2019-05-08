# Documento de Visão

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
| 27/03/2019 | 0.1 | Adicionando template  | Gabriela e Renan |
| 01/04/2019 | 0.2 | Modificando template para preenchimento  | Alexandre Miguel |
| 08/04/2019 | 0.3 | Adicionando proposta no documento  | Victor Hugo |
| 08/04/2019 | 0.4 | Adicionando Oportunidade de Negócio  | Letícia Meneses |
| 09/04/2019 | 0.5 | Adicionando Documento Adicionais  | Letícia Meneses |
| 09/04/2019 | 0.6 | Adicionando abreviações  | Gabriela Guedes |
| 10/04/2019 | 0.7 | Adicionando Perspectiva do Produto  | Davi Alves |
| 10/04/2019 | 0.8 | Adicionando Funcionalidades do Produto e Definição dos Usuários  | Alexandre Miguel |
| 10/04/2019 | 0.9 | Adicionando Visão Geral e Definição dos Envolvidos  | Luiz Guilherme |
| 10/04/2019 | 0.9.1 | Adicionando Introdução  | Renan Schadt |
| 10/04/2019 | 0.9.2 | Adicionando Problema a Ser Resolvido  | Renan Schadt |
| 11/04/2019 | 0.9.3 | Adicionando Posicionamento do Produto  | Renan Schadt |
| 11/04/2019 | 0.9.4 | Adicionando Resumo dos Recursos | Rômulo Souza |
| 11/04/2019 | 0.9.5 | Adicionando Alternativas e Critérios de Qualidade | João Robson |
| 11/04/2019 | 1.0 | Adicionando Requisitos | Davi Alves |
| 22/04/2019 | 1.1 | Revisando Documento | Alexandre Miguel |
| 23/04/2019 | 2.0 | Revisão final do documento | Gabriela Guedes e Renan Schadt|


## 1. Introdução
O documento de visão define o escopo de alto nível do produto, o propósito do software a ser desenvolvido e seu valor mercadológico. Este visa estabelecer e nivelar as expectativas dos envolvidos, de modo a alinhar a visão dos stakeholders sobre o que exatamente é o software em questão.

### 1.1. Proposta  
Este documento tem como objetivo apresentar a ideia geral do webapp translate.me e com isso entender o contexto no qual o webapp está inserido.
O translate.me é um webapp, feito para comunicade acadêmica, que visa implementar um marketplace de tradução de textos de artigos científicos e livros.

### 1.2. Definições, Acronimos, e Abreviações

**UnB** - Universidade de Brasília

**FGA** - Faculdade do Gama, campus da UnB

**Desenho** - A matéria Arquitetura e Desenho de Software

**Translate.me** - Nome do sistema a ser desenvolvido

**Usuário Tradutor** - Usuário da aplicação responsável pela tradução de textos

**Usuário Autor** - Usuário da aplicação que submete textos para serem traduzidos   

**Stakeholders** - Partes envolvidas e interessadas na aplicação, como possíveis usuários, investidores, dentre outros

**RUP** - *Rational Unified Process*, Processo proposto pela IBM que fornece técnicas para aumentar a produtividade da equipe

**Webapp** - Aplicação Web

**Freelancer** - Proficional autonomo que se autoemprega em diferentes empresas utilizando de seu tempo livre.

**Gamificação** - Uso de macânicas e dinâmicas de jogos para engajar pessoas, resolver problemas e melhorar o aprendizado.

**Front-end** - Interface de interação com o usuário

**Back-end** - Sistema responsável pelas regras de negócio da aplicação

### 1.3. Visão Geral

O **Translate.me** é um projeto criado para a disciplina de Desenho de Software da Universidade de Brasília, na Faculdade do Gama (FGA) e é uma aplicação web que servirá como uma ferramenta de aproximação entre um cliente que precisa de uma tradução profissional e tradutores freelancers que buscam uma alternativa extra de renda.

O público-alvo da aplicação são estudantes acadêmicos que produzem artigos científicos, relatórios, documentam processos ou demais atividades acadêmicas que buscam relevância internacional com sua publicação. Assim, um estudante brasileiro que não possui uma proficiência em uma determinada língua pode ter a sua publicação traduzida em diversos idiomas, por um tradutor que a domina e que busca realizar esse serviço de forma centralizada. Com isso, o público-alvo também passa a ser os tradutores profissionais.

A criação do **Translate.me** surge da ideia de facilitar o encontro entre um cliente e um especialista em tradução, porém, diferenciando-se do disposto atualmente no mercado, a plataforma descentraliza a tradução feita por somente um tradutor, permitindo a tradução de textos privados, estudos não-publicados, patentes e demais propriedades intelectuais que poderiam ter seu conteúdo exposto se a tradução é realizada somente por um profissional.

Este documento está organizado de acordo com a metodologia **RUP**, o *Rational Unified Process* , definindo o problema a ser resolvido, os requisitos do software, o momento do mercado no qual o projeto se encaixa, a utilização da aplicação desejada e os usuários, levantamentos sobre metodologia de desenvolvimento do software e os processos utilizados, um esboço do cronograma de desenvolvimento e sua documentação.

## 2. Posicionamento
O **Translate.me** ataca o nicho de tradução científica, para usuários que demandam uma tradução de alto nível. Trazendo diferenciais como divisão de textos entre tradutores, elementos de gamificação e preço acessível. Este tópico demonstra como o produto se encaixa no mercado e quais são seus diferenciais para obter destaque.  

### 2.1. Oportunidade de Negócio
O **Translate.me** oferece uma plataforma de serviço de tradução de artigos e documentos, fazendo a ligação entre o usuário que precisa de uma tradução e o usuário tradutor.

O serviço automatizado visa solucionar a demanda de traduções de artigos, em que muitas vezes o escritor/pesquisador não possui o conhecimento para traduzir seus textos, precisando assim de alguém que possa fazer isso, com qualidade e segurança.

O objetivo da aplicação é facilitar e automatizar os processos do serviço de tradução de textos, o qual um cliente tem a necessidade de tradução, disposto a pagar pelo serviço, e um tradutor que deve receber um valor justo pelo trabalho feito. Logo, o Translate.me intermedia essa transação para que ambas partem possam ser beneficiadas, contando com uma estratégia de segurança na tradução do artigo, diversidade de tradutores para o mesmo documento evitando a exposição total do texto e garantindo qualidade e revisão de tradução. Entre todo os trâmites nesse fluxo, o Translate.me deve ganhar uma porcentagem do valor da tradução de até 15%, partindo daí o capital gerado pelo sistema.

### 2.2. Problema a Ser Resolvido
| O problema de | Falta de proficiência para traduzir um texto complexo para outra língua |
|:---:|:---:|
| Afeta | Acadêmicos e outros profissionais que desejam que seu trabalho supere a barreira linguística |
| Cujos impactos são | Desempenho ruim em conferências e oportunidades de negócio perdidas |
| Uma boa solução seria | Um software com a função de conectar usuários com pessoas capazes na língua em questão, para que seja feito o serviço de tradução |


### 2.3. Posicionamento do Produto
| Para | Profissionais |
|:---:|:---:|
| Que | Desejam que seus trabalhos sejam traduzidos para diferentes línguas |
| O translate.me | É um website |
| Que | Visa conectar tradutores e clientes, para que seja efetuado o serviço de tradução |
| Diferente de | Websites similares que não permitem acompanhamento do processo e comunicação entre as partes envolvidas |
| Nosso produto | Oferece uma fórmula modularizada e interativa de tradução a um preço acessível |


## 3. Perfil dos Usuários, Envolvidos e Mercado    
Os envolvidos na utilização da plataforma podem ser simplificados na tabela abaixo:

|Representantes|Descrição|Tipo|Responsabilidades|Envolvimento|
|:---:|:---:|:---:|:---:|:---:|
|Estudantes de Línguas Estrangeiras|Estudantes, não-certificados que possuem conhecimento em uma ou várias línguas estrangeiras|Usuário interessado que não atua profissionalmente como tradutor ainda e busca melhorar|Realizar traduções de textos simples e textos auxiliares|Médio|
|Graduados e Professores de Línguas Estrangeiras|Estudantes e professores certificados que possuem conhecimento avançado em uma ou várias línguas estrangeiras|Usuário que trabalha como tradutor profissional e busca uma forma fácil de realizar sua atividade profissional|Realizar traduções técnicas, de cunho acadêmicos e revisão de textos já traduzidos|Alto|
|Estudantes autores de textos acadêmicos|Estudantes acadêmicos de diferentes níveis que buscam traduzir uma produção acadêmica de sua autoria|Usuário com pouca proficiência em uma determinada língua que busca contratar um profissional de tradução|Definir o texto a ser traduzido, dividí-lo e categorizá-lo|Alto|

### 3.1. Definição dos Envolvidos
A definição de envolvidos no projeto (stakeholders) é bastante confusa dentro da engenharia de software. Neste projeto, será assumido que os envolvidos são todos os interessados na criação e utilização do software da melhor forma possível, assim são definidos os seguintes stakeholders:

#### 3.1.1 Usuários finais da aplicação
São estes os usuários descritos no próximo tópico, dentre eles são os utilizadores da plataforma, que são alunos com proficiência para tradução de textos mais simples e auxiliares; professores e profissionais de tradução, que são responsáveis pelas traduções mais técnicas e acadêmicas e por fim o cliente que contrata o serviço de tradução oferecido.

#### 3.1.2 Desenvolvedores
Os desenvolvedores do projeto consiste em um grupo de dez alunos do curso de Engenharia de Software da UnB que cursam a disciplina de Desenho de Software no primeiro semestre do ano de 2019 na Universidade de Brasília. Estes são os responsáveis pela documentação, desenvolvimento da aplicação, idealização e manutenção da plataforma. A lista dos desenvolvedores pode ser encontrada na [página inicial do repositório da aplicação](https://translate-me.github.io/docs/)

#### 3.1.3 Professores e Monitores da disciplina
Por fim, existem também os stakeholders que avaliam a disciplina, cujo foco é este projeto. Os alunos são coordenados pela professora Milene Serrano e pelo conjunto de monitores. Seus objetivos são definir critérios de qualidade, prazos de entrega e atribuir determinados padrões de projeto que devem ser adotados no decorrer do desenvolvimento.

### 3.2. Definição dos Usuários  

Os usuários no contexto da aplicação são:

#### 3.2.1. Estudantes de Línguas Estrangeiras

São estudantes que, a medida que desenvolvem o aprendizado em uma língua estrangeira, sentem-se aptos a realizar serviços de traduções, ainda que conscientes das limitações de seu conhecimento, porém representando uma quantidade significativa de possíveis usuários, que agilizam o processo de tradução.

#### 3.2.2. Graduados e Professores de Línguas Estrangeiras

Representam envolvidos com alto conhecimento da língua estrangeira em questão e que podem prestar serviços mais especializados de tradução ou revisão, na expectativa de receberem pagamentos maiores do que estudantes da área, com menos flexibilidade para serviços de tradução, porém com maior garantia de qualidade.

#### 3.2.3. Estudantes autores de textos acadêmicos

São estudantes de diversas áreas do conhecimento que elaboraram textos acadêmicos e desejam submete-los para algum contexto internacional, sejam seminários ou avaliações de bancas acadêmicas, fazendo necessária a tradução desse material de forma especializada e coerente, o que foge de seus conhecimentos na língua em específico, pelo uso de expressões e termos nativos.

### 3.3. Alternativas e Competição   
Existem algumas soluções que realizam a tradução de texto por meio de uma plataforma digital. Considerando serviços de tradução instantânea, que são genéricos e não são especializados em determinado tipo ou tema específico de texto, podemos citar o Google Tradutor e o Yandex. Tratando-se de serviços para tradução que têm o foco em traduções de manuscritos ou artigos científicos, alguns podem ser destacados, como mostrado abaixo:

#### 3.3.1. [EditingServices](https://www.tandfeditingservices.com/services/translation.html)
Proveem serviços de edição e tradução, com fases dedicadas a revisão do texto traduzido por especialistas em revisão gramatical e semântica.

#### 3.3.2. [Editage](https://www.editage.com/translation-services/brazilian-portuguese-to-english-translation.html)
Serviço especializado em tradução de documentos acadêmicos, formado por tradutores de várias áreas que combinam seu conhecimento para entregar um documento perfeitamente traduzido.


## 4. Definição do Produto
O **Translate.me** trata-se de uma plataforma de tradução de textos e artigos acadêmicos. A especificidade e limitação do público e do tema se deve à preocupação dos desenvolvedores deste projeto com os direitos autoriais dos textos em processo de tradução. Além disso, houve também uma preocupação em atender ao público de pessoas que possuem certificação em língua estrangeira, permitindo que atuem como _freelancers_ neste projeto. A gamificação será uma metodologia presente no **Translate.me** , como forma de incentivar que os usuários se mantenham conectados à plataforma e em uso constante da mesma.

### 4.1. Perspectiva do Produto

O produto tem como principal caracteristica ajudar não somente a pessoa que deseja a tradução de seu artigo, mas também os envolvidos que estão fazendo o trabalho requerido. Com diferenciais de segurança na submissão de seu documento, comunicação com o tradudor e por fim incetivos baseados em gamificação na plataforma.

### 4.2. Resumo dos Recursos

Dentre os principais recursos oferecidos pelo **Translate.me**, estão os serviços de cadastro, login e logout de usuário; inserção, tradução e revisão de textos; sistema de pagamento; chat e acompanhamento entre autores e tradutores; sistema de nivelamento entre os tradutores.


## 5. Funcionalidades do Produto

Os recursos e funcionalidades do webapp **Translate.me** compreendem serviços implementados de forma independente, buscando atender as necessidades identificadas dos usuários da plataforma, aqui descritos em ordem de prioridade.

### 5.1. Login e Cadastro

A aplicação possui um sistema para cadastro de usuários em conexão direta com o sistema de Login, fazendo uso tanto de um método nativo para o fluxo de registro, quanto métodos que integrem informações de outras aplicações (como Facebook ou Google), permitindo acesso facilitado ao usuário.

### 5.2. Submissão de texto

O **Translate.me**, para cumprir com sua função principal de propiciar a tradução, possui a funcionalidade de submissão de textos em formatos que propiciem diferentes etapas de funcionalidades que compõem o restante da aplicação, como a fragmentação de textos.

### 5.3. Fragmentação de textos

Para separar o texto completo a ser traduzido em módulos menores, impedindo que um único tradutor tenha contato com todo o conteúdo, a aplicação conta com a funcionalidade de separação do texto em fragmentos, por meio de indicação do usuário autor dos pontos em que cada fragmento se inicia e finaliza.

### 5.4. Estimativa de Dados

Visando garantir a integridade do texto e uma estimativa de dados como o tempo total de tradução, a aplicação conta com um sistema de medição de informações para que o usuário autor possa realizar planejamentos de custos, prazos e segurança do arquivo traduzido que receberá, analisando métricas coletadas automaticamente pela aplicação e as repassando em formato amigável ao usuário autor.

### 5.5. Acompanhamento de tradução

Durante o período de tradução, o sistema conta ainda com um suporte ao usuário que informa a porcentagem da correção, permitindo um acompanhamento do processo antes da efetiva entrega do texto traduzido, sendo ainda uma forma de fornecer ao usuário a possibilidade de replanejamento de prazos conforme o ritmo de tradução.

### 5.6. Revisão de tradução

Para mitigar traduções errôneas, a aplicação conta com um sistema que limita a quantidade de correções disponíveis para o usuário tradutor mediante revisão de traduções de terceiros, para garantir que um texto traduzido tenha tido contato com mais de uma fonte de tradução, dificultando assim a propagação de erros no arquivo traduzido.

### 5.7. Sistema de Gamificação

Como forma de motivação dos usuários tradutores, seja para maior participação na plataforma ou para contribuição com outros tradutores por meio das correções, a aplicação institui um sistema de gamificação com pontuações e rankings, que se refletem em priorizações de traduções ou, em casos negativos, a penalidades como suspensão temporária ou definitiva. Esse sistema leva em conta, ainda, a afinidade do usuário tradutor com a língua utilizada.

### 5.8. Contato Anônimo

A Aplicação **Translate.me** possui ainda um sistema de comunicação entre tradutor e autor, porém estabelecendo critérios rígidos de anonimato em ambas as pontas, garantindo que determinados usuários não sejam beneficiados por motivos que saem do escopo da aplicação ou do método gamificado.


## 6. Restrições  

### 6.1. Restrições de Design   
O webapp deve ter um design de alta compreensão e acessibilidade.

### 6.2. Restrições de Implementação   
A aplicação será implementada em *Python* com framework *Django*, *Rest Framework*  e *React*. E será dividido em microsserviços.

### 6.3. Restrições de Segurança   
O aplicativo não será responsável por copyright dos textos submetidos com taxa abaixo 50% de privacidade (índice medidos com métricas do site).

### 6.4. Restrições de Design   
Por se tratar de uma aplicação web, uma restrição do projeto é possuir acesso a uma conexão estável e navegadores compatíveis com os listados no projeto para acessar o webapp.

## 7. Critérios de Qualidade

### 7.1 - Testes unitários

Serão utilizados testes unitários em cada microsserviço criado no back-end para garantir a alta qualidade do codigo.

### 7.2 - Usabilidade

No front-end, os componentes do [Material-UI](https://material-ui.com/) serão utilizados. Eles são baseados no [Material Design](https://material.io/), uma linguagem visual que provê boas práticas de design e acessibilidade para criar produtos de alta qualidade.

## 8. Requisitos   

Os requisitos podem ser acessados diretamente no documento elaborado, acessado a [Tabela de Requisitos](../../../requisitos/tabela_requisitos).


## 9. Documentação Adicional
A plataforma dispõe de documentos gerais como FAQ, informações sobre a equipe e formas de contato.
Acerca do FAQ do **Translate.me** , são reunidas as dúvidas mais frequentes, sendo criados links que levam a resolução desse problema ou um esclarecimento sobre determinado assunto. Mesmo que a dúvida do usuário não se enquadre nas expostas, existe o campo para fazer próprias perguntas, e será dado todo o suporte para o esclarecimento e resolução de alguma pendência para o usuário.

Conjuntamente as documentações adicionais apresentadas ao usuário, a equipe aborda informações sobre os integrantes e dados técnicos sobre o sistema, por conseguinte aborda formas de contato com os responsáveis pelo **Translate.me** .

## 10. Referências

 *  [Template de Documento de Visão](https://www.ibm.com/support/knowledgecenter/pt-br/SSYMRC_6.0.5/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.html)

 * [Definição de RUP](https://pt.wikipedia.org/wiki/IBM_Rational_Unified_Process)

 * [Editage](https://www.editage.com/translation-services/brazilian-portuguese-to-english-translation.html)
