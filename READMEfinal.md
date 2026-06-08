# Comunicação e Relação de Dados na Internet das Coisas (IoT)

## Introdução

A Internet das Coisas (IoT) permite que dispositivos físicos conectados à internet coletem, compartilhem e utilizem dados para monitoramento e automação de processos.

A comunicação entre dispositivos é essencial para que as informações sejam transmitidas, processadas e transformadas em ações inteligentes.

---

# Como Funciona a Comunicação na IoT

O fluxo de comunicação em um sistema IoT geralmente ocorre da seguinte forma:

```text
Ambiente
   ↓
Sensor
   ↓
Microcontrolador
   ↓
Internet/Rede
   ↓
Servidor ou Nuvem
   ↓
Aplicação
   ↓
Usuário
```

---

# Etapas da Comunicação

## 1. Coleta de Dados

Os sensores capturam informações do ambiente.

### Exemplos

- Temperatura
- Umidade
- Luminosidade
- Distância
- Presença

Exemplo:

```text
Temperatura = 27°C
Umidade = 65%
```

---

## 2. Processamento

O microcontrolador (Arduino ou ESP32) recebe os dados e pode realizar cálculos ou tomar decisões.

Exemplo:

```cpp
if (temperatura > 30) {
   ligarVentilador();
}
```

---

## 3. Transmissão

Os dados são enviados por tecnologias como:

- Wi-Fi
- Bluetooth
- Ethernet
- LoRaWAN
- ZigBee

Exemplo:

```text
Sensor
  ↓
ESP32
  ↓
Wi-Fi
  ↓
Nuvem
```

---

## 4. Armazenamento e Análise

Os dados são armazenados em plataformas IoT, onde podem ser analisados e transformados em gráficos, relatórios ou alertas.

Exemplos de plataformas:

- Arduino Cloud
- ThingSpeak
- Blynk

---

# Protocolos de Comunicação

## MQTT

Protocolo leve e muito utilizado em IoT.

```text
Publicador
    ↓
Broker
    ↓
Assinante
```

## HTTP

Utilizado para comunicação com páginas web e servidores.

## CoAP

Protocolo otimizado para dispositivos com poucos recursos.

---

# Relação dos Dados na IoT

Os dados seguem um ciclo contínuo:

```text
Coleta
 ↓
Transmissão
 ↓
Armazenamento
 ↓
Processamento
 ↓
Decisão
 ↓
Ação
```

Exemplo:

```text
Sensor detecta solo seco
          ↓
Sistema processa informação
          ↓
Irrigação é acionada
```

---

