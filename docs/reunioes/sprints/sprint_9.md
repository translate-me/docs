# Sprint 7

## Histórico de Revisão

  | Data | Versão | Descrição | Autor |
  |---|---|---|---|
  | 27/05/2019 | 1.0 | Transcrição do planejamento da sprint | Alexandre Miguel |


## Registro

| Data da Reunião | Participantes | Meio | Local |
| :---: | :---: | :---: | :---: |
| 27/05/2019 | Alexandre Miguel <br> Rômulo Souza <br> Davi Alves <br> Gabriela Guedes <br> Helena Goulart <br> Letícia Meneses <br> Renan Schadt <br> Luiz Guilherme | Hangouts | - |


## Introdução

A Reunião teve o viés de resolver demandas existentes para a implentação em código do projeto, bem como de refletir acerca das considerações da dinâmica recente (Seminário de Padrões Emergentes).

### Novos Papéis

A troca de papéis foi definida conforme a seguinte tabela:

| Papel | Sprint 7 |
|:---: | :---: |
| Scrum Master | Alexandre Miguel |
| Product Owner ( *PO* ) | Rômulo Souza |
| Arquiteto | Victor Hugo |

### Planejamento da Sprint

O Planejamento seguiu os seguintes tópicos, sendo discutidos pelos membros participantes para consenso geral.

#### Semana Sem Pareamentos

Tema foi apresentado como uma forma de otimizar o volume de produtos de software gerado, finalizando uma etapa de nivelamento de conhecimentos para priorizar o desenvolvimento do projeto.


#### Issues de Código

Issues da semana foram decididas como voltadas para código, de Frontend e Backend, para posterior desenvolvimento do produto nos padrões determinados.

#### GoFs

Finalização de issues de documentação de modelos de GoFs, dado que várias issues se tornaram dívidas técnicas e devem ser resolvidas ainda nessa sprint.

#### Refatoração do Backend

Para garantir a unicidade do código e compreensão do desenvolvimento por pessoas externas ao projeto, foi determinado que o serviço de tradução seria refatorado  pelo integrante Victor Hugo para conformidade com os serviços de perfil e autenticação. Assim, o foco maior do desenvolvimento será para adiantamento do desenvolvimento do Frontend, enquanto o desenvolvimento de Backend será reduzido durante o período de refatoração.

#### Tabela de Atuação da Sprint

Dado o contexto de refatoração, a atuação de cada integrante da equipe no desenvolimento durante a sprint seguirá a seguinte tabela:

| Integrante | Área de Atuação | Tecnologia |
| :---: | :---: | :---: |
| Gabriela Guedes | Frontend | React |
| Davi Alves | Frontend | React |
| Helena Goulart | Frontend | React |
| Renan Schadt | Frontend | React |
| Luiz Guilherme | Frontend | React |
| João Robson | Backend / Frontend | Django / React |
| Victor Hugo | Backend | Django |
| Rômulo Souza | Backend | Django |
| Letícia Meneses | Backend | Django |
| Alexandre Miguel | Backend | Django |

#### Issues e Responsáveis

| Issue | Contexto | Integrante Responsável |
| :--- | :---: | :---: |
| US61 - Acessar Página de Perfil | Frontend | Davi Alves |
| US35 - Tela Inicial do Tradutor | Frontend | |
| US40 - Revisar Tradução | Frontend | |
| US31 - Finalizar Tradução | Frontend | Helena Goulart |
| US08 - Adicionar Informações Para Submeter Texto | Frontend | |
| US18 - Acompanhar Estado da Tradução | Frontend | J |
| US10 - Adicionar Breakpoints | Frontend | Luiz Guilherme |
| US23 - Implementar Registros de Revisão | Backend | Rômulo Souza |
| US06 - Submeter Certificado de Língua | Backend | Letícia Meneses |
| US62 - Implementar Fluxo de Notificação | Backend | Alexandre Miguel |
| Refatoração do Serviço de Tradução | Backend | Victor Hugo |

## Review

### O que cada um fez

#### Luiz

- Fez a issue, mas faltou resolver o bug e retirar o breakpoint
- Pegou issue da Helena para fazer e não terminou

#### Victor

- Refatorou o Translate-me

#### Rômulo

- Implementou o composite e filter na nova refatoração

#### Renan

- Fez a história e faltou umas coisas

#### Gabi

- Terminou a história e deu PR

#### Davi

- Finalizando issue e faltando imagem do usuário

#### Helena

- Padronizou o front
- Resolveu dívidas técnicas

#### Alexandre

- GoF
- Finalizando issue hoje

### Pontos Positivos

- Distribuição de Issues Individuais
- Dupla Scrum e PO
- Fim dos Pareamentos
- Flexibilização de Entregas
- Pareamento de Sábado
- Diminuição de Débitos Técnicos
- Alinhamento de Visão (Back e Front)


### Pontos Negativos

- Identidade Visual Não Sendo Seguido
- Frontend Aceitando PR do Backend
- Dialogar melhor resoluções do projeto


### Como Melhorar

- Setorizar Avaliação de PRs
