# Documento de Arquitetura Translate.me

### Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
| 31/03/2019 | 0.1 | Adicionando o Template do documento de arquitetura | Victor |
| 01/04/2019 | 0.2 | Modificando Template para preenchimento | Alexandre Miguel|
| 09/04/2019 | 0.3 | Adicionando Introdução e Requisitos e Restrições arquiteturais | Gabriela Guedes |


### Objetivo do documento
Este documento tem como objetivo descrever e caracterizar as decisões arquiteturais do projeto
translate.me. A caraterização será feita apenas no ambito do software não levando em conta medições
como de performace.

## Sumário
1. [Introdução](#1-introdução)  
	1.1 [Finalidade](#1.1)  
	1.2 [Escopo](#1.2)  
	1.3 [Definições, Acrônimos e Abreviações](#1.3)  
	1.4 [Referências](#1.4)  
2. [Representação arquitetural](#2)
3. [Requisitos e Restrições arquiteturais](#3-requisitos-e-restrições-arquiteturais)
4. [Visão Lógica](#4.)  
	4.1 [Visão geral de camadas e pacotes ](#4.1)  
5. [Visão de implementação](#5)  
	5.1 [Diagrama de classes](#5.1)
6. [Visão de implementação](#6)
7. [Dimensionamento](#7)
8. [Qualidade](#8)


### 1. Introdução

Este documento visa apresentar a arquitetura de software a ser aplicada no sistema do Translate.me, de forma que facilite a visualização dos requisitos e da estrutura para os envolvidos. 

#### 1.1. Finalidade
---
#### 1.2. Escopo
---
#### 1.3. Definições, Acrônimos e Abreviações
---
#### 1.4. Referências
[Lino](https://botlino.github.io/docs/doc-arquitetura)
---
### 2. Representação arquitetural
![arquitetura](https://i.ibb.co/zf99Pb7/architecture.png)
---
### 3. Requisitos e Restrições arquiteturais

|Requisito|Solução|
|---|---|
|Linguagem|O front-end será feito em *JavaScript* e o back-end, em *Python*|
|Plataforma|Serão usadas as plataformas *ReactJS* para o front-end e *Django* para o back-end|
|Segurança| É necessário uma segurança para com os dados, pois todos os usuários irão interagir de forma anônima. Para uma maior segurança das informações, será necessário a utilização de token nas requisições|
|Persistência|O sistema lidará com uma quantidade grande de dados(informações de usuário e textos em tradução), que para um bom funcionamento do sistema não podem ser perdidos, para a persistência destes dados será utilizado um banco de dados relacional *PostgreSQL*|
|Arquitetura|Será feita uma arquitetura de microsserviços, para um melhor funcionamento e desempenho do sistema, já que não serão dependentes entre si|

### 4. Visão Lógica
---
#### 4.1. Visão geral de camadas e pacotes
---
### 5. Visão de implementação
---
#### 5.1. Diagrama de classes
---
### 6. Visão de implementação
---
### 7. Dimensionamento
---
### 8. Qualidade
---
