# Guess the Number

Jogo de Adivinhação com Circuitos Lógicos Combinacionais

![Funcionamento do jogo principal](/img/main.gif "Funcionamento do jogo principal")

## Introdução

Este relatório descreve o projeto de um jogo de adivinhação baseado em circuitos lógicos combinacionais. O jogo permite que dois jogadores façam palpites de 4 bits para tentar adivinhar um número secreto também representado por 4 bits. O circuito utiliza componentes como decodificadores de displays de segmentos, um circuito comparador de magnitude e multiplexadores 2 para 1.

## Objetivo
O objetivo deste projeto é criar um jogo de adivinhação em que dois jogadores alternam entre si para fazer palpites sobre um número secreto de 4 bits. O sistema deve avaliar os palpites e fornecer três resultados possíveis: "correto", "maior que o número secreto" e "menor que o número secreto" para cada jogada.

## Componentes Utilizados

### **Multiplexadores 2 para 1**
![Multiplexador 2 para 1](/img/mux.gif "Multiplexador 2 para 1")
Os multiplexadores são utilizados para alternar entre os jogadores, selecionar o palpite correto a ser exibido no display e escolher os sinais de resultado apropriados.

### **Circuito Comparador de Magnitude**
![Comparador](/img/comparator.gif "Comparador")
Um circuito comparador de magnitude é empregado para comparar os palpites dos jogadores com o número secreto. Ele determina se o palpite é maior, menor ou igual ao número secreto, gerando os sinais de resultado correspondentes.

### **Decodificadores para Displays de 7 Segmentos**
![Decodificador](/img/decoder.gif "Decodificador")

Dois decodificadores de displays de segmentos são utilizados para exibir os números de 0 a 15, correspondentes aos palpites e ao número secreto. Cada decodificador converte um valor binário de 4 bits em sinais de controle para segmentos de displays de 7 segmentos.

## Funcionamento
1. **Inicialização**:
   O jogo começa com ambos os displays de segmentos exibindo o número 0. O jogador inicial é definido através de um botão dedicado. Um palpite de 4 bits é inserido usando um conjunto de interruptores.

2. **Fase de Palpite**:
   O jogador ativo é selecionado pelo botão de seleção de jogador. O palpite é inserido por meio de interruptores de 4 bits.

3. **Comparação**:
   O palpite é comparado com o número secreto usando o circuito comparador de magnitude. Com base na comparação, os sinais de resultado são gerados - "correto", "maior que o número secreto" ou "menor que o número secreto".

4. **Exibição de Resultados**:
   Os resultados da comparação são exibidos nos displays de segmentos por meio dos decodificadores. Além disso, o display exibe o palpite atual.

5. **Alternância de Jogadores**:
   Após a exibição dos resultados, os jogadores alternam pressionando o botão de seleção de jogador.

6. **Fim do Jogo**:
   O jogo continua até que um dos jogadores adivinhe corretamente o número secreto. Nesse momento, um sinal de vitória é gerado, indicando o término do jogo.

## Conclusão
O jogo de adivinhação construído com circuitos lógicos combinacionais é um exemplo interessante de como elementos simples podem ser combinados para criar uma experiência interativa. Através do uso de decodificadores, comparadores e multiplexadores, os jogadores podem realizar palpites, receber feedback imediato e competir para adivinhar o número secreto. Isso demonstra a aplicação prática da lógica digital em cenários de entretenimento e jogos.