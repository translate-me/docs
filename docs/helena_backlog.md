# Introspecção

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
