# Detona Ralph - Jogo Interativo

## Descrição
Este projeto é um jogo inspirado no filme **"Detona Ralph"**, onde o jogador precisa clicar nos inimigos que aparecem na tela para marcar pontos antes que o tempo acabe. O objetivo é alcançar a maior pontuação possível.

## Funcionalidades
- **Interface visual**:
  - Exibe o **tempo restante**, a **pontuação** e o número de **vidas**.
  - Alvo visualizado em quadrados dinâmicos.
- **Contagem regressiva**: O jogo termina automaticamente quando o tempo acaba.
- **Sistema de pontuação**: Incrementa ao acertar o inimigo.
- **Feedback sonoro**: Um som é reproduzido quando o jogador acerta o inimigo.

## Estrutura
### **HTML**
Define a estrutura do jogo:
- Um **menu superior** que mostra:
  - Tempo restante.
  - Pontuação atual.
  - Quantidade de vidas.
- Um **painel 3x3** com quadrados onde os inimigos aparecem.

### **CSS**
Responsável pelo estilo:
- Fundo com textura e cores vibrantes.
- Destaque visual para o inimigo (imagem do Ralph).
- Interface pixelada com fontes retro.

### **JavaScript**
Gerencia a lógica do jogo:
- **Estado do jogo (`state`)**:
  - `state.view`: Referências aos elementos do DOM.
  - `state.values`: Variáveis do jogo como tempo restante, pontuação e posição do inimigo.
  - `state.actions`: Gerencia os temporizadores (`setInterval`).
- **Funções principais**:
  - `countDown`: Gerencia o tempo restante.
  - `randomSquare`: Escolhe o próximo quadrado a exibir o inimigo.
  - `playSound`: Reproduz sons ao acertar o inimigo.
  - `addListenerHitBox`: Adiciona eventos para capturar cliques.
  - `initialize`: Inicializa os eventos e configurações do jogo.


