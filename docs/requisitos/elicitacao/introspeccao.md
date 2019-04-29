# Introspecção

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
| 06/04/2019 | 0.1 | Adição das Introspecções 1 a 7  | Helena Goulart |
| 06/04/2019 | 0.2 | Adição das Introspecção 8 e 9  | Letícia Meneses |
| 06/04/2019 | 0.3 | Adição da Introspecção 10 e 11 | Alexandre Miguel |
| 27/04/2019 | 0.4 | Criação do documento | Alexandre Miguel |

## Introdução  

Para a montagem do backlog ao final do arquivo, foi realizada uma introspecção ao imaginar diferentes fluxos de usuários na plataforma, baseado nas definições realizadas após o [Brainstorming](../brainstorming) realizado em reunião anterior. O formato tomado nas introspecções foi realizado como storytelling tendo como olhar os diferentes tipos de usuários da aplicação.

## Definição

A técnica de introspecção consiste em imaginar que tipo de sistema seria desejável por uma pessoa que estivesse executando uma tarefa específica, utilizando um equipamento específico, em um lugar específico, dentre outros. Se dá ao imaginar que características um sistema deveria ter para obter a satisfação do usuário definido.

## Introspecção 1

#### Rastreabilidade

| Nome | Papel | Observação |
|--|--|--|
| Helena Goulart | Usuária do Web App | Membro da equipe |

#### Contexto
Trata-se de uma estudante chamada Bianca, que encontra-se no mestrado em
Engenharia de Energia e que teve dificuldades na tradução de artigos que desejou
publicar durante o período da graduação. Desse modo, Bianca possui uma grande
trava com línguas estrangeiras e tradução de textos técnicos. Foi assim que
teve a ideia de pesquisar no Google ferramentas de tradução, que não fossem o
translate da propria ferramenta, e descobriru o web app Translate.me. Bianca
sentiu-se receosa em submeter seu artigo em um site desconhecido para tradução,
porém como o trauma vivido até então era maior que o medo com os direitos
autorais, resolveu arriscar. Em primeiro lugar, abriu o site e leu a descrição
de como funcionava a ferramenta. Interessada em conhecer mais, criou uma conta
no site, clicando na aba _"Inscreva-se"_ e efetivando seu _login_ através do
_Facebook_. O Translate.me enviou um e-mail de confirmação de conta, e a usuária
conseguiu confirmar com apenas um clique. Após a confirmação, encontrou um
tutorial de como funcionava a página. Ao finalizar o tutorial, a usuária optou
por fazer a sua primeira submissão.

#### Necessidades Técnicas
* Um site que transmita segurança em relação aos direitos autorais;
* Um site que transmita segurança em relação à qualidade da tradução.

#### Necessidades Sociais
* Poder contar com algo ou alguém que possa ajudar no processo de tradução
do artigo.

#### Necessidades Individuais
* Superação de um trauma em relação à tradução de artigos científicos;
* Um artigo com tradução de qualidade a ser subemtido em uma revista.

#### Requisitos Elicitados

| Código | Descrição | Prioridade | Classificação |
|--|--|--|--|
| INT1.1 | O site deve conter uma página inicial explicando o que é o site e como ele funciona | Must | Não Funcional |
| INT1.2 | O site deve conter uma página para explicar as diretrizes de segurança de direitos autorais | Must | Não Funcional |
| INT1.3 | O site deve apresentar a opção de inscrever-se através de nome de usuário e senha | Must | Funcional |
| INT1.4 | O site deve conter a opção de inscrever-se com facebook ou gmail | Should | Funcional |
| INT1.5 | O site deve conter a opção de realizar o login com nome de usuário e senha | Should | Funcional |
| INT1.6 | O site deve conter a opção de realizar o login com facebook ou gmail | Should | Funcional |
| INT1.7 | O cadastro no site deve ser efetivado através de um e-mail de confirmação, que ativa a conta com apenas um _click_ | Must | Funcional |
| INT1.8 | O usuário cadastrado deve receber um tutorial de uso do site, no qual as principais funcionalidades recebem ênfase e informações detalhadas de como usar | Must | Funcional |
| INT1.9 | O usuário deve ter a opção de submeter o artigo no site | Must | Funcional |

## Introspecção 2

#### Rastreabilidade

| Nome | Papel | Observação |
|--|--|--|
| Helena Goulart | Usuária do Web App | Membro da equipe |

#### Contexto
Ao clicar na opção de submeter o texto traduzido, Bianca conferiu se o tipo do
arquivo era compatível com o exigido pela plataforma, que era um formato PDF.
Este pré-requisito foi atendido e a usuária pode visualizar logo após submeter
o artigo quais eram os trechos que os tradutores teriam acesso. Surgem na tela
então duas opções: aceitar os trechos como estão, ou definir manualmente como os
trechos poderiam ser dividos. Bianca não viu muito sentido em como os trechos
estavam dividos e optou por editar a divisão. Ao concluí-la, o site alertou
se ela tem certeza sobre a edição, e que o site não se responsabiliza pelo excesso
de informação disponibilizada pela própria autora do texto. Ela afirmou se
responsabilizar, afinal havia pressa para que o serviço fosse realizado e não
se atentou muito à segurança dos dados. O site questionou qual o prazo para a
conclusão do serviço, informando as opções de prazo mínimo e máximo que os tradutores
possuem. Bianca, com muita pressa, optou pelo prazo mínimo.

#### Necessidades Técnicas
* Ferramentas que suportem formatos de texto mais comuns para subimissão de artigos;
* Divisão automática do texto em trechos.

#### Necessidades Sociais
* Privacidade dos dados.

#### Necessidades Individuais
* Prazos para conclusão do serviço.

#### Requisitos Elicitados

| Código | Descrição | Prioridade | Classificação |
|--|--|--|--|
| INT2.1 | O site deve suportar formatos de texto mais comuns para subimissão de artigos; | Should | Não Funcional |
| INT2.2 |O site deve dividir o texto do usuário em vários pequenos trechos | Must | Funcional |
| INT2.3 | Um mesmo tradutor não pode ter acesso completo ao texto do usuário | Must | Não Funcional |
| INT2.4 | O usuário deve poder personalizar a divisão de trechos do texto | Must | Funcional |
| INT2.5 | O usuário não poderá disponibilizar o texto completo para o tradutor no processo de personalização da divisão | Must | Funcional |
| INT2.6 | O site deve questionar se o usuário possui certeza da personalização da divisão do texto | Should | Funcional |
| INT2.7 | O site deve disponibiliar prazo mínimo e máximo para a conclusão do serviço | Must | Funcional |
| INT2.8 | O usuário deve poder selecionar uma data limite para receber o texto traduzido de acordo com o período mínimo e máximo disponibilizado pelo site | Must | Funcional


## Introspecção 3


#### Rastreabilidade

| Nome | Papel | Observação |
|--|--|--|
  | Helena Goulart | Tradutora | Membro da equipe |

#### Contexto
Certa vez a estudante de história Fabíola estava interessada em conseguir dinheiro sem necessariamente passar horas em um escritório ou qualquer emprego fixo, uma vez que estava redigindo seu TCC1 na Universidade de Brasília. Fabíola possui alta pontuação no TOEFL e já deu aulas particulares de inglês, e então realizou uma busca no google de _"freelancer inglês"_, deparando-se com o Translate-me. Ao ler a página de informações para freelancers, Fabíola concluiu que atende aos requisitos necessários para ser tradutora no site, dentre eles: ter uma conta em um banco virtual, ter um diploma ou certificado de competência em língua estrangeira, e optou por inscrever-se na plataforma.

#### Necessidades Técnicas
* Informações sobre os pré-requisitos para participar.

#### Necessidades Sociais
* Informações dadas de maneira acessível.

#### Necessidades Individuais
* Ganhar dinheiro como _freelancer_.

#### Requisitos Elicitados

