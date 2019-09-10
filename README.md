# AFD

Um Estado é criado instanciando um objeto da classe __Estado__, que leva como parâmetros: o "nome" do Estado, uma lista com possíveis Estados que ele pode transitar*, uma lista com o alfabeto das transições*, um parâmetro booleano que verifica se o Estado é inicial ou não e por fim um Estado que verifica se ele é final ou não.
    
   __Exemplo:__   ```estado1 = Estado('q1', ['q2', 'q3'], ['a', 'b'], True, False)```
    
Algumas observações sobre as listas:
  - A lista de Estados possíveis é uma lista de Strings, onde cada String é o nome do Estado que ele pode transitar.
  - A lista com o alfabeto está relacionada com a lista de Estados, ou seja, a primeira posição da *listaAlfabeto* está relacionada com a primeira posição da *listaEstados*, dessa forma é representada a transição de um Estado para outro.
  - Portanto, as listas devem ter o mesmo tamanho.
