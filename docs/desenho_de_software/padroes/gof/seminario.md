# GOFs Proxy e Facade

## Proxy
### O que é?
Responsável por controlar o acesso ao objeto (OU CLASSE, PODEM MUDAR ISSO AQUI SE QUISEREM ) e modificar seu comportamento, agindo como um "substituto" do objeto real.

#### Benefícios
* Segurança
* Evita duplicação de obejtos, aumentando a eficiência

### Exemplo em Java
![](../../../assets/desenho/padroes/DiagramaProxy.png)
Veja o exemplo completo no [repositório](https://github.com/translate-me/exemplosGOF/tree/master/proxy).

### É aplicavel em nosso projeto?
A estrutura do proxy é facilmente aplicável no translate.me. Veja abaixo alguns exemplos iniciais de restrições que podem ser implementadas por proxy:

* __Validação da criação do perfil tradutor:__ Ao criar um perfil de tradutor ele deve ser associado a um usuário que ainda não possui um perfil de tradutor, e como o usuário cria o perfil através da plataforma, ele deve estar logado.

* __Controlar visualização de fragmentos:__ A visualização de um fragmento deve ter algumas seguranças em relação a qual usuário está visualizando o fragmento, caso seja o usuário tradutor, que está traduzindo, ele deve poder ver tanto o texto a ser traduzido quanto a sua tradução, caso seja o autor, não deve ser visto a tradução até que a mesma esteja pronta. Um usuário não envolvido não deve ter permissão de visualização.

* __Criação de categorias:__ Durante a criação de uma categoria deve ter uma validação para que a categoria criada não é repetida.

    (Essa validação pode também ser feita com o Multiton)

Inclusive o Django, plataforma utilizada no projeto do translate.me para fazer a API de microsservissos, utiliza deste padrão de projeto. O __serializer__ do Django é um proxy que adiciona restrições, controle e valida os dados serão passados para a API.



## Facade
### O que é?
Facade é um dos Padrões de Design mais simples e mais usados na programação orientada a objetos. Ele discute o encapsulamento de um subsistema complexo dentro de um único objeto de interface. Isso reduz a curva de aprendizado necessária para alavancar com sucesso o subsistema. Também promove o desacoplamento do subsistema de seus potencialmente muitos clientes. Por outro lado, se o Facade for o único ponto de acesso para o subsistema, ele limitará os recursos e a flexibilidade que os "usuários avançados" podem precisar. Esse tipo de padrão de projeto vem sob padrão estrutural, pois esse padrão adiciona uma interface ao sistema existente para ocultar suas complexidades.
Esse padrão envolve uma única classe que fornece métodos simplificados requeridos pelo cliente e chama representantes para métodos de classes de sistema existentes.

### Exemplo em Java

### É aplicavel em nosso projeto?