# COLLECTIONS FRAMEWORK
- Oque é:
    -   Collection é um objeto que agrupa múltiplos elementos
(variáveis primitivas ou objetos) dentro de uma única unidade.
- Composição:
  - Interfaces: É um contrato que quando assumido por uma
classe deve ser implementado.
  - Implementações ou Classes: são as materializações, a
codificação das interfaces.
  - Algoritmos: É uma sequência lógica, finita e definida de
instruções que devem ser seguidas para resolver um problema.

  ## Interface List
- ArrayList x LinkedList
  - ArrayList deve ser usado onde mais operações de pesquisa são necessárias, e LinkedList
deve ser usado onde mais operações de inserção e exclusão são necessárias.
- Declaração ArrayList: 
  - Ex: "List < Double> lista = new ArrayList< Double>();"
-   Métodos ArrayList:
    -   _lista.add_(_elemento a inserir_): adiciona itens no final da lista;
    -   _lista.indexOf_(_elemento a buscar_): retorna indice do elemento buscado;
    -   _lista.add_(_indice_,_elemento a inserir_): adiciona item ao índice informado;
    -   _lista.set_(_indice_,_elemento q vai substituir_): substitui o item da posicão do indice
    -   _lista.contains_(_elemento a procurar_): retorna true se elemento estiver na lista, senão false
    -   _lista.get_(_indice_): retorna o elemento do indice
    -   _Collections.min(lista)_: retorna o menor elemento da lista
    -   _Collections.max(lista)_: retorna o maior elemento da lista
    -   _lista.iterator()_: itera sobre a lista, declaração é *Iterator< TipoElementosDaLista> iterator = lista.iterator()*
        -   _iterator.hasnext()_: verifica se há um proximo elemento na lista, true se sim false senao
        -   *iterator.next()*: pega o valor do prox elemento da lista
        -   *iterator.remove()*: remove elemento da posicao do iterator
    - *lista.size()*: retorna a qtd de elementos da lista
    - *lista.remove(posicao ou elemento)*: remove o elemento informado ou elemento da posicao informada
    - *lista.clear()*: limpa toda a lista.
    - *lista.IsEmpty()*: retorna true se lista for vazia, senao false


