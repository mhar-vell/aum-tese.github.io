---
layout: page
title: turBOT
subtitle: Mini Autonomous Underwater Vehicle
---

{% assign date_format = site.date_format | default: "%B %-d, %Y" %}
{%- capture site_tags -%}
    {%- for tag in site.tags -%}
      {% if tag contains 'turbot' %}
        {{- tag | first -}}{%- unless forloop.last -%},{%- endunless -%}
      {% endif %} 
    {%- endfor -%}
{%- endcapture -%}
{%- assign tags_list = site_tags | split:',' | sort -%}

<center><img style="border:0px solid black;" src="{{ 'assets/img/turbot/turbot-design.png' | relative_url }}" text-align=center width="500" alt="Mohan" /><br></center>

<div class="before-content">
  <center>
    {%- for tag in tags_list -%}
      <br>
      <a href="#{{- tag -}}" class="btn btn-primary tag-btn"><i class="fas fa-tag" aria-hidden="true"></i>&nbsp;{{- tag -}}-posts&nbsp;({{site.tags[tag].size}})</a>
    {%- endfor -%}
  </center>    
  <!--hr class="mark"-->
</div>

<!-- ## Introdução -->
turBOT é um veículo subaquático autônomo de pequenas dimensões feito para realizar pesquisas costeiras em águas rasas. O projeto é concebido pela parceria  entre o SENAI CIMATEC e a Universidade de San Diego, nos Estados Unidos. 
<br>

## Detalhamento
Os principais objetivos são realizar o Estudo do Estado da Arte sobre temas relacionados, confeccionar o design da estrutura externa do veículo e realizar a sua simulação CFD, implementar funcionalidades de autonomia usando a prática de simulação em tempo real e a escrita de artigos relacionados às atividades desenvolvidas ao longo do projeto. 

turBOT será capaz de  navegar em ambientes subaquáticos internos e externos de até 50 m de profundidade. Será capaz de identificar e desviar de obstáculos e irá possuir eficiência energética suficiente para executar por completo suas tarefas.
Até o momento, o projeto turBOT submeteu um resumo expandido à conferência <a href="https://global21.oceansconference.org">Global OCEANS 2021</a>, em San Diego. Ao longo de 2021 espera-se participar de outras conferências e revistas como a <a href="https://ieeeoes.org/publications/ieee-journal-of-oceanic-engineering">IEEE Journal of Oceanic Engineering</a>
<br>

## Simulação
Simulação realizada no Gazebo com uso do <a href="https://uuvsimulator.github.io/">UUV Simulator</a>:
<center><iframe width="560" height="315" src="https://www.youtube.com/embed/ib3dWUQ7jkM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center>
<br>


<!-- equipe -->
<center><h3 class="post-title">Equipe de desenvolvimento</h3><br/></center>
<div class="row">
  <div class=" col-xl-auto offset-xl-0 col-lg-4 offset-lg-0">
    <table class="table-borderless highlight">
      <thead>
        <tr>
          <th><center><img src="{{ 'assets/img/people/marcoreis8b&w-1.png' | relative_url }}" width="100" alt="andersonqueiroz" class="img-fluid rounded-circle" /></center></th>
          <th></th>
          <th><center><img src="{{ 'assets/img/people/leonardolima-1.png' | relative_url }}" width="100" alt="brenda" class="img-fluid rounded-circle"/></center></th>
          <th></th>
          <th><center><img src="{{ 'assets/img/people/viniciusfelismino-1.png' | relative_url }}" width="100" alt="marco" class="img-fluid rounded-circle"/></center></th>
          <th></th>
          <th><center><img src="{{ 'assets/img/people/felipemohr-1.jpg' | relative_url }}" width="100" alt="marco" class="img-fluid rounded-circle"/></center></th>
        </tr>
      </thead>
      <tbody>
        <tr class="font-weight-bolder" style="text-align: center margin-top: 0">
          <td width="25%">Marco Reis</td>
          <td></td>
          <td width="25%">Leonardo Lima</td>
          <td></td>
          <td width="25%">Vinícius Felismino</td>
          <td></td>
          <td width="25%">Felipe Mohr</td>
        </tr>
        <tr style="text-align: center" >
          <td style="vertical-align: top"><small>Pesquisador Sênior do projeto <br>Mestre em Engenharia de Produção e Eng. Eletricista.</small></td>
          <td></td>
          <td style="vertical-align: top"><small>Engenheiro de Controle e Automação e especialista em robótica. Responsável pela simulação real-time.</small></td>
          <td></td>
          <td style="vertical-align: top"><small>Engenheiro Mecânico e especialista em robótica. Responsável por desenhos e simulações CFD.</small></td>
          <td></td>
          <td style="vertical-align: top"><small>Graduando em Engenharia Elétrica. Suporte em etapas de desenvolvimento e pesquisa do projeto.</small></td>
        </tr>
      </tbody>
    </table>
  </div>
</div>
<br>

### Resumo do Projeto
1. Categoria: <font color="#fbb117">AUV</font>
2. Prazo: <font color="#fbb117">02 anos</font>
3. Data de início: <font color="#fbb117">23/novembro/2020</font>
4. Data de término: <font color="#fbb117">28/outubro/2022</font>
5. Repositório URL: <a href="https://github.com/Brazilian-Institute-of-Robotics/bir_turbot"><font color="#fbb117">turBOT Simulation</font></a>
6. Apresentação URL: <a href="https://github.com/Brazilian-Institute-of-Robotics/bir_turbot-docs"><font color="#fbb117">turBOT Docs</font></a>
7. Artigos produzidos: <a href="https://github.com/Brazilian-Institute-of-Robotics/bir_a_turbot-simulation"><font color="#fbb117">turBOT Simulation paper</font></a>

<br>

## Referências
1. Manhães, M. M. M. et al. Uuv simulator: A gazebo-based package for underwater
intervention and multi-robot simulation. In: OCEANS 2016 MTS/IEEE Monterey. [S.l.:
s.n.], 2016. p. 1–8.

<br>
<hr class="mark">
<div id="full-tags-list">
<h3 class="post-title"><font color="#fbb117">Posts</font></h3>
  {%- for tag in tags_list -%}
      <h4 id="{{- tag -}}" class="linked-section">
          <i class="fas fa-tag" aria-hidden="true"></i>
          &nbsp;{{- tag -}}&nbsp;({{site.tags[tag].size}})
      </h4>
      <div class="post-list">
          {%- for post in site.tags[tag] -%}
              <div class="tag-entry">
                  <a href="{{ post.url | relative_url }}">{{- post.title -}}</a>
                  <div class="entry-date">
                      <time datetime="{{- post.date | date_to_xmlschema -}}">{{- post.date | date: date_format -}}</time>
                  </div>
              </div>
          {%- endfor -%}
      </div>
  {%- endfor -%}
</div>
