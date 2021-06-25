---
layout: page
title: Walker
subtitle: Um robô bípede
---

<center><img src="{{ 'assets/img/walker/walker_missao.png' | relative_url }}" alt="Walker_missao" width="380"/></center>

<!-- ## Introdução -->

### Apresentação
Um robô terrestre que se locomove sobre dois pés é classificado como bípede. Para isto, os movimentos realizados por este robô são similares a um andar antropomórfico. Movimentos antropomórficos são amplamente estudados e utilizados tanto na área medicinal como na industrial. 

<!--objetivo, data-->
O Walker faz parte da primeira fase do programa de estágio do laboratório de Robótica e Sistemas Autonômos. A iniciativa visa a construção de um robô autônomo bípede para exploração em um ambiente indoor controlado. Este projeto foi iniciado em 12 de maio de 2021 e será finalizado em 30 de julho de 2021. 

<!--justificativa-->
Um robô deste porte e com movimentação autônoma é comumente utilizado para realizar tarefas *indoor* simples e para interagir com os humanos. A elaboração e construção deste robô proporciona o aprendizado de conceitos básicos da robótica móvel e de visão computacional, como também, proporciona o embasamento para a formulação de um projeto. 

Para concepção do robô Walker, buscamos por projetos similares existentes, com o intuito de nortear nosso desenvolvimento.
A imagem a seguir ilustra as principais referências utilizadas para o projeto. 

<img src="{{ 'assets/img/walker/walker_semelhantes.png' | relative_url }}" alt="Semelhantes" />


Da esquerda para direita: ROFI [1], Darwin-OP [2] e NAO [3].


### Missão

Como missão do robô Walker, ele deverá explorar uma área delimitada em busca de uma TAG.
Ao encontrá-la, ela indicará a posição de uma esfera no ambiente.
O Walker deverá, então, deslocar-se até essa posição e encontrar a esfera.
A TAG e a esfera podem ser vistas na primeira imagem. 


### Como ele fará isso?
<img src="{{ 'assets/img/walker/walker_componentes.png' | relative_url }}" alt="Walker_componentes" />
<!--<img src="/assets/img/walker/walker_componentes.png" width="250">-->

Para desempenhar suas funções, o Walker contará com alguns componentes. 
Dentre eles, os principais são:
- **Raspberry Pi 4:** Será a central de processamento do robô, controlando todo seu funcionamento
- **Dynamixels XM430:** Atuadores que irão possibilitar o deslocamento do robô sobre dois pés
- **Sensores Ultrassônicos HC-SR04:** Permitirão a detecção de obstáculos, possibilitando sua navegação autônoma
- **Raspicam:** A câmera será utilizada para a detecção e reconhecimento de TAGs, possibilitando sua localização

## Equipe

<table border="0">
    <tr>
      <td><center><img src="{{ 'assets/img/people/brendaalencar-1.png' | relative_url }}" align="center" width="120" /></center></td>
      <td><center><img src="{{ 'assets/img/people/felipemohr-1.jpg' | relative_url }}" align="center" width="120" /></center></td>
      <td><center><img src="{{ 'assets/img/people/marcoreis8b&w-1.png' | relative_url }}" align="center" width="120" /></center></td>
    </tr>
    <tr>
        <td><b style="font-size:15px"><center>Brenda Alencar</center></b></td>
        <td><b style="font-size:15px"><center>Felipe Mohr</center></b></td>
        <td><b style="font-size:15px"><center>Marco Reis</center></b></td>
    </tr>
    <tr>
        <td><center>Estagiária no CC RoSA, graduanda em Eng. Elétrica. Participou de projetos de Robótica Subaquática e Manipuladores Subaquáticos</center></td>
        <td><center>Estagiário no CC RoSA, graduando em Eng. Elétrica. Participou de projetos de Robótica Subaquática e Robótica Móvel</center></td>
        <td><center>Eng. Eletricista e Mestre em Engenharia de Produção. Orientador e responsável pelos projetos do Centro de Competência RoSA</center></td>
    </tr>
</table>

### Resumo do Projeto
1. Categoria: Robótica móvel
2. Prazo: 2 meses e 18 dias
3. Data de início: 12/05/2021
4. Data de término: 30/07/2021
5. Repositório URL: [Walker](https://github.com/Brazilian-Institute-of-Robotics/bir_walker)
6. Sponsor: Senai Cimatec
7. Recursos materiais: --
8. Apresentação URL:[Walker-docs](https://github.com/Brazilian-Institute-of-Robotics/bir_walker-docs/tree/main)
9. Report URL: [Walker-report](https://github.com/Brazilian-Institute-of-Robotics/bir_walker-docs/tree/report-design)
10. Artigos relacionados:

## Referências
1. [ROFI](http://www.projectbiped.com/prototypes/rofi). **RObot FIve**. Acesso em: 7 de Junho de 2021 .
1. [Darwin-OP](https://emanual.robotis.com/docs/en/platform/op/getting_started). **ROBOTIS OP**. Acesso em: 7 de Junho de 2021.
1. [Nao](https://www.softbankrobotics.com/emea/en/nao). **NAO ROBOTIS SoftBank Robotics**. Acesso em: 7 de Junho de 2021.
