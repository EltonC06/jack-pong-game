# Pong para Dois Jogadores — Projeto ESC

Este é um projeto de extensão do clássico jogo `Pong`, desenvolvido como parte da disciplina (Elementos de Sistemas de Computacionais) do curso de Sistemas de Informação da UFRPE baseado na plataforma `nand2tetris`. O objetivo foi adaptar o jogo para permitir dois jogadores humanos, com mecânicas de rebote, derrota e exibição de mensagens de "Game Over".

---

### 📌 Objetivo

Estender o jogo original `Pong` (localizado em `nand2tetris/projects/11/Pong`) para incluir:

* Dois jogadores humanos jogando simultaneamente.
* Controles independentes para cada jogador.
* Condições de vitória/derrota com exibição de mensagem final.

---

### 🎮 Controles

* **Jogador 1 (Barra Inferior):** Teclas Esquerda/Direita (← →)
* **Jogador 2 (Barra Superior):** Teclas A/D

---

### ✅ Funcionalidades Implementadas

* Segunda barra espelhada na parte superior da tela.
* Movimento independente para ambas as barras.
* Colisão e rebote da bola em ambas as barras.
* Detecção de derrota quando a bola ultrapassa a barra.
* Exibição de mensagem clara de "Game Over" com o jogador perdedor.
* Estrutura modular com os seguintes arquivos:
    ```
    ├── Main.jack
    ├── PongGame.jack
    ├── Ball.jack
    └── Bat.jack
    ```

---

### 🧠 Lógica de Jogo

* A bola rebate nas duas barras com a mesma lógica de colisão.
* Se a bola passar pela parte inferior, o **Jogador 1** perde.
* Se a bola passar pela parte superior, o **Jogador 2** perde.
* A mensagem de "Game Over" é exibida ao centro da tela com o jogador derrotado.
* O jogo pode ser reiniciado manualmente recarregando o projeto.

---

### 🛠️ Tecnologias

* **Linguagem:** `Jack`
* **Plataforma:** `nand2tetris`
* **Módulos:** Código organizado em classes reutilizáveis para manter a clareza e modularidade.