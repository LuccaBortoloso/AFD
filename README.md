# AFD, como criar?

Um Estado é criado instanciando um objeto da classe __Estado__, que leva como parâmetros: o "nome" do Estado, uma lista com possíveis Estados que ele pode transitar*, uma lista com o alfabeto das transições*, um parâmetro booleano que verifica se o Estado é inicial ou não e por fim um Estado que verifica se ele é final ou não.
    
   __Exemplo:__   ```estado1 = Estado('q1', ['q2', 'q3'], ['a', 'b'], True, False)```
  
# Notas sobre as listas

Algumas observações sobre as listas:
  - A lista de Estados possíveis é uma lista de Strings, onde cada String é o nome do Estado que ele pode transitar.
  - A lista com o alfabeto está relacionada com a lista de Estados, ou seja, a primeira posição da *listaAlfabeto* está relacionada com a primeira posição da *listaEstados*, dessa forma é representada a transição de um Estado para outro.
  - Portanto, as listas devem ter o mesmo tamanho.  

# Palavra aceita?

Para verificar se uma palavra é aceita ou não, o primeiro passo é chamar a função *aceitePalavra()*. Para isso, você deve passar como parâmetros o autômato (que é uma lista de Estados) e a palavra que deve ser verificada.  
```automato = [estado1, estado2, estado3, ...]```  
```palavra = aceitePalavra(automato, 'abababa')```

# Minimização
Para saber a minimização do autômato basta utilizar a função *criandoTabela()* que tem como parâmetro o autômato (o mesmo da função anterior).

```criandoTabela(automato)```

O resultado é um dicionário indicando os Estados e se eles foram marcados ou não.

```q1,q2 = 'x' ```
```q2,q3 = '0' ```
