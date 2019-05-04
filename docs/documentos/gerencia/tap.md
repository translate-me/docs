# TAP - *Termo de Abertura do Projeto*

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
| 02/05/2019 | 0.1 | Criação do Template do Documento | Alexandre Miguel |
| 02/05/2019 | 0.2 | Preenchimento dos Tópicos 1 a 6  | Alexandre Miguel |
| 03/05/2019 | 0.3 | Preenchimento dos Tópicos 9, 9.1, 10 e 11 | Alexandre Miguel |
| 04/05/2019 | 0.4 | Preenchimento dos Tópicos 7, 8,  9.2, 9.3, 10 e revisão | Alexandre Miguel |


## 1. Introdução

O Objetivo desse documento é apresentar o projeto **Translate.me**, abordando informações com o objetivo geral do projeto, requisitos de alto nível, riscos no desenvolvimento e uma análise dos recursos empregados.

## 2. Descrição do Projeto

O Projeto **Translate.me** objetiva o desenvolvimento de uma aplicação web que permita a conexão entre integrantes da comunidade acadêmica que desejem traduzir textos e tradutores com experiência na língua de destino para realizar essa tradução, utilizando para isso abordagens de desenho e arquitetura de software, como modelagem utilizando a notação UML e a aplicação de padrões de projetos _GoFs_ e _Grasps_.

## 3. Finalidade do Projeto

Através do desenvolvimento da aplicação, objetiva-se conectar a comunidade tradutora, ou cujos conhecimentos de duas línguas permitam o desempenho de traduções, com a comunidade acadêmica que possui a intencionalidade de enviar artigos ou documentos para instituições internacionais e que necessita de uma tradução rigorosa para tal, utilizando princípios do anonimato entre esses dois tipos de usuário, visando maior segurança quanto ao conteúdo do texto e dos envolvidos.

## 4. Objetivos Mensuráveis do Projeto e Critários de Sucesso Relacionados

São descritos, na seguinte tabela, os objetivos a serem alcançados pelo projeto e os critérios de sucesso que simbolizam o alcance desse objetivo.

| Objetivo | Criétrios de Sucesso |
| --- | --- |
| **Estabelecer Conexão de Serviços entre Tradutores e Autores** | - Envio, pelo autor, de textos a serem traduzidos <br> - Recepção, pelo usuário, de textos traduzidos <br> - Chat anônimo entre tradutor e autor para solução de dúvidas |
| **Garantir Segurança das Informações do Texto Traduzido** | - Sistema de fragmentação de textos <br> - Métricas de confiabilidade expostas ao usuário <br> - Termos de uso explicativos e restritivos |
| **Implementar Sistema Gamificado** | - Sistema de pontuação para tradutores <br> - Punições e recompensas de acordo com as ações dos usuários na plataforma  |

## 5. Requisitos de Alto Nível

O **Translate.me** será uma aplicação web para viabilizar o contato entre usuários que desejam traduzir textos e usuários tradutores, viabilizando a quantia estipulada por tradução e as técnicas de sigilo de informações, seguindo os seguintes requisitos de alto nível:

* O Design da aplicação deverá passar confiabilidade e segurança para os usuários;
* A Aplicação deve ser intuitiva, sem que o usuário precise consultar material adicional para viabilizar seu uso;
* Deverá haver sigilo quanto à identidade tradutores e autores, para preservar informações;
* A Aplicação deverá seguir uma implementação Gamificada, com rankings, pontuações e reflexo das atividades dos usuários em pontos;
* A Aplicação deverá permitir que o usuário escolha diferentes formas de categorizar e fragmentar textos traduzidos;

## 6. Riscos do Projeto

Sob esse tópico estão elencados os principais riscos do Translate.me e as ações preventivas para os devidos riscos.

| Risco | Plano de Ação |
| --- | --- |
| **Dificuldade de integração da equipe para reuniões e alinhamentos.** | Identificação de horários comuns e reuniões em finais de semana. |
| **Problemas de ambientação para desenvolvimento.** | Disponibilização de ambiente de desenvolvimento por meio de imagens e ferramenta Docker. |
| **Membros do grupo estarem fazendo outras disciplinas e atividades complementares, gerando falta de compromentimento.** | Identificação do compromentimento dos membros com medidas punitivas e flexibilização da quantidade de demandas para esses membros, de forma que não atrapalhe o andamento do projeto. |


## 7. Resumo do Cronograma de Marcos

O Projeto possui 8 marcos ao longo do desenvolvimento, demarcados pela progressão da disciplina ao qual está vinculado (_203882 - Arquitetura e Desenho de Software_) para o primeiro semestre letivo de 2019. Sendo assim, a seguinta tabela apresenta essas datas bem como o que representam para o projeto. Durante o período entre esses eventos, as atividades desempenhadas seguirão o planejamento explicitado pelo modelos na [Metodologia do Grupo](../../../metodologia).

| Data | Evento | Descrição |
| --- | --- | --- |
| 25/03/2019 | Seminário 1 | Exposição de artefatos da metodologia utilizada no desenvolvimento do projeto |
| 05/04/2019 | Seminário 2 | Exposição da [Metodologia](../../../metodologia) estruturada para o projeto |
| 15/04/2019 | Seminário 3 | Exposição de [Modelagens Estáticas de UML](../../../desenho_de_software/uml/uml_estaticos) para compreensão e planejamento da estrutura do projeto |
| 29/04/2019 | Seminário 4 | Exposição de [Modelagens Dinâmicas de UML](../../../desenho_de_software/uml/uml_dinamicos) para compreensão e planejamento da estrutura do projeto |
| 24/05/2019 | Seminário 5 a | Apresentação das Modelagens e Implementações dos Padrões [GRASPs](../../../desenho_de_software/padroes/grasp) e [GoFs](../../../desenho_de_software/padroes/gof) na estrutura de codificação do projeto |
| 27/05/2019 | Seminário 5 b | Apresentação dos Padrões de Projeto Emergentes Utilizados |
| 24/06/2019 | Seminário 6 | Exposição da Modelagem e [Documento de Arquitetura de Software](../../projeto/doc_de_arquitetura) |
| 01/07/2019 | Seminário 7 | Exposição do Projeto Completo |

## 8. Lista das Partes Interessadas

Sob um ponto de vista generalista, levando em conta os tipos de acessos da plataforma, as seguintes entidades são tidas como partes interessadas do Projeto:

* ***Tradutores*** - Usuários cujo interesse é em encontrar textos para traduzir por uma quantia justa e de forma facilitada;
* ***Autores*** - Membros da comunidade acadêmica cujos textos elaborados precisam ser traduzidos e cujo conteúdo do texto deve ser mantido ou não em sigilo;

No aspecto de desenvolvimento, idealização e gerência, a equipe composta pelos membros integrantes do projeto também configura partes interessadas do projeto, sendo:

* Alexandre Miguel   
* Davi Alves  
* Gabriela Guedes  
* Helena Goulart  
* João Robson  
* Letícia Meneses  
* Luiz Guilherme  
* Renan Schadt  
* Rômulo Vinícius  
* Victor Hugo  

## 9. Resumo dos Recursos Financeiros

Esse tópico compreende a expectativa de gastos para o projeto, de acordo com o levantamento de recursos já utilizados, bem como recursos que serão destinados ao desenvolvimento.

### 9.1. Recursos Humanos

Tendo a análise mercadológica de estágios no curso de Engenharia de Software, desempenhados por membros o grupo ou identificáveis conforme o contexto de ofertas de estágio (_analisado em Maio de 2019_) identifica-se que, em média, estágios de 20 horas semanas configuram um salário médio de R$1.200,00 o que gera uma estimativa de custo-hora de R$15,00/hora, têm-se ainda que espera-se um desempenho de trabalho de 8 a 12 horas semanais com a disciplina, permitindo assumir o total de 10 horas semanais. Levando em conta que o desempenho das atividades do semestre letivo levam 17 semanas para se totalizarem, é possível organizar a seguinte tabela, informando o custo geral.

| Integrantes | Horas Trabalhadas por semana | Número de Semanas | Custo por Hora | Total de Horas Trabalhadas | Custo Total |
| --- | --- | --- | --- | --- | --- |
| 1 | 10 Horas | 17 | R$15,00 | 170 Horas | R$2.550,00 |
| 10 | 100 Horas | 17 | R$15,00 | 1700 Horas | R$25.500,00 |

Assim, o gasto total esperado para recursos humanos é de R$25.500,OO. O Mesmo paradigma analítico foi planejado para os gastos com alunos pela Universidade de Brasília em 2018, mas a carência de dados explicitados tornou a análise inviável.

### 9.2. Recursos Físicos e Serviços

Para cada um dos 10 integrantes do projeto fez-se necessário o uso de um computador pessoal, ou _notebook_ cujo custo individual para o desempenho das atividades necessárias é, em média R$4.000,00. Além disso, levando em conta que as 170 horas esperadas pelo desempenho do projeto envolvem uso de energia elétrica e de internet, os seguintes dados compõe uma tabela de gastos geral dos recursos físicos do projeto.

