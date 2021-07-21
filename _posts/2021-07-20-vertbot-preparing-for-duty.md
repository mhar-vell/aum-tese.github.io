---
layout: post
title: Preparing for duty
subtitle: Sensors tests and Gazebo first steps
thumbnail-img: /assets/img/vertbot/vertbot_model.png
share-img: /assets/img/rosa-logo-redondo.png
tags: [vertbot]
---

# Testando os sensores do Vertbot

Nesta etapa de desenvolvimento foi feita a pesquisa dos pacotes e das bibliotecas necessárias para o funcionamento dos diversos sensores presentes no projeto, seguido do teste e integração dos sensores com o ROS operando na Jetson Nano. Nos testes feitos com os sensores de corrente e de tensão, foi verificada uma inconsistência do valor apresentado como resultado para o valor real que estava sendo medido, devido a uma não linearidade nas respostas dos sensores. Devido a isso, foi levantada a curva das suas respostas analógicas de saída em função das suas entradas, e feita uma linearização na faixa de operação que a alimentação do robô estará operando.Os sensores de corrente, de tensão e o sensor ultrassônico são sensores com resposta analógica de até 5 V, tensão não suportada pelas portas analógicas da Jetson Nano. Portanto tais sensores serão ligados a um microprocessador Arduino Nano, sendo necessário o pacote rosserial para a integração das respostas do Arduino com o ROS operando na Jetson Nano.

![Teste do sensor de corrente](https://raw.githubusercontent.com/mhar-vell/projects/vertbot/assets/img/vertbot/test_current_sensor.jpg)
<!-- ![Teste do sensor de corrente](https://raw.githubusercontent.com/mhar-vell/projects/master/assets/img/vertbot/test_current_sensor.jpg) master branch -->

![Teste do sensor de tensão](https://raw.githubusercontent.com/mhar-vell/projects/vertbot/assets/img/vertbot/test_voltage_sensor.jpg)
<!-- ![Teste do sensor de tensão](https://raw.githubusercontent.com/mhar-vell/projects/master/assets/img/vertbot/test_voltage_sensor.jpg) master branch -->

![Tabela do teste do sensor de tensão](https://raw.githubusercontent.com/mhar-vell/projects/vertbot/assets/img/vertbot/test_table_voltage_sensor.jpg)
<!-- ![Tabela do teste do sensor de tensão](https://raw.githubusercontent.com/mhar-vell/projects/master/assets/img/vertbot/test_table_voltage_sensor.jpg) master branch -->

![Teste do sonar](https://raw.githubusercontent.com/mhar-vell/projects/vertbot/assets/img/vertbot/test_sonar.jpg)
<!-- ![Teste do sonar](https://raw.githubusercontent.com/mhar-vell/projects/master/assets/img/vertbot/test_sonar.jpg) master branch -->

O pacote disponível para a câmera estéreo Mynt Eye é desenvolvido para o Ubuntu 18.04, porém a versão usada na Jetson Nano é a 20.04, sendo necessário o uso do container Docker com a versão 18.04 do Ubuntu para utilizar o pacote. Os demais sensores apresentaram respostas coerentes com os pacotes encontrados no estudo da arte desenvolvido.

![Teste da camera Mynt Eye](https://raw.githubusercontent.com/mhar-vell/projects/vertbot/assets/img/vertbot/test_mynt-eye.jpg)
<!-- ![Teste da camera Mynt Eye](https://raw.githubusercontent.com/mhar-vell/projects/master/assets/img/vertbot/test_mynt-eye.jpg) master branch -->

![Teste da camera Rasp V2](https://raw.githubusercontent.com/mhar-vell/projects/vertbot/assets/img/vertbot/test_camera_v2.jpg)
<!-- ![Teste da camera Rasp V2](https://raw.githubusercontent.com/mhar-vell/projects/master/assets/img/vertbot/test_camera_v2.jpg) master branch -->

![Teste do LiDAR](https://raw.githubusercontent.com/mhar-vell/projects/vertbot/assets/img/vertbot/test_lidar.jpg)
<!-- ![Teste do LiDAR](https://raw.githubusercontent.com/mhar-vell/projects/master/assets/img/vertbot/test_lidar.jpg) master branch -->

# Desenvolvimento do URDF

Após a atualização da estrutura do modelo do robô, foi dado o início da construção do arquivo URDF para inicializar a simulação. Alguns ajustes serão feitos futuramente no chassis para adicionar os encaixes do sensor de corrente, sensor de tensão e shield do motor, além do desenvolvimento de uma peça de encaixe da _caster ball_ e possíveis redimensionamentos para o encaixe de peças que estão em processo de compra. Com o workspace da simulação já iniciado, é possível começar os testes de sensores via simulação para a criação da rede de sensores e os testes de interação entre eles, além do desenvolvimento dos algoritmos e das funcionalidades abordadas no projeto.

![Modelo Vertbot no Gazebo](https://raw.githubusercontent.com/mhar-vell/projects/vertbot/assets/img/vertbot/vertbot_gazebo.png)
<!-- ![Modelo Vertbot no Gazebo](https://raw.githubusercontent.com/mhar-vell/projects/master/assets/img/vertbot/vertbot_gazebo.png) master branch -->