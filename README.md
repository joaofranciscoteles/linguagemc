# Jogo Da Vida

# Introdução
<p>O Jogo da Vida tem sua origem na brilhante mente do matemático inglês John Conway, o qual desenvolveu um conjunto de regras para simular o desenvolvimento de uma civilização que são aplicadas a cada nova geração. Essas regras quando aplicadas reproduzem alterações e mudanças nas civilizações, gerando muitas vezes comportamentos estáveis e recorrentes, como também caóticos e imprevisíveis. Dentre as regras criadas pelo matemático estão: 

- Uma célula viva com menos de dois vizinhos vivos morre (solidão).
- Uma célula viva com mais de três vizinhos vivos morre (superpopulação).
- Uma célula viva com dois ou três vizinhos vivos sobrevive.
- Uma célula morta com exatamente três vizinhos vivos se torna viva (reprodução). </p>

# Objetivo
<p>Com a finalidade de simular as ideias do Jogo da Vida, foi desenvolvido um programa que recebendo uma Civilização 0 e um número de gerações como entrada, faria as alterações e mudanças nas células, gerando um novo mapa atualizado pelas regras base do Jogo da vida com a nova civilização.  </p>

# Solução Proposta
<p>Para o desenvolvimento do programa o Jogo da Vida, foram criados 3 arquivos: Main.cpp, JogoDaVida.cpp e JogoDaVida.hpp

- Main.cpp: contém a abertura dos arquivos de entrada e saída, a leitura do número de gerações pelo usuário, a instanciação da classe JogoDaVida e a chamada de suas funções.
- JogoDaVida.hpp:Contém a declaração das variáveis e funções envolvidas no processo
- JogodaVida.cpp: Contém a declaração das funções utilizadas.

Para atualizar as células foram utilizadas duas matrizes, uma chamada de original e uma cópia. A função processa_matriz que recebe as matrizes e faz a verificação das regras bases, utilizando a chamada de outra função para contar o número de vizinhos de cada célula em determinada posição.
</p>


<div align=center>
<img src="Captura de tela de 2024-03-21 20-13-55.png" width="650px">
</div>
<p  align="center">
A imagem ilustra o funcionamento da função processa_matriz juntamente com a função conta_vizinhos
</p>


# Compilação e Execução

Um arquivo Makefile que realiza todo o procedimento de compilação e execução está disponível no código. Para utilizá-lo, siga as diretrizes de execução no terminal:


| Comando                |  Função                                                                                           |                     
| -----------------------| ------------------------------------------------------------------------------------------------- |
|  `make clean`          | Apaga a última compilação realizada contida na pasta build                                        |
|  `make`                | Executa a compilação do programa utilizando o gcc, e o resultado vai para a pasta build           |
|  `make run`            | Executa o programa da pasta build após a realização da compilação       
