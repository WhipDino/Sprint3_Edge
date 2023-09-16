# Projeto de Monitoramento de Ambiente com Arduino e IoT

Este projeto demonstra como criar um sistema de monitoramento de ambiente utilizando um Arduino, sensores ultrassônicos, um LDR (Light-Dependent Resistor), um display LCD, e IoT (Internet das Coisas) para visualizar e analisar os dados coletados em tempo real.

# Sensores nos postes

O foco do nosso projeto é diminuir o consumo de energia e a poluição visual causada pelos postes de luz. Utilizaremos luz baixa enquanto ninguém estiver próximo, assim que for detectada a presença de um pedestre ou carro, os postes atingirão o nível de luminosidade necessário para a locomoção naquele trecho. Dessa forma é possível usar as tecnologias estudadas no curso para contribuir com a ideia de cidades inteligentes e sustentabilidade. Com os dados coletados pelos sensores de movimento, seremos capazes de entender o fluxo de pessoas e automóveis em cada local onde a tecnologia for utilizada, com essas informações é possível reduzir os tráfego em certas regiões e ajudar aplicativos de GPS a traçarem melhores rotas.


## Visão Geral

A Internet das Coisas (IoT) permite a conexão de dispositivos do mundo físico à internet, possibilitando o monitoramento e controle remoto de diversos parâmetros. Neste projeto, utilizamos um Arduino para coletar dados de um sensor ultrassônico e um LDR, que medem distância e luminosidade, respectivamente. Esses dados são transmitidos para um servidor Node-RED via MQTT (Message Queuing Telemetry Transport) e, em seguida, enviados para a plataforma TagoIO para análise e visualização.

## Componentes

### Hardware

- Arduino Uno
- Sensor Ultrassônico HC-SR04
- LDR (Light-Dependent Resistor)
- Display LCD 16x2
- Fonte de Tensão
- Jumpers e cabos diversos

### Software

- [Arduino IDE](https://www.arduino.cc/en/software)
- [Node-RED](https://nodered.org/)
- [TagoIO](https://tago.io/)

## Configuração

1. **Montagem do Hardware:** Monte os componentes conforme o esquema de ligação fornecido (inserir esquema aqui).

2. **Programação do Arduino:** Carregue o código do Arduino disponível neste repositório para o seu Arduino utilizando a Arduino IDE.

3. **Node-RED:** Configure um fluxo no Node-RED para receber dados do Arduino via MQTT. Certifique-se de ajustar as configurações MQTT de acordo com a sua rede.

4. **TagoIO:** Crie uma conta no TagoIO e configure uma integração MQTT para receber os dados do Node-RED.

5. **Dashboard TagoIO:** Crie um dashboard personalizado no TagoIO para visualizar os dados coletados em tempo real.

## Uso

Após a configuração, o sistema estará coletando dados do sensor ultrassônico e do LDR. Esses dados serão enviados para o Node-RED e, em seguida, para o TagoIO. Você pode visualizar e analisar esses dados através do seu dashboard personalizado no TagoIO.