| Código | Descrição | Prioridade | Classificação |
|--|--|--|--|
| INT3.1 | O site deve ter uma página instruindo como o site funciona e quais são os pré-requisitos para _freelancers_ | Must | Não Funcional |
| INT3.2 | O site deve exigir que todos os usuários, tanto tradutores como usuários a terem seu textos traduzidos, tenham contas virtuais | Must | Não Funcional |
| INT3.3 | O site deve exigir dos tradutores uma certificação em língua estrangeira | Should | Não Funcional |

## Introspecção 4


#### Rastreabilidade

| Nome | Papel | Observação |
|--|--|--|
  | Helena Goulart | Tradutora | Membro da equipe |

#### Contexto
Após retirar seu certificado da gaveta, Fabíola anexou uma foto dele no Translate.me logo depois de preencher os dados de login necessários, incluindo e-mail, um nome de usuário e senha. Para atrair mais clientes, Fabíola preencheu seu perfil com informações como: foto de perfil, idade, curso que está graduando, e-mail para contato e uma descrição básica sobre si mesma. Essas informações ficaram localizadas no perfil de Fabíola, e o Translate.me fixou uma informação de seu nível de competência e de qual é a instituição que lhe garantiu certificação em língua estrangeira.

#### Necessidades Técnicas
* O site deve suportar mais de um formato de documento.

#### Necessidades Sociais
* Conter informações de perfil e de contato.

#### Necessidades Individuais
* Submeter a certificação em inglês na plataforma.

#### Requisitos Elicitados

| Código | Descrição | Prioridade | Classificação |
|--|--|--|--|
| INT4.1 | O site deve aceitar formatos de texto comuns para o _upload_ da certificação em língua estrangeira | Must | Não Funcional |
| INT4.2 | O site deve permitir que todos os usuários tenham um perfil | Must | Funcional |
| INT4.3 | O perfil do usuário deve conter foto de perfil | Should | Não Funcional |
| INT4.4 | O perfil do usuário deve expor informações para contato | Must | Não Funcional |
| INT4.5 | O usuário pode incluir informações sobre si mesmo, como uma _bio_ | Must | Funcional |
| INT4.6 | O usuário deve poder editar as informações do seu perfil  | Must | Funcional |
| INT4.7 | O site deve validar a veracidade da certificação em língua estrangeira | Must | Não Funcional |
| INT4.8 | O site deve expor no perfil qual é a certificação do usuário em questão | Must | Não Funcional |

## Introspecção 5

#### Rastreabilidade

| Nome | Papel | Observação |
|--|--|--|
  | Helena Goulart | Tradutora | Membro da equipe |

#### Contexto
Dois dias após realizar o login na plataforma, Fabíola percebeu que não recebeu notificações a respeito de pedidos de traduções, e entrou no Translate.me para ver se havia recebido alguma mensagem. Ao efetuar o _login_, percebeu que havia um _feed_, mostrando os novos pedidos de traduções, e uma lista de categorias à direita. Ao clicar na categoria _Ciências da natureza_, encontrou uma tese de mestrado solicitando tradução. Fabíola ficou bastante surpresa pelas traduções ficarem categorizadas, e aceitou fazer a tradução da tese de mestrado de uma estudante chamada Bianca. Ao clicar em "Quero traduzir esse texto", apareceram alguns trechos para Bianca traduzir.

#### Necessidades Técnicas
* Existência de categorização dos textos a serem traduzidos.

#### Necessidades Sociais
* Existir um _feed_ contendo todas as traduções submetidas recentemente no site.

#### Necessidades Individuais
* Acessibilidade e facilidade em encontrar trabalhos.

#### Requisitos Elicitados

| Código | Descrição | Prioridade | Classificação |
|--|--|--|--|
| INT5.1 | O site deve conter um _feed_ com as traduções submetidas recentemente | Must | Não Funcional |
| INT5.2 | O site deve conter categorias que separem os textos a serem traduzidos de acordo com temas em comum | Must | Não Funcional |
| INT5.3 | O site deve conter uma comunicação de estilo conversativa com o usuário | Should | Não Funcional |
| INT5.4 | O usuário deve poder selecionar a opção de traduzir o texto | Must | Funcional |

