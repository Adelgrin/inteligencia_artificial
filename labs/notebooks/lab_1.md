# Relatório jogo dos oito

## Implementações:
* classe PuzzleState
    1. função init
    2. função is_goal
    3. função get_sucessor
* função print_board
* função reconstruct_path
* função show_solution
* função bfs
* função manhattan_distance
* função a_star

### PuzzleState
Esta classe implementa as funções para definir o objetivo e como devemos processar os nós sequenciais além de inicializara matriz

### print_board
Esta função serve apenas para representar de maneira visual o tabuleiro

### reconstruct_path
Adiciona a uma lista o caminho ultilizado sendo calculado de maneira reversa (do final para o inicio)

### show_solution
apresenta o caminho construido pelo reconstruct_path e todos os tabuleiros printados usando print_board

### bfs
Implentação da função bfs para explorar todos os nós visitados de maneira recursiva

### manhattan_distance
Calculo da distancia a posição atual e o objetivo

### a_star
Implementação parecida com o bfs porem ultiliza a heuristica da distancia até o objetivo
