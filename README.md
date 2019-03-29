# Translate.me | Documentação
Documentação referente ao projeto do Tradutor, na disciplina de Desenho de Software

## Primeiros passos
Para editar a documentação, utilizando o [MKDocs](https://www.mkdocs.org/) e o template [Material Design](https://squidfunk.github.io/mkdocs-material/) e para utilizá-lo será necessário um ambiente com Python instalado e o gerenciador de dependências Pip.

## Editar a documentação
Para criar o site disponível em https://desenho2019-1.github.io/docs/ você deve realizar os seguintes passos:
* ```git clone https://github.com/desenho2019-1/docs.git```
* ```pip install mkdocs```
* ```pip install mkdocs-material```

E então veja localmente o seu site:
* ```mkdocs serve```

Assim, que estiver desejável, você deverá commitar suas alterações
* ```git add . ```
* ```git commit -m "Nome do seu commit em inglês"```
* ```git push origin master```

E atualizar a documentação disponível no site:
* ```mkdocs gh-deploy```