## Introspecção 6


#### Rastreabilidade

| Nome | Papel | Observação |
|--|--|--|
  | Helena Goulart | Usuária | Membro da equipe |

#### Contexto
Era uma terça-feira a tarde quando Bianca entrou no Translate.me para acompanhar o processo de tradução de seu artigo. Ao digitar o link e entrar na página, encontrou a opção "Textos em andamento", e viu que havia uma bola vermelha e pequena nessa opção, indicando uma notificação. Ao clicar, apareceu o nome de quatro pessoas que estavam com a tradução em andamento, e Bianca visualizou o perfil de uma por uma, e ficou bastante contente em ver que todos que estavam realizando o trabalho eram bastante competentes para isso. Ao voltar para a página de "Textos em andamento", clicou na opção de "Acompanhar a tradução de Fabíola", e conseguiu ver em tempo real como andava o trabalho da tradutora.

#### Necessidades Técnicas
* Notificar os usuários de que existem atualizações no status de tradução do texto.

#### Necessidades Sociais
* Conhecer quem está traduzindo o texto.

#### Necessidades Individuais
* Acompanhar se o texto submetido está em processo de tradução.

#### Requisitos Elicitados

| Código | Descrição | Prioridade | Classificação |
|--|--|--|--|
| INT6.1 | O site deve notificar quando houver uma atualização no status de alguma atividade do usuário | Must | Não Funcional |
| INT6.2 | O usuário deve poder visualizar o perfil de outros usuários | Must | Funcional |
| INT6.3 | O site deve informar quem são as pessoas que estão traduzindo o texto do usuário | Should | Não Funcional |
| INT6.4 | O usuário deve poder acompanhar as traduções e visualizar como elas estão sendo feitas | Must | Funcional |


## Introspecção 7

#### Rastreabilidade

| Nome | Papel | Observação |
|--|--|--|
  | Helena Goulart | Tradutora | Membro da equipe |

#### Contexto
Assim que clicou para começar a tradução do texto de Bianca, o site Translate.me direcionou Fabíola para uma página informando as diretrizes de segurança, assim como as políticas de privacidade e de segurança de dados. Fabíola clicou na caixa de seleção informando estar ciente de todas as regras e em seguida apertou a opção "Continuar". Então, foi direcionada para a tradução. Nessa página informava o prazo máximo para entrega do serviço, e Fabíola logo começou a realizar o trabalho. Enquanto realizava a tradução, quando escrevia palavras, termos e expressões de maneira incorreta, o _software_ oferecia sugestões de correção, o que facilitou o serviço de tradução. Duas horas depois, o serviço estava concluído.

#### Necessidades Técnicas
* Informar aos usuários a importância da segurança de dados e as diretrizes do site;
* Auxiliar o usuário com as traduções.

#### Necessidades Sociais
* Prazos para entrega da tradução.

#### Necessidades Individuais
* Visualizar o prazo de entrega do serviço.

#### Requisitos Elicitados

| Código | Descrição | Prioridade | Classificação |
|--|--|--|--|
| INT3.1 | O site deve informar a importância das seguranças de dados e as diretrizes do site | Must | Não Funcional |
| INT3.2 | O usuário não poderá começar nenhuma tradução sem antes confirmar que está de acordo com as políticas de privacidade e de segurança de dados do site | Must | Funcional |
| INT3.3 | O site deve informar ao tradutor o prazo para a entrega do serviço | Must | Não Funcional |
| INT3.4 | O site deve conter o apoio do _software_ CAT | Must | Funcional |

## Introspecção 8

#### Rastreabilidade

| Nome | Papel | Observação |
|--|--|--|
| Letícia Meneses | Autora | Membro da equipe/Usuário |

#### Contexto

