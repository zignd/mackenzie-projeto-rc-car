# Circuitos Elétricos e Eletrônicos 2º sem. 2018

## Turma 01N
## Projeto: Radio-Controlled Car
## Integrantes do grupo:

* Igor Hipólito Vieira, 4180942-4
* Salomon Asher Motoryn, 4182512-8

## Descrição resumida do projeto

Um carrinho de controle remoto controlado por sinal de rádio. O carrinho seria composto de um Arduino para processar o sinal de rádio recebido e controlar os motores com base nesses sinais, um micro motor DC para realizar o funcionamento das rodas traseiras, um motor de passo ou um servo motor para realizar o funcionamento das rodas frontais e um módulo NRF24L01 para comunicação sem fio com o controle. Já o controle seria composto de um Arduino, botões para o usuário decidir a direção e a velocidade e um módulo NRF24L01 para comunicaço sem fio com o carrinho.
_______________________________________

Obs:

`src/` códigos desenvolvidos

`doc/` documentação do projeto

## Descrição detalhada do hardware

### Controle remoto

Para a elaboração do controle, usamos um Arduino Uno, uma placa de protoboard 5x17, um módulo de rádio NRF24L01+ para transmissão de sinais ao módulo de rádio NRF24L01+ localizado no carrinho, um joystick, uma bateria de 9 volts para o Arduino. 

### Carrinho

Para a elaboração do carrinho, usamos um Arduino Uno, uma placa de protoboard 5x17, um módulo de rádio NRF24L01+ para o recebimento de sinais do módulo de rádio NRF24L01+ localizado no controle remoto, dois motores DC para operar as rodas, uma ponte H L298N para controlar os motores DC, uma bateria de 9 volts para o Arduino, 3 baterias de 3.7 volts para os motores DC junto com um suporte para baterias.

## Descrição do processo de montagem do projeto

### Controle remoto

Para a montagem do controle remoto, siga o diagrama de montagem abaixo utilizando os materiais descritos no tópico "Descrição detalhada do hardware" na seção "Controle remoto".

![Controle Remoto 1](https://i.imgur.com/Ams6EKq.png)
(diagrama de montagem)

![Controle Remoto 2](https://i.imgur.com/1WzhqcZ.png)
(diagrama esquemático)

Em seguida basta fazer o upload do código localizado em `src/controller/controller.ino` para o Arduino Uno que será utilizado para o controle remoto.

### Carrinho

Para a montagem do carrinho, siga o diagrama de montagem abaixo utilizando os materiais descritos no tópico "Descrição detalhada do hardware" na seção "Carrinho".

![Carrinho 1](https://i.imgur.com/YfYKh7C.png)
(diagrama de montagem)

![Carrinho 2](https://i.imgur.com/VJpcJ6v.png)
(diagrama esquemático)

Em seguida basta fazer o upload do código localizado em `src/car/car.ino` para o Arduino Uno que será utilizado para o carrinho.
