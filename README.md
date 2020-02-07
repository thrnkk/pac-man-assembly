
<p align="center">
  <img height="350px" widht="350px"  src="https://i.pinimg.com/originals/90/d2/e3/90d2e3ff2856032d36fcc7dc49334191.png">
</p>

# assemblyPacMan

Esse projeto consiste em recriar o famoso jogo Pacman programando-o na linguagem Assembly

## Pacman

O jogo consiste em:

> &nbsp;&nbsp;Pac-Man (conhecido em japonês com o nome de Puckman ou パックマン) é um jogo eletrônico criado pelo Tōru Iwatani para a empresa Namco, e sendo distribuído para o mercado americano pela Midway Games. Produzido originalmente para Arcade no início dos anos 1980, tornou-se um dos jogos mais jogados e populares no momento, tendo versões modernas para diversos consoles e continuações para tantos outros, inclusive na atualidade. A mecânica do jogo é simples: o jogador era uma cabeça redonda com uma boca que se abre e fecha, posicionado em um labirinto simples repleto de pastilhas e 4 fantasmas que o perseguiam. O objetivo era comer todas as pastilhas sem ser alcançado pelos fantasmas, em ritmo progressivo de dificuldade.

## Programas Necessários

> [Proteus 8 Professional](https://www.labcenter.com/)

## Bibliotecas

> [8086](https://pt.wikipedia.org/wiki/Intel_8086)

## O projeto

<p align="center">
  <img src="https://cdn.discordapp.com/attachments/646426616351817762/674015240589148170/unknown.png">
</p>

O projeto foi desenvolvido como um trabalho para a matéria de `Arquitetura de Computadores II` no ano de 2020, ele explora uma lógica criada para trabalhar com diversos sprites, sendo somente para o pacman, um total de 8 (2 para cada lado).

### Estrutura para o Funcionamento do Jogo

<p align="center">
  <img src="https://cdn.discordapp.com/attachments/646426616351817762/675135853751828519/unknown.png">
</p>

São necessário `três principais` componentes para conseguir reproduzir o jogo:

> processador 8086 para comportar a lógica.<br>
> processador 8253 para comportar os sons. <br>
> terminal de vídeo.<br>