O contexto dessa introspecção se dá por uma pessoa de ambiente acadêmico que acabou de saber da aplicação Translate.me, e gostaria de visualizar a plataforma sem nenhum compromisso com cadastro. Ela deseja ver os serviços oferecidos pelo app e uma explicação dos mesmos. A pessoa precisa ter acesso a quaisquer documentações que explique sobre o webapp, assim como tutorias, contato e um FAQ.

### Necessidades do Contexto

Este tópico aborda as necessidades obtidas nessa introspecção.

##### Necessidades técnicas
* Suporte para diversos navegadores
* Limitar dados do usuário caso esteja no celular
##### Necessidades individuais
* Uma mostra do app para não cadastrados
* A necessidade de um site intuitivo
* Conseguir ver informações dos serviços oferecidos sem estar cadastrado
#### Requisitos Elicitados

| Código | Descrição |
|--|--|
|INT1.1 | O usuário deve conseguir ver de forma resumida a plataforma
| INT1.2 | Deve aparecer a opção de login/cadastro na tela inicial
| INT1.3 |O site deve mostrar informações básicas e chamativas para despertar o interesse na pessoa
| INT1.4 | O site deve mostrar um menu com opções limitadas para a pessoa que está visualizando sem cadastro
| INT1.5 | O usuário deve ver opções de FAQ, contato e uma explicação sobre o Translate.me
| INT1.6 | A opção de cadastro/login deve estar sempre aparecendo na tela para os não logados
| INT1.7 | Algumas opções do site devem ser restritas a usuários não logados, aparecendo então um pop up de cadastro/login ao ser clicado


## Introspecção 9

| Nome | Papel | Observação |
|--|--|--|
| Letícia Meneses | Autora | Membro da equipe/Usuário |

#### Contexto

Uma pessoa quer utilizar os serviços do translate.me para traduzir seu artigo para alemão, pois seu artigo será publicado em um journal com Qualis alto e muito renomado.

### Necessidades do Contexto

Este tópico aborda as necessidades obtidas nessa introspecção.

##### Necessidades técnicas
* Suporte para vários navegadores
* Servidor precisa estar sempre no ar

##### Necessidades individuais
* Conseguir cadastrar e logar na página
* Ter opções de línguas para traduzir qualquer documento
* Necessidade de prazo para que entregue o produto
* Confiabilidade na exposição dos documentos

#### Requisitos Elicitados

| Código | Descrição |
|--|--|
| INT2.1 | Ao entrar na página, o usuário deve conseguir fazer cadastro ou login na plataforma
| INT2.2 |Durante o cadastro, o usuário deve ver não termos de aceite informações de confiabilidade a exposição do artigo
| INT2.3 | O usuário deve conseguir visualizar e editar suas informações de perfil
| INT2.4 | O usuário deve conseguir colocar/cadastrar seu artigo para que seja traduzido
| INT2.5 | O usuário deve poder escolher qual língua será traduzida seu artigo
| INT2.6 | O usuário deve conseguir dividir seu artigo para que vários tradutores traduzam e desconectar informações
| INT2.7 | O usuário deve conseguir requerer níveis maiores de tradutores para que conduza a tradução do seu artigo
| INT2.8 | O usuário tradutor e o usuário contratante devem conseguir ter contato entre eles
| INT2.9 | O usuário deve conseguir ver informações básicas de seus tradutores
| INT2.10 | O usuário deve conseguir estabelecer um prazo para a entrega da tradução
| INT2.11 | O usuário deve acompanhar o processo de tradução de seu artigo/documento
| INT2.12 | O usuário avaliar o serviço do tradutor, dentro das normas a serem cumpridas


## Introspecção 10

| Nome | Papel | Observação |
|--|--|--|
| Alexandre Miguel | Autor | Usuário que precisa traduzir artigo |

### Contexto

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


## Introspecção 11

| Nome | Papel | Observação |
|--|--|--|
| Alexandre Miguel | Autor | Tradutor frequente |

### Contexto

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
