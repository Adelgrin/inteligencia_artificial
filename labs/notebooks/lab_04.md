# Laboratório 04 de algoritimo CSP e MRV
## Desafio 1
Principais fuções:
* is_consistent_map
* backtracking_map
### is_consistent_map:
Esta função recebe o mapa de vizinhos definido anteriormente e itera entre os valores deste dicionario.
então ele retora o estado de um valor que tenha sido visitado negado (isto é com a função de not invertemos o estado)
### backtracking_map:
Esta função começa verificando se todos os valores foram verificados por meio de verificação do tamanho das listas
então verificamos e a variavel foi visitada, se não ela é adicionada no começo de uma lista para um funcionamento parecido como uma fila, e o processo é

para cada valor no mapa se ele for consistente baseado na função `is_consistent_map` ele adiciona este valor no grafo e faz o backtracking se retornar um resultado adicionamos ele, se não removemos ele do grafo essenciamente matando o galho

## Desafio 2
Principais funções:
* create_domains
* initial_assignment
* is_valid
* backtracking_sudoku
* select_mrv_variable
* backtracking_mrv
### create_domains:
Esta função cria uma lista para funcionar como um grafo, definindo os valores x e y do tabuleiro para todos os valores iguais a 0, essencialmente criando os objetivos
### initial_assignment:
Esta função cria um mapa de variaveis conhecidas com suas coordenadas x e y
### is_valid
Esta função permuta as duas listas criadas anteriormente e retorna apenas valores diferentes dos objetivos de criação.
### backtracking_sudoku:
Verifica o tamanho da lista para fazer uma sobrecarga do metodo e retornar a lista completa quando finaliazar a recursão.
Então verificamos e a variavel foi visitada, se não ela é adicionada no começo de uma lista para um funcionamento parecido como uma fila, e o processo é
### select_mrv_variable:
Define uma variavel não não visitada retorna o menor valor da lista de objetivos
### backtracking_mrv:
Sobrecarga do metodo para retornar a lista de variaveis não visitadas
seleciona a variavels ultilizando o metodo mrv e intera entre todos os valores do grafo para validar