| Item | Custo por Unidade | Quantidade | Total |
| --- | --- | --- | --- |
| _Notebook_ | R$ 4.000,00 | 10 | R$ 40.000,00 |
| Energia Elétrica | 0,557 R$/kWh | - 65 watts por carregador _Notebook_ <br>- 10 _Notebooks_ <br>- 170 horas em carga para cada _Notebook_ <br> - 110.500 Watts | R$ 61,55 |
| Internet<br> | R$124,99 ao mês | 4 meses | R$ 499,96 |

Assim, o Gasto total para recursos físicos compõe R$ 40.561,51 para o projeto.

### 9.3. Custo total

Análise dos custos gerais conforme os tipos de recursos empregados no desenvolvimento do projeto.

| Tipo de Recurso | Subtotal |
| --- | --- |
| Humano | R$ 25.500,00 |
| Físico e Serviços  | R$ 40.561,51  |
| **Total** | R$ 66.061,51 |

## 10. Critérios Para Término do Projeto

Para a finalização do projeto e seu encerramento, é necessário que as etapas referenciadas no [Resumo de Cronograma e Marcos](#7-resumo-do-cronograma-de-marcos) sejam alcançadas com sucesso, além dos [Objetivos Mensuráveis do Projeto](#4-objetivos-mensuraveis-do-projeto-e-critarios-de-sucesso-relacionados) do projeto estarem satisfeitos e entregues conforme os [Requisitos de Alto Nível](#5-requisitos-de-alto-nivel). Pelo modelo de desenvolvimento definido na [Metodologia do Projeto](../../../metodologia), para cada etapa referenciada como _Sprint_ existe também um replanejamento que permite a flexibilização de critérios mais pontuais para o término das etapas e para a entrega geral, não se distanciando do definido como os [Objetivos Mensuráveis do Projeto](#4-objetivos-mensuraveis-do-projeto-e-critarios-de-sucesso-relacionados). Assim, o prazo final do cronograma, identificado como apresentação do projeto, é estipulado como marcador principal para a finalização das atividades, que podem ser continuadas mediante replanejamento da equipe e iniciativa externa às atividades da disciplina a qual está vinculada.

## 11. Integrantes do Projeto

Os seguintes membros são integrantes do projeto, cujo desempenho de atividades possui caráter variável, conforme definido na [Metodologia do Projeto](../../../metodologia) utilizando elementos do Scrum com papéis rotativos. Assim, a gerência foi desempenhada ora por membros, ora por grupos, conforme a necessidade da etapa do projeto, o que pode ser observado através das documentações em  [Reuniões](../../../reunioes/sprints/sprint_0).

* Alexandre Miguel   
* Davi Alves  
* Gabriela Guedes  
* Helena Goulart  
* João Robson  
* Letícia Meneses  
* Luiz Guilherme  
* Renan Schadt  
* Rômulo Vinícius  
* Victor Hugo  

## 12. Referências

 - [Informações Sobre Termo de Abertura do Projeto](https://robsoncamargo.com.br/blog/Termo-de-abertura-de-projeto-saiba-tudo-sobre-ele)

 - [Exemplo Prático do Termo de Abertura do Projeto](https://sitecampus.com.br/documentos-de-projetos-termo-de-abertura-do-projeto-exemplo-pratico/)

 - [Template da Documentação](http://www.easybok.com.br/downloads/tap-termo-de-abertura-do-projeto-6-ed/)

 - [Guia PMBoK](https://www.devmedia.com.br/guia-pmbok-gerenciamento-da-integracao/29154)

 - [Documento de Gestão Universidade de Brasília](http://www.dpo.unb.br/images/phocadownload/documentosdegestao/relatoriogestao/2018/Relatrio_de_Gesto_UnB_2018.pdf)

 - [Anuário Estatístico da Universidade de Brasília - 2018](http://www.dpo.unb.br/images/phocadownload/unbemnumeros/anuarioestatistico/Anurio_Estatstico_2018.pdf)

 - [Calendário por Atividades da Universidade de Brasília](http://www.saa.unb.br/images/stories/documentos/calendarios/graduacao/cal_atividades/cal_at_2019_1.pdf)

- [Ranking de Tarifas de Energia Elétrica](http://www.aneel.gov.br/ranking-das-tarifas)

- [Consumo de Energia de Aparelhos Utilizados](https://20somethingfinance.com/how-much-electricity-costs-appliances-and-how-to-cut-your-usage/)

- [Preço de Internet](https://www.assinenet.com.br/NET_NetVirtua_BandaLarga_30mega.html)
