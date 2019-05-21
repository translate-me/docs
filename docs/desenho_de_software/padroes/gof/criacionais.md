# GoFs Criacionais

## Histórico de Revisão:
| Data | Versão | Descrição | Autor |
|---|---|---|---|
| 20/05/2019 | 0.1 | Adicionando Multiton GOF | Gabriela Guedes |

## 1. Multiton

### 1.1 Definição


O multiton consiste na utilização de um método para retornar um objeto. Esse método deve receber uma chave, e caso já exista um objeto com essa chave, ele é retornado, caso contrário, um novo objeto é criado. O multiton é considerado uma extensão do padrão de projeto singleton, onde o método de criação de objetos deve ser privado e que só permite a criação de uma instância para a classe, no caso do multiton, é utilizado um dicionário para agrupar todas as instancias geradas.

### 1.2 Análise
É possivel a implementação do Multiton em nosso projeto, veja o exemplo de implementação em python:

``` py
def multiton(cls):
   instances = {}
   def getinstance(id):
      if id not in instances:
         instances[id] = cls(id)
      return instances[id]
   return getinstance


@multiton
class MyObject( object ):
   def __init__( self, arg):
      self.id = arg

a = MyObject(1)
b = MyObject(2)
c = MyObject(2)

print("Should be False:")
print(a is b)

print("Should be True:")
print(b is c)
```

### 1.3 Estrutura mínima

![](../../../assets/desenho/padroes/multiton.png)

* Mapeamento das instâncias a partir da chave
* Inicializador da classe
* Método `getInstance()` que retorna um objeto da classe

## 2. Referências
[Black Wasp - Multiton](http://www.blackwasp.co.uk/Multiton.aspx)
[Stack Overflow](https://stackoverflow.com/questions/669932/how-to-create-a-class-that-doesnt-re-create-an-object-with-identical-input-para)
