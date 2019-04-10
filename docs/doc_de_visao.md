## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
| 27/03/2019 | 0.1 | Adicionando template | Gabriela e Renan |
| 01/04/2019 | 0.2 | Modificando template para preenchimento  | Alexandre Miguel |
|  08/04/2019 | 0.3  | Adicionando proposta no documento  |  Victor Hugo  |
|  09/04/2019 | 0.4  | Adicionando abreviações  |  Gabriela Guedes  |
|  10/04/2019 | 0.5  | Adicionando Perspectiva do Produto  |  Davi Alves  |
|  10/04/2019 | 0.6  | Adicionando Funcionalidades do Produto e Definição dos Envolvidos  |  Alexandre Miguel  |

### 1. Introdução  

#### 1.1. Proposta  
<p> Este documento tem como objetivo apresentar a ideia geral do webapp translate.me e com isso entender o contexto no qual a webapp está inserido.</p>
<p> O translate.me é uma webapp, feito para comunicade acadêmica, que visa implementar um marketplace de tradução de textos de artigos científicos e livros.</p>

#### 1.2. Escopo  

#### 1.3. Definições, Acronimos, e Abreviações

**UnB** - Universidade de Brasília

**FGA** - Faculdade do Gama, campus da UnB

**Desenho** - A matéria Arquitetura e Desenho de Software

**Translate.me** - Nome do sistema a ser desenvolvido

**Usuário Tradutor** - Usuário da aplicação responsável pela tradução de textos

**Usuário Autor** - Usuário da aplicação que submete textos para serem traduzidos   

#### 1.4. Visão Geral
---

### 2. Posicionamento     

#### 2.1. Oportunidade de Negócio
<p> O Translate.me oferece uma plataforma de serviço de tradução de artigos e documentos, fazendo a ligação entre o usuário que precisa de uma tradução e o usuário tradutor. </p>

<p> O serviço automatizado visa solucionar a demanda de traduções de artigos, em que muitas vezes o escritor/pesquisador não possui o conhecimento para traduzir seus textos, precisando assim de alguém que possa fazer isso, com qualidade e segurança.</p>

<p> O objetivo da aplicação é facilitar e automatizar os processos do serviço de tradução de textos, o qual um cliente tem a necessidade de tradução, disposto a pagar pelo serviço, e um tradutor que deve receber um valor justo pelo trabalho feito. Logo, o Translate.me intermedia essa transição para que ambas partem possam ser beneficiadas, contando com uma estratégia de segurança na tradução do artigo, diversidade de tradutores para o mesmo documento evitando a exposição total do texto e garantindo qualidade e revisão de tradução. Entre todo os trâmites nesse fluxo, o Translate.me deve ganhar uma porcentagem do valor da tradução de até 15%, partindo dai o capital gerado pelo sistema.</p>

#### 2.2. Problema a Ser Resolvido  

#### 2.3. Posicionamento do Produto
---
### 3. Perfil dos Usuários, Envolvidos e Mercado    

#### 3.1. Definição dos Envolvidos  

Os envolvidos ou partes interessadas no contexto da aplicação são:

##### 3.1.1. Estudantes de Línguas Estrangeiras

São estudantes que, a medida que desenvolvem o aprendizado em uma língua estrangeira, sentem-se aptos a realizar serviços de traduções, ainda que conscientes das limitações de seu conhecimento, porém representando uma quantidade significativa de possíveis usuários, que agilizam o processo de tradução.

##### 3.1.2. Graduados e Professores de Línguas Estrangeiras

Representam envolvidos com alto conhecimento da língua estrangeira em questão e que podem prestar serviços mais especializados de tradução ou revisão, na expectativa de receberem pagamentos maiores do que estudantes da área, com menos flexibilidade para serviços de tradução, porém com maior garantia de qualidade.

##### 3.1.3. Estudantes autores de textos acadêmicos

São estudantes de diversas áreas do conhecimento que elaboraram textos acadêmicos e desejam submeter esses textos para algum contexto internacional, sejam seminários ou avaliações de bancas acadêmicas, fazendo necessária a tradução desse texto de forma especializada e coerente, o que fogem de seus conhecimentos na língua em específico, pelo uso de expressões e termos nativos.



#### 3.2. Definição de Usuários  

#### 3.3. Alternativas e Competição   
---

### 4. Definição do Produto

#### 4.1. Perspectiva do Produto

<p>O produto tem como principal caracteristica ajudar não somente a pessoa que deseja a tradução de seu artigo, mas também os envolvidos em que estão fazendo o trabalho requerido. Com diferenciais de segurança na submição de seu documento, cominicação com o tradudor e por fim incetivos baseados em gamificação na plataforma.</p>

#### 4.2. Resumo dos Recursos

---
### 5. Funcionalidades do Produto

