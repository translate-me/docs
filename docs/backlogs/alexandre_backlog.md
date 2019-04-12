# Backlog Individual

|  Autor | Data |
| --- | --- |
| Alexandre Miguel | 06/04/2019 |

## Introdução  

Para a montagem do backlog ao final do arquivo, foi realizada uma introspecção ao imaginar diferentes fluxos de usuários na plataforma, baseado nas definições realizadas após o [Brainstorming](#) realizado em reunião anterior. O formato tomado nas introspecções foi realizado como storytelling tendo como olhar os diferentes tipos de usuários da aplicação.

## Introspecção 1

Usuário chamado João precisa traduzir artigo a ser publicado em seu TCC, ao pedir recomendações de formas de fazer isso de forma efetiva, fica sabendo do aplicativo "translate.me" e acessa aplicação. Ao realizar seu cadastro, decide se utiliza um sistema nativo ou se cadastra-se com o google ou facebook, optando pelo cadastro com o facebook. O usuário então decide que será um usuário autor, para postar textos e assim cadastra seu cartão de crédito para realizar o pagamento do serviço prestado. Ao acessar a página de inserção de textos, o usuário deve escolher entre os métodos de inserção do arquivo, como um txt, um ODT ou um Input próprio, optando assim por um txt. Em seguida, João utiliza do sistema de separação do texto em módulos para tradução, evitando que o trabalho inteiro esteja exposto a um único tradutor. Para auxiliar a tradução, João adiciona um resumo do conteúdo do TCC, estabelece palavras que devem ter traduções fixas e adiciona uma tag para identificação do conteúdo e da complexidadade linguística do tópico. Durante o período de tradução, João acompanha o progresso através de porcentagens de avanço e, ao final do período estipulado, João recebe o documento inteiramente traduzido em um formato de saída genérico, em .txt. Caso perceba alguma incoerência, João notifica a falta de correção, podendo enviar uma dúvida sobre algum aspecto. Após qualquer ajuste, João atribui uma nota para a correção e acumula pontos de uso.

### Requisitos Elicitados

|  Requisito | ID |
| :---: | :---: |
|  A Aplicação deve possuir um sistema de cadastro | IA1.01 |
|  A Aplicação deve permitir o cadastro pelo facebook | IA1.02 |
|  A Aplicação deve permitir o cadastro pela conta do google | IA1.03 |
|  A aplicação deve permitir a diferenciação entre usuários tradutores e usuários autores | IA1.04 |
|  Os usuários que desejam ter textos traduzidos devem ser referidos como "Autores" | IA1.05 |
|  Os usuários que traduzem textos devem ser referidos como "Tradutores" | IA1.06 |
|  A aplicação deve possuir um sistema de Carteira Virtual para transferência de créditos como pagamento por serviço | IA1.07 |
|  A Aplicação deve possuir uma funcionalidade de inserção de texto pelo usuário autor a ser traduzido pelo usuário tradutor | IA1.08 |
|  A Aplicação deve possuir diferentes formas de inserção de texto a critério do usuário autor | IA1.09 |
|  A aplicação deve possuir um sistema de separação do texto em fragmentos para correção  | IA1.10 |
|  A aplicação deve possuir um sistema de envio sem repetição de fragmentos para usuários corretores | IA1.11 |
|  A aplicação deve notificar o usuário da não responsabilização por direitos autorais | IA1.12 |
|  A aplicação deve medir a segurança do texto de acordo com a quantidade de fragmentos | IA1.13 |
|  A aplicação deve informar ao usuário um prazo para a entrega da correção conforme a quantidade e tamanho dos fragmentos  | IA1.14 |
|  Os fragmentos de texto devem possuir resumos elaborados pelo autor para contextualização do tradutor | IA1.15 |
|  A aplicação deve possuir uma página de acompanhamento de correções para o usuário autor | IA1.16 |
|  A aplicação deve notificar o usuário autor de que seu texto foi totalmente traduzido | IA1.17 |
|  Os fragmentos de texto devem possuir tags que indiquem o tema e a complexidade do texto geral | IA1.18 |
|  A Aplicação deve estabelecer um contato em anonimato entre usuário tradutor e usuário autor para solução de dúvidas | IA1.19 |


## Introspecção 2

Uma usuária chamada Ana, que deseja traduzir textos para complementar seus ganhos como professora de Inglês, decide se cadastrar na plataforma por ouvir indicações de seu uso. Ao realizar o cadastro pela conta do google, ela opta pela opção de usuária tradutora, enviando seu certificado de graduação na língua. Após o cadastro, Ana recebe um fragmento de texto para traduzir, com informações do prazo de entrega da tradução, e aceita corrigi-lo. Após algumas correções, o aplicativo solicita que Ana revise algumas correções antes de prosseguir com as correções, informando que correções superficiais serão identificadas posteriormente e o usuário será penalizado. Ana acessa o site com frequência e quando encontra uma revisão que precisa de modificações, realliza as modificações, notificando o usuário corretor acerca do e recebe pontuações.

### Requisitos Elicitados

|  A Aplicação deve possuir sistema de verificação de proeficiência dos falantes da língua | IA2.01 |
| :---: | :---: |
|  Os fragmentos devem ser enviados para os usuários tradutores com prazo estabelecido | IA2.02 |
|  A Aplicação deve possuir uma página para seleção dos fragmentos a serem traduzidos | IA2.03 |
|  A Aplicação possuir sistema de revisão por usuários de fragmentos traduzidos | IA2.04 |
|  [Não Funcional] A Aplicação deve enviar mensagens explicativas sobre dúvidas que possam surgir para o usuário, como a explicação do motivo das correções | IA2.05 |
|  A Aplicação deve possuir um sistema de pontuação para usuários tradutores | IA2.06 |
|  [Não Funcional] O Sistema de pontuação deve influenciar nas ações dos usuários tradutores da plataforma | IA2.07 |
|  O Usuário tradutor deve possuir badges ou selos que identifiquem seu nível de proeficiência na língua | IA2.08 |
|  O Sistema de pontuação deve ser utilizado para priorizar a disponibilização de fragmentos para tradução | IA2.09 |
|  A Aplicação deve limitar novas correções por revisões de correções de outros usuários | IA2.10 |
|  O Usuário Tradutor deve poder fazer correções nas traduções em que atua como revisor | IA2.11 |
|  A Aplicação deve possuir um sistema de Login próprio | IA2.12 |
|  A Aplicação deve possuir um sistema de Login com facebook | IA2.13 |
|  A Aplicação deve possuir um sistema de Login com Google | IA2.14 |

## Backlog Final

|  Código | Épico | Eu, como... | Gostaria de... | Para poder... | Priorização | Requisito Associado |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  USA01 | Cadastro | Usuário | Me cadastrar na aplicação | Ter acesso às funcionalidades do translate.me | Must | IA1.01 |
|  USA02 | Cadastro | Usuário | Me cadastrar através do Facebook | Ter acesso às funcionalidades de forma prática e integrada | Should | IA1.02 |
|  USA03 | Cadastro | Usuário | Me cadastrar através do Google | Ter acesso às funcionalidades de forma prática e integrada | Should | IA1.03 |
|  USA04 | Cadastro | Usuário | Escolher qual será minha atuação na plataforma | Acessar ferramentas condizentes com o tipo de utilização que pretendo ter da plataforma | Must | IA1.04, IA1.05, IA1.06 |
|  USA05 | Cadastro | Desenvolvedor | Atribuir termos aos tipos de usuário da aplicação | Diferenciar entre usuários que traduzem textos e usuários autores de textos | Must | IA1.04, IA1.05, IA1.06 |
|  USA06 | Cadastro | Usuário Tradutor | Submeter documento que comprove meu conhecimento em alguma língua  | Garantir minha colocação correta perante a aplicação | Must | IA2.01 |
|  USA07 | Tradução | Desenvolvedor | Aplicar diferentes formas de inserção de textos na aplicação | Dar ao usuário escolhas de inserção se adaptem a suas necessidades | Should | IA1.08 |
|  USA08 | Tradução | Usuário Autor | Inserir meu texto na aplicação | Permitir que a tradução seja realizada em cima do texto pretendido | Must | IA1.07 |
|  USA09 | Tradução | Usuário Autor | Adicionar informações acerta do texto submetido | Direcionar o tipo de tradução esperado  | Must | IA1.15, IA1.18 |
|  USA10 | Tradução | Usuário Tradutor | Visualizar fragmentos disponíveis para tradução | Escolher qual fragmento gostaria de traduzir conforme meus conhecimentos e habilidades | Must | IA2.03 |
|  USA11 | Tradução | Desenvolvedor | Limitar a quantidade de correções pelas revisões realizadas | Garantir que os textos corrigidos sejam revisados | Must | IA1.08 |
|  USA12 | Gamificação | Desenvolvedor | Implementar sistema de pontuação para usuários tradutores | Incentivar o fluxo de tradução e revisão dos fragmentos com qualidade | Must | IA2.04, IA2.06, IA2.08, IA2.09, IA2.10 |
|  USA13 | Gamificação | Usuário Tradutor | Realizar modificações em um texto traduzido | Corrigir o texto conforme a linguagem demanda | Should | IA2.12 |
|  USA14 | Login | Usuário | Realizar o login na aplicação | Acessar os recursos da aplicação | Must | IA2.12 |
|  USA15 | Login | Usuário | Realizar o login na aplicação pelo Facebook | Acessar os recursos da aplicação com integração à conta do facebook | Should | IA2.13 |
|  USA16 | Login | Usuário | Realizar o login na aplicação pelo Google | Acessar os recursos da aplicação com integração à conta do Google | Should | IA2.14 |
|  USA17 | Pagamento | Desenvolvedor | Acoplar sistema de carteira virtual à aplicação | Permitir que os usuários realizem transferências seguras de crédito | Would | IA1.06 |
