---
layout: page
title: AUM
subtitle: Planejamento dinâmico de trajetórias de manipuladores subaquáticos
---

<center>
<img src="{{ 'assets/img/aum/mohan-model.png' | relative_url }}" text-align=center width="500" alt="Mohan" />
</center><br>

## Desenvolvendo um modelo
A interação veículo-manipulador subaquático é uma das principais novas áreas de estudo para a pesquisa subaquática, pois inclui movimento acoplado e incertezas de parâmetros \cite{Mohan2015}. Segundo \citeonline{Mohan2015}, esses veículos começaram a desempenhar um papel vital nas atividades submarinas, incluindo, mas não se limitando, à exploração do fundo do mar, petróleo offshore, investigações militares e científicas. A dinâmica não-linear acoplada entre o veículo e o braço do manipulador apresenta desafios únicos no ambiente submarino \cite{Mohan2015Londhe}.

O objetivo deste projeto é desenvolver um modelo para a compensação das perturbações sofridas por manipuladores utilizados em veículos submarinos remotamente controlados.

Um dos pontos importantes no desenvolvimento da autonomia de um manipulador robótico é a sua consistência na movimentação de objetos em seu *end-effector*. O fato do desenvolvimento desta pesquisa estar sendo submetido a um ambiente subaquático eleva ainda mais a importância no desenvolvimento dos testes, onde vários componentes são integrados entre si e desempenham funcionalidades específicas para um ambiente controlado. Trazer estes aspectos para o laboratório é algo que deve ser preponderante para a realização do projeto, pois o mesmo deve ser testado e simulado com elementos capazes de ambientalizar o fenômeno do ponto de visto de controle num ambiente subaquático. 

<br>

## Detalhamento
O processo dessa pesquisa empregará um estudo dos algoritmos de planejamento de trajetória dinâmico para manipuladores, a partir de métodos estatísticos e comparativos. O desenvolvimento é feito padronizando os métodos e elementos para que sejam compatíveis com o framework de Sistema Operacional de Robô (ROS, do inglês *Robot Operation System*) na versão Noetic. 

<br>

## Simulação
Como o projeto está em desenvolvimento, simulações parciais estão sendo testadas (referência).

<br>

## Live Action
Testes preliminares também estão sendo realizados em laboratório, onde alguns resultados foram alcançados.

<br>


<center>
  <h3 class="post-title">Equipe de desenvolvimento</h3><br/>
</center>
<div class="row">

  <div class=" col-xl-auto offset-xl-0 col-lg-4 offset-lg-0">
      <table class="table-borderless highlight">
        <thead>
          <tr>
            <th><center><img src="{{ 'assets/img/people/andersonvale1.png' | relative_url }}" width="100" alt="andersonqueiroz" class="img-fluid rounded-circle" /></center></th>
            <th></th>
            <th><center><img src="{{ 'assets/img/people/brendaalencar.jpeg' | relative_url }}" width="100" alt="brenda" class="img-fluid rounded-circle"/></center></th>
            <th></th>
            <th><center><img src="{{ 'assets/img/people/marcoreis8b&w.png' | relative_url }}" width="100" alt="marco" class="img-fluid rounded-circle"/></center></th>
          </tr>
        </thead>
        <tbody>
          <tr class="font-weight-bolder" style="text-align: center margin-top: 0">
            <td width="33.33%">Anderson Queiroz</td>
            <td></td>
            <td width="33.33%">Brenda Alencar</td>
            <td></td>
            <td width="33.33%">Marco Reis</td>
          </tr>
          <tr style="text-align: center" >
            <td style="vertical-align: top"><small>Pesquisador Jr. do projeto <br>Engenheiro da Computação, Especialista em Robótica e Sistemas Autonônomos.</small></td>
            <td></td>
            <td style="vertical-align: top"><small>Estagiária no CC RoSA, graduanda em Eng. Elétrica.</small></td>
            <td></td>
            <td style="vertical-align: top"><small>Pesquisador Sênior do projeto <br>Mestre em Engenharia de Produção e Eng. Eletricista.</small></td>
          </tr>
        </tbody>
      </table>
  </div>
</div>

<br>

### Resumo do Projeto
1. Categoria: Manipuladores
2. Prazo: 02 anos
3. Data de início: <font color="#fbb117">23/novembro/2020</font>
4. Data de término: <font color="#fbb117">28/outubro/2022</font>
5. Repositório URL: 
6. Sponsor: <a href="http://www.senaicimatec.com.br/en/"><font color="#fbb117">Senai CIMATEC</font></a>
7. Recursos materiais: US$
8. Apresentação URL:
9. Report URL: 
10. Artigos relacionados: 

<br>

## Referências
##### 1 
SANTHAKUMAR, M.;  KIM, J. Robust adaptive tracking control of autonomous underwater vehicle-manipulator systems.Journal  of  Dynamic  Systems,  Measurement,and Control, American Society of Mechanical Engineers Digital Collection, v. 136, n. 5,2014.  
##### 2 
DANNIGAN, M.; RUSSELL, G. T. Evaluation and reduction of the dynamic coupling between a manipulator and an underwater vehicle.IEEE Journal of Oceanic Engineering,IEEE, v. 23, n. 3, p. 260–273, 1998.   
