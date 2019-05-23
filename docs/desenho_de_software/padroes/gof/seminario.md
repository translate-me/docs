# GOFs Proxy e Facade

## Proxy
### O que é?

### Exemplo em Java
![](../../../assets/desenho/padroes/DiagramaProxy.png)
Veja o exemplo completo no [repositório](https://github.com/translate-me/exemplosGOF/tree/master/proxy).

### É aplicavel em nosso projeto?
A estrutura do Proxy é facilmente aplicável no translate.me. Veja abaixo alguns exemplos iniciais de restrições que podem ser implementadas por proxy:

* __Validação da criação do perfil tradutor:__ Ao criar um perfil de tradutor ele deve ser associado a um usuário que ainda não possui um perfil de tradutor, e como o usuário cria o perfil através da plataforma, ele deve estar logado.

* __Controlar visualização de fragmentos:__ A visualização de um fragmento deve ter algumas seguranças em relação a qual usuário está visualizando o fragmento, caso seja o usuário tradutor, que está traduzindo, ele deve poder ver tanto o texto a ser traduzido quanto a sua tradução, caso seja o autor, não deve ser visto a tradução até que a mesma esteja pronta. Um usuário não envolvido não deve ter permissão de visualização.

* __Criação de categorias:__ Durante a criação de uma categoria deve ter uma validação para que a categoria criada não é repetida.

    (Essa validação pode também ser feita com o Multiton)



## Facade
### O que é?

### Exemplo em Java

### É aplicavel em nosso projeto?