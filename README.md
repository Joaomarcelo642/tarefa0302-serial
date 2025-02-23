# Tarefa 01 - 03/02: Introdução às Interfaces de Comunicação Serial com RP2040 UART, SPI e I2C

Este projeto implementa um sistema de controle utilizando o Raspberry Pi Pico, um display OLED SSD1306 via I2C, botões físicos e uma matriz de LEDs WS2812 para exibição de números.

## 📌 Funcionalidades

- Exibição de caracteres no display OLED SSD1306
- Exibição de números na matriz de LEDs WS2812
- Controle de LEDs RGB via botões físicos
- Comunicação serial para entrada de caracteres e números
- Utilização de interrupções para os botões
- Uso de DMA para controle eficiente da matriz WS2812

## 🛠️ Hardware Utilizado

- Raspberry Pi Pico
- Display OLED SSD1306 (I2C)
- Matriz de LEDs WS2812 (25 LEDs)
- Botões físicos (BUTTON_A e BUTTON_B)
- LEDs RGB individuais (Verde e Azul)

## 📌 Mapeamento de Pinos

| Componente | Pino no Pico |
|------------|-------------|
| SDA (I2C)  | 14 |
| SCL (I2C)  | 15 |
| WS2812 Data | 7 |
| Botão A | 5 |
| Botão B | 6 |
| LED Verde | 11 |
| LED Azul | 12 |

## 📜 Dependências

Para compilar e rodar o código, certifique-se de ter as seguintes bibliotecas instaladas:

- **Pico SDK**
- **ssd1306.h** (Driver para o display OLED)
- **font.h** (Fonte para renderização no OLED)
- **matrizNumero.h** (Mapeamento de números para exibição na matriz de LEDs)
- **ws2812.pio.h** (Código PIO para controle dos LEDs WS2812)

## 🚀 Como Compilar e Executar

1. Configure o ambiente do **Pico SDK**
2. Compile o código utilizando **CMake**
3. Faça o upload do arquivo `.uf2` gerado para o Raspberry Pi Pico
4. Conecte ao dispositivo via porta serial para enviar comandos

## 🎮 Como Usar

- Envie um número (0-9) pela comunicação serial para exibi-lo na matriz de LEDs
- Envie uma letra (A-Z ou a-z) para exibi-la no display OLED
- Pressione o **Botão A** para alternar o LED Verde
- Pressione o **Botão B** para alternar o LED Azul

## 📌 Observações

- O código implementa debounce por software para os botões físicos
- A matriz de LEDs WS2812 é controlada via PIO e DMA para melhor desempenho
- A comunicação serial é usada para entrada de caracteres e números

## Vídeo de Demonstração

https://drive.google.com/file/d/10XH5XrXxgB5asDL3w93pSs08eCaPqYO0/view?usp=drive_link

---

🔧 **Desenvolvido para fins acadêmicos e experimentação com sistemas embarcados.**


