### Contexto execução debug
De inicio a função minimax é chamada para o maximizador. A variavel depth = 0; is_max = true.
- É iterado o minimax, é chamado evaluate(board), não possui vencedor, score = 0.
is-moves_left(board) retorna true porque ainda há movimentos. Inicializa best = -math.inf porque é a vez do maximizador.
 - O codigo roda o loop para passar pelos movimentos existentes, primeira posição encontrada e marcada com o X.
- Chamada recursiva: chama minimax(board, 1, false). depth +=1. is_max = false(porque é a vez do minimizador).
- O minimizador passa pelos movimentos restantes, marca a célula encontrada com O celula(0,2)
- Chamada recursiva pelo Minimizador: chama minimax(board, 2, true) - depth e incrementado para 2. is_max = true.
- Explorado movimentos pelo maximizador: passa pelas celulas encontra (1,0) e marca com X.
- Chamada recursiva pelo maximizador: chama minimax(boar, 3, false). depth = 3. is_max = false.

![imagem-debug](minimax.png)
