
<p align="center">
  <img height="350px" widht="350px"  src="https://i.pinimg.com/originals/90/d2/e3/90d2e3ff2856032d36fcc7dc49334191.png">
</p>

# assemblyPacMan

Esse projeto consiste em recriar o famoso jogo Pacman programando-o na linguagem Assembly

## Pacman

O jogo consiste em:

> &nbsp;&nbsp;Pac-Man (conhecido em japonês com o nome de Puckman ou パックマン) é um jogo eletrônico criado pelo Tōru Iwatani para a empresa Namco, e sendo distribuído para o mercado americano pela Midway Games. Produzido originalmente para Arcade no início dos anos 1980, tornou-se um dos jogos mais jogados e populares no momento, tendo versões modernas para diversos consoles e continuações para tantos outros, inclusive na atualidade. A mecânica do jogo é simples: o jogador era uma cabeça redonda com uma boca que se abre e fecha, posicionado em um labirinto simples repleto de pastilhas e 4 fantasmas que o perseguiam. O objetivo era comer todas as pastilhas sem ser alcançado pelos fantasmas, em ritmo progressivo de dificuldade.

## Bibliotecas

> [8086](https://pt.wikipedia.org/wiki/Intel_8086)

## O projeto

<p align="center">
  <img src="https://cdn.discordapp.com/attachments/646426616351817762/674015240589148170/unknown.png">
</p>

O projeto foi desenvolvido como um trabalho para a matéria de `Arquitetura de Computadores II` no ano de 2020, ele explora uma lógica criada para trabalhar com diversos sprites, sendo somente para o pacman, um total de 8 (2 para cada lado).

### Loop para Funcionamento do Jogo

Primeiramente é necessário criar um loop para rodar o jogo e não permitir que o mesmo termine, e isso foi feito da seguinte forma:

> <br>
>
> MAIN:
>
> ```//Compara se o jogador perdeu```<br>
> &nbsp;&nbsp;CMP DERROTA_PAC, 1<br>
> 
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```//Se sim, pula para o loop de derrota```<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;JE DERROTA_LOOP<br>
>   
> ```//Compara se a comida tiver < 1```<br>
> &nbsp;&nbsp;CMP CONT_FOOD, 1<br>
> 
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```//Se sim, pula para o loop de vitória```<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;JL VITORIA_LOOP<br>
> 
> ```//Chama a função responsável por desenhar o mapa```<br>
> &nbsp;&nbsp;CALL DESENHA_MAPA<br>
>  
> ```//Define a primeira coluna como a sexta```<br>
> &nbsp;&nbsp;MOV CONT_COLUNA_PONTUACAO, 6<br>
>
> ```//Chama a função responsável por escrever a pontuação```<br>
> &nbsp;&nbsp;CALL ESCREVE_PONTUACAO_NUM<br>
>  
> ```//Chama a função responsável por receber os inputs```<br>
> &nbsp;&nbsp;CALL RECEBE_CARACTER<br>
> 
> ```//Retorna ao começo do loop```<br>
> &nbsp;&nbsp;JMP MAIN<br>
> <br>

