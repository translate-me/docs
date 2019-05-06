# Política de Contribuição

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
  | **20/04/2019** | 1.0 | Criação e definição do documento de políticas de contribuição | Luiz Guilherme |

## Política de *Branches*
Para a criação de _branches_ siga os seguintes passos e modelo:

* O nome da _branch_ (NomeDaBranch) deverá ser uma abstração do nome da história de usuário a qual se refere.

* Caso não tenha _tag_.
```
NomeDaBranch
```

* Caso tenha _tag_, ela será o número da _issue_ a qual a se refere a história de usuário.
```
Numero_da_issue-NomeDaBranch
```

* O NomeDaBranch deverá ser escrito seguindo o padrão CamelCase
```
Numero_da_issue-NomeDaBranch
```

### Exemplo prático
* Sem _tag_
```
OurPolicies
```

* Com _tag_
```
Issue_01-CamelCase
```

## Política de *Commits*
Os _commits_ devem seguir o seguinte padrão:

* Deverão descrever sucintamente o que foi feito.
```
Descrição sucinta
```

* Deverão ser escritas no presente do indicativo.
```
Cria um novo documento
```

* A língua do _commit_ deverá seguir como idioma padrão o inglês

* Como o trabalho será codificado em inglês, os _commits_ de código e documentação devem ser escritos em inglês.
```
Creates a new class
```

* Caso tenha alguma _tag_ referente, deverá ser usado o número da _issue_ correspondente.
```
[Issue_01] Create a new class
```

* A _tag_ deverá ser separada por underline, nunca por espaço.

### Exemplo prático

* _Commit_ referente a código ou documento com _tag_
```
[Issue_11] Updates bot answers
```

## Política de *Pull Requests*
Para a criação de um _pull request_ direcionado a branch _master_, deve-se seguir os seguintes passos:

### Status

* Titule o PR com a tag **WIP** (ou seja _work in progress_)

### Descrição
* Utilize o _template_ de _issue_ destinada ao _pull request_.
* Lembrando que o _pull request_ tem a _branch_ base a **_master_** e a _compare_ a branch que se deseja juntar.
* **Lembrando**: assim que for realmente finalizado as alterações referentes ao _pull request_, deve-se retirar a tag **WIP**.

![Imgur](https://i.imgur.com/REsu5YL.png)
 
### _Reviewers_ 

* Assinale os _reviewers_, ou seja, aqueles responsáveis à análise do _pull request_. Por exemplo, caso sua _feature_ esteja relacionada a arquitetura do projeto, assinale o **EPS** que desempenha esse papel.

![](https://user-images.githubusercontent.com/18364727/44523705-31385e00-a6b1-11e8-9e2b-ce3e14702132.png)

### Colaboradores

* Assinale os colaboradores do _pull request_

![](https://user-images.githubusercontent.com/18364727/44523721-52994a00-a6b1-11e8-9a58-34471d984b12.png)

### _Labels_

* Marque as _labels_ relacionadas ao _pull request_. Geralmente será as mesmas assinaladas na issue referente.

![](https://user-images.githubusercontent.com/18364727/44523775-7ceb0780-a6b1-11e8-8388-ced20930782b.png)

### _Milestone_

* Marque a _Milestone_, ou seja, a _sprint_ ou _release_ atual.

![](https://user-images.githubusercontent.com/18364727/44523797-98eea900-a6b1-11e8-8bc9-f9d6ba3c5d9f.png)

### _Issue_ relacionada

* Conecte a _issue_ trabalhada neste _pull request_ 

![](https://raw.githubusercontent.com/RomeuCarvalhoAntunes/2018.1-Reabilitacao-Motora/master/docs/imagens/Tutoriais/Tutorial_PullRequest_08.png)