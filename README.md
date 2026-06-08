
# Internet das Coisas (IoT) e Arduino
## Conteúdo Teórico e Prático

---

# 1. Introdução à Internet das Coisas (IoT)

A **Internet das Coisas (Internet of Things - IoT)** é um conceito tecnológico que permite que objetos físicos sejam conectados à internet para coletar, compartilhar e processar dados automaticamente.

Esses dispositivos podem incluir:

- Sensores
- Câmeras
- Lâmpadas inteligentes
- Geladeiras inteligentes
- Relógios inteligentes
- Veículos conectados
- Equipamentos industriais

O principal objetivo da IoT é tornar processos mais eficientes, automatizados e inteligentes.

---

# 2. Conceitos Fundamentais

## Conectividade

Capacidade de dispositivos se conectarem à internet ou redes locais.

## Sensoriamento

Uso de sensores para coletar informações do ambiente.

### Exemplos

- Temperatura
- Umidade
- Luminosidade
- Movimento
- Distância

## Processamento

Transformação dos dados coletados em informações úteis.

## Automação

Tomada de decisões sem intervenção humana.

### Exemplo

Se a temperatura ultrapassar **30°C**, um ventilador pode ser ligado automaticamente.

---

# 3. Componentes de um Sistema IoT

## Sensores

Responsáveis pela coleta dos dados.

### Exemplos

- DHT11 (temperatura e umidade)
- HC-SR04 (distância)
- LDR (luminosidade)
- MQ-2 (gás e fumaça)

## Microcontrolador

Responsável pelo processamento.

### Exemplos

- Arduino Uno
- ESP32
- ESP8266

## Rede de Comunicação

Permite envio dos dados.

### Tecnologias

- Wi-Fi
- Bluetooth
- ZigBee

## Plataforma de Dados

Recebe, armazena e analisa informações.

### Exemplos

- ThingSpeak
- Blynk
- Arduino Cloud

---

# 4. Aplicações da IoT

## Casas Inteligentes

- Controle de iluminação
- Controle de temperatura
- Segurança residencial

## Indústria 4.0

- Monitoramento de máquinas
- Manutenção preditiva
- Controle de produção

## Cidades Inteligentes

- Controle de trânsito
- Monitoramento ambiental
- Gestão de energia

---

# 5. Vantagens e Desafios da IoT

## Vantagens

- Automação de processos
- Economia de recursos
- Maior eficiência
- Monitoramento remoto
- Tomada de decisões baseada em dados

## Desafios

- Segurança
- Privacidade
- Custos de implementação
- Dependência da internet
- Compatibilidade entre dispositivos

---

# 6. Introdução ao Arduino

O **Arduino** é uma plataforma de prototipagem eletrônica de código aberto utilizada para criar projetos de automação, robótica e Internet das Coisas.

É composta por:

- Hardware (placa física)
- Software (IDE Arduino)

---

# 7. Estrutura de um Arduino

## Microcontrolador

Executa o programa armazenado na placa.

## Pinos Digitais

Trabalham com dois estados:

- HIGH (1)
- LOW (0)

## Pinos Analógicos

Permitem leitura de sinais variáveis.

### Exemplo

Valores entre:

```text
0 até 1023
```

## Porta USB

Utilizada para:

- Programação
- Alimentação elétrica

---

# 8. Programação Básica

Todo programa Arduino possui duas funções principais.

## Setup

Executada apenas uma vez.

```cpp
void setup() {

}
```

## Loop

Executada continuamente.

```cpp
void loop() {

}
```

### Exemplo: Piscar LED

```cpp
void setup() {
  pinMode(13, OUTPUT);
}

void loop() {
  digitalWrite(13, HIGH);
  delay(1000);

  digitalWrite(13, LOW);
  delay(1000);
}
```

---

# 9. Sensores e Atuadores

## Sensores

Coletam informações do ambiente.

| Sensor | Função |
|----------|---------|
| DHT11 | Temperatura e Umidade |
| LDR | Luminosidade |
| HC-SR04 | Distância |
| MQ-2 | Detecção de Gases |

---

## Atuadores

Executam ações físicas.

| Atuador | Função |
|----------|---------|
| LED | Iluminação |
| Motor DC | Movimento |
| Servo Motor | Controle Angular |
| Buzzer | Emissão de Som |

---

# 10. Projetos Práticos com Arduino

## Projeto 1 – Semáforo Inteligente

### Componentes

- Arduino Uno
- 3 LEDs
- Resistores


---

# 11. Integração Arduino + IoT

Para conectar projetos à internet normalmente utiliza-se:

## ESP8266

Módulo com conectividade Wi-Fi.

## ESP32

Microcontrolador que possui:

- Wi-Fi integrado
- Bluetooth integrado
- Maior capacidade de processamento

### Fluxo de Funcionamento

```text
Sensor
   ↓
Arduino / ESP32
   ↓
Internet
   ↓
Plataforma IoT
   ↓
Usuário
```

---

# 12. Exemplo de plataforma IoT


## Arduino Cloud

Permite:

- Monitoramento remoto
- Criação de painéis
- Controle de dispositivos

---

# 13. Segurança em IoT

## Principais Riscos

- Vazamento de dados
- Invasões
- Roubo de informações
- Ataques cibernéticos


---

# 14. Comunicação e Relação de Dados na IoT

## Como os Dados Circulam na IoT

A comunicação na Internet das Coisas ocorre através de um fluxo contínuo de coleta, transmissão, processamento e utilização de dados.

```text
Ambiente
   ↓
Sensor
   ↓
Microcontrolador
   ↓
Rede de Comunicação
   ↓
Servidor/Nuvem
   ↓
Aplicação
   ↓
Usuário
```

---

## Etapa 1 – Coleta de Dados

Os sensores capturam informações do ambiente.

---

## Etapa 2 – Processamento Local

O microcontrolador recebe os dados e pode tomar decisões.

```cpp
if (temperatura > 30) {
   ligarVentilador();
}

---

## Etapa 3 – Transmissão dos Dados

Os dados são enviados por meio de:

- Wi-Fi
- Bluetooth
- Ethernet
- LoRa
- ZigBee


---

## Etapa 4 – Armazenamento

Os dados são armazenados em:

- Bancos de dados
- Servidores
- Plataformas IoT

### Objetivos

- Histórico
- Relatórios
- Monitoramento
- Auditoria

---

## Etapa 5 – Análise dos Dados

Os dados armazenados podem gerar:

- Gráficos
- Alertas
- Relatórios
- Automações

### Exemplo

```text
Temperatura > 35°C
        ↓
Enviar alerta
        ↓
Ligar ventilador
```

---

## Comunicação Entre Dispositivos

Nem toda comunicação ocorre pela internet.

Os dispositivos podem se comunicar diretamente.

### Exemplo

```text
Sensor de Presença
        ↓
ESP32
        ↓
Lâmpada Inteligente
        ↓
Acender
```

---

## Protocolos de Comunicação

### MQTT

Características:

- Leve
- Rápido
- Pouco consumo de energia
- Muito utilizado em IoT

Modelo:

```text
Publicador
     ↓
Broker MQTT
     ↓
Assinante
```

---

### HTTP

Muito utilizado para integração com páginas web e APIs.

```text
ESP32
  ↓
Servidor Web
```

---

### CoAP

Protocolo otimizado para dispositivos com poucos recursos de processamento e energia.

---

## Relação Entre os Dados na IoT

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
 ↓
Nova Coleta
```

Esse ciclo cria sistemas inteligentes capazes de monitorar, analisar e automatizar tarefas continuamente.


````
