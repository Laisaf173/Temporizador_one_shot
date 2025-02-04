# Simulação temporizador de um disparo (One Shot) no Raspberry Pi Pico W

## Introdução
Este repositório contém um programa em C desenvolvido para o Raspberry Pi Pico W, utilizando o Pico SDK. O código implementa:
- One Shot (temporizador de um disparo com botão) - Um sistema em que um botão aciona três LEDs simultaneamente e eles apagam um de cada vez, a cada 3 segundos.

O código foi testado utilizando o simulador Wokwi e a ferramenta educacional BitDogLab.

## Funcionamento
Quando o botão é pressionado, os três LEDs acendem ao mesmo tempo. A cada **3 segundos**, um LED é desligado na seguinte ordem:

- LED Vermelho desliga primeiro.
- LED Amarelo desliga em seguida.
- LED Verde desliga por último.

O botão só pode ser pressionado novamente após todos os LEDs serem desligados. Um sistema de debounce evita leituras erradas do botão.
