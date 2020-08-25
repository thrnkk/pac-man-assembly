
<p align="center">
  <img height="350px" widht="350px"  src="https://i.pinimg.com/originals/90/d2/e3/90d2e3ff2856032d36fcc7dc49334191.png">
</p>

## Descrição do Projeto

Esse projeto consiste em recriar uma espécie de `PACMAN` utilizando a linguagem de programação `Assembly`.

### Requisitos :heavy_check_mark:

<ul>
  <li> O jogo deve ter splash art de abertura e deve aguardar o usuário pressionar uma tecla :heavy_check_mark: </li> 
  <li> O Pacman deve ir para todos os lados com atalhos do teclado :heavy_check_mark:</li>
  <li> O Pacman deve ter colisão com as paredes :heavy_check_mark:</li>
  <li> O Pacman deve mudar a sprite de si próprio :heavy_check_mark:</li>
  <li> O jogo deve gerar paredes randomicamente :heavy_check_mark:</li>
  <li> O jogo deve emitir áudio em algum momento :x:</li>
  <li> O jogo deve mostrar a pontuação :heavy_check_mark:</li>
  <li> O jogo deve gerar frutas gradativamente :heavy_check_mark:</li>
  <li> O jogo deve finalizar quando a tela for preenchidas por frutas (derrota) :heavy_check_mark:</li>
  <li> O jogo deve finalizar quando o jogador comer todas as frutas (vitória) :heavy_check_mark:</li>
</ul>

### Programas Necessários :computer:

É necessário utilizar algum simulador para conseguir simular o processador com o programa sendo executado em sua memória. No caso foi utilizado o [Proteus 8 Professional](https://www.labcenter.com/).

### Bibliotecas :books:

O projeto necessita da biblioteca do processador [8086](https://pt.wikipedia.org/wiki/Intel_8086) dentro do Proteus para o seu funcionamento adequado.

### O projeto :space_invader:

O projeto exibe a seguinte tela, permitindo o movimento do jogador pelo WASD.

<p align="center">
  <img src="https://cdn.discordapp.com/attachments/646426616351817762/674015240589148170/unknown.png">
</p>

### Estrutura :hammer_and_wrench:

<p align="center">
  <img src="https://cdn.discordapp.com/attachments/646426616351817762/675135853751828519/unknown.png">
</p>

A imagem contém componentes que não são necessários para o funcionamento do jogo.

Somente `três` componentes são essenciais:

<ul>
  <li> processador 8086 para comportar a lógica. :heavy_check_mark:</li> 
  <li> processador 8253 para comportar os sons. :x:</li> 
  <li> terminal de vídeo. :heavy_check_mark:</li> 
</ul>

---

<p align="center">
  <a href="https://github.com/thrnkk" ><img src="https://img.shields.io/badge/github-thrnkk-24292e"></a>
</p>