Os recursos e funcionalidades do webapp ***translate.me*** compreendem serviços implementados independentemente, buscando atender as necessidades identificadas dos usuários da plataforma, aqui descritos em ordem de prioridade.

#### 5.1. Login e Cadastro

A Aplicação possui um sistema para cadastro de usuários em conexão direta com o sistema de Login, fazendo uso tanto de um método nativo para o fluxo de registro, quanto métodos que integrem informações de outras aplicações (como Facebook ou Google), permitindo acesso facilitado ao usuário.

#### 5.2. Submissão de texto

O ***translate.me***, para cumprir com sua função principal de propiciar a tradução, possui a funcionalidade de submissão de textos em formatos que propiciem diferentes etapas de funcionalidades que compõem o restante da aplicação, como a fragmentação de textos.

#### 5.3. Fragmentação de textos

Para separar o texto completo a ser traduzido em módulos menores, impedindo que um único tradutor tenha contato com todo o conteúdo, a aplicação conta com a funcionalidade de separação do texto em fragmentos, por meio de indicação do usuário autor dos pontos em que cada fragmento se inicia e finaliza.

#### 5.4. Estimativa de Dados

Visando garantir a integridade do texto e uma estimativa de dados como o tempo total de tradução, a aplicação conta com um sistema de medição de informações para que o usuário autor possa realizar planejamentos de custos, prazos e segurança do arquivo traduzido que receberá, analisando métricas coletadas automaticamente pela aplicação e as informando em formato amigável ao usuário autor.

#### 5.5. Acompanhamento de tradução

Durante o período de tradução, o sistema conta ainda com um suporte ao usuário que informa a porcentagem da correção, permitindo um acompanhamento do processo antes da efetiva entrega do texto traduzido, sendo ainda uma forma de fornecer ao usuário a possbilidade de replanejamento de prazos conforme o ritmo de tradução.

#### 5.6. Revisão de tradução

Para mitigar traduções errôneas, a aplicação conta com um sistema que limita a quantidade de correções disponíveis para o usuário tradutor mediante revisão de traduções de terceiros, para garantir que um texto traduzido tenha tido contato com mais de uma fonte de tradução, dificultando assim a propagação de erros no arquivo traduzido.

#### 5.7. Sistema de Gamificação

Como forma de motivação dos usuários tradutores, seja para maior participação na plataforma ou para contribuição com outros tradutores por meio das correções, a aplicação institui um sistema de gamificação com pontuações e rankings, que se refletem em priorizações de traduções ou, em casos negativos, a penalidades como suspensão temporária ou definitiva. Esse sistema leva em conta, ainda, a afinidade do usuário tradutor com a língua utilizada.

#### 5.8. Contato Anônimo

A Aplicação ***translate.me*** possui ainda um sistema de comunicação entre tradutor e autor, porém estabelecendo critérios rígidos de anônimato em ambas as pontas, garantindo que determinados usuários não sejam beneficiados por motivos que saem do escopo da aplicação ou do método gamificado.

---
### 6. Restrições   
#### 6.1. Restrições de Design   
<p> O webapp tem que ter um design de alta compreensão e acessibilidade.</p>

#### 6.2. Restrições de Implementação   
<p> A aplicação será implementada em python com framework Django, Rest Framework  e React. E será dividido em microserviços.</p>

#### 6.3. Restrições de Segurança   
<p> O aplicativo não será responsável por copyright dos textos submetidos com taxa abaixo 50% de privacidade(indice medidos com métricas do site).</p>

#### 6.4. Restrições de Design   
<p> Por se tratar de uma aplicação na web uma restrição do projeto é possuir acesso a uma internet estável e navegadores compatíveis com os listados no projeto para acessar o webapp.</p>

### 7. Critérios de Qualidade
---
### 8. Requisitos    
---
### 9. Documentação Adicional
<p> A plataforma dispõe de documentos gerais como FAQ, informações sobre a equipe e formas de contato. </p>
<p> Acerca do FAQ do Translate.me, são reunidas as dúvidas mais frequentes, sendo criados links que levam a resolução desse problema ou um esclarecimento sobre determinado assunto. Mesmo que a dúvida do usuário não se enquadre nas expostas, existe o campo para fazer próprias perguntas, e será dado todo o suporte para o esclarecimento e resolução de alguma pendencia para o usuário. </p>
<p> Conjuntamente as documentações adicionais apresentada ao usuário, as informações sobre o software e a equipe integra as documentações para usuários, aborda informações sobre os integrantes e dados técnicos sobre o sistema, por conseguinte aborda formas de contato com os responsáveis pelo Translate.me.

### 10. Referências
---
 * **Template de Documento de Visão - ** [https://www.ibm.com/support/knowledgecenter/pt-br/SSYMRC_6.0.5/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.html](https://www.ibm.com/support/knowledgecenter/pt-br/SSYMRC_6.0.5/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.html)
