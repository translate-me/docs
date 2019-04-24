# Banco de Dados

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
|24/04/2019| 0.1 | Transcrição do Modelo Entidade Relacionamento efetivado no drive do grupo | Alexandre Miguel |

## Modelo Entidade - Relacionamento (ME-R)

  Dada a arquitetura do projeto, modularizada por microsserviços, as entidades se referem ao que será requerido e utilizado em cada módulo

### Entidades e Atributos

#### Certificação

* CERTIFICACAO (<span style="text-decoration:underline">idCertificacao</span> , idioma, escola, tipoCertificacao)

#### Autenticação

* AUTOR (<span style="text-decoration:underline">idAutor</span> , cpf, nome, apelido, email, senha)

* TRADUTOR (<span style="text-decoration:underline">idAutor</span>, <span style="text-decoration:underline">idTradutor</span> , cpf, nome, apelido, email, senha, nivel, {lingua})

#### Tradução

* TEXTO (<span style="text-decoration:underline">idTexto</span> , contexto, linguaOrigem , linguaDestino)

* FRAGMENTO (<span style="text-decoration:underline">idFragmento</span> , contexto, linguaOrigem , linguaDestino, conteudo, valor)


#### Chat

* CHAT (<span style="text-decoration:underline">idChat</span> , apelidoTradutor, apelidoAutor)

* FRAGMENTO (<span style="text-decoration:underline">idMessage</span> , conteudo, data)


### Relacionamentos

* **TRADUTOR -** ***detem*** **- CERTIFICACAO**  
Um tradutor detêm nenhuma ou várias certificações, mas cada certificação é detida somente por um tradutor.  
Cardinalidade: **1:n**

* **AUTOR -** ***participa*** **- CHAT**   
Um autor participa de nenhum ou de vários chats, mas cada chat possui um único autor.  
Cardinalidade: **1:n**

* **AUTOR -** ***escreve*** **- CHAT**    
Um autor escreve nenhuma ou várias mensagens, mas cada mensagem é escrita por somente um autor.
Cardinalidade: **1:n**

* **TRADUTOR -** ***traduz*** **- FRAGMENTO**    
Um tradutor pode traduzir nenhum ou vários fragmentos, mas cada fragmento é traduzido por somente um tradutor.
Cardinalidade: **1:n**

* **TEXTO -** ***contem*** **- FRAGMENTO**    
Um texto contém um ou vários fragmentos, e cada fragmento está contido em um único texto.
Cardinalidade: **1:n**

* **AUTOR -** ***possui*** **- TEXTO**    
Um autor possui nenhum ou vários textos, mas cada texto é possuído por um único autor.
Cardinalidade: **1:n**

## Diagrama Entidade - Relacionamento (DE-R)

![translateme_der](assets/banco_de_dados/translateme_der.png)

## Diagrama Lógico
