# Projeto Display - Raspberry Pi Pico  
Este projeto foi desenvolvido por **Kalel Ezveither** e tem como objetivo controlar um **display OLED SSD1306** e uma **matriz de LEDs WS2812**, além de processar eventos de botões e entrada serial na **Raspberry Pi Pico**.

##  Funcionalidades
- Exibe números (0-9) na matriz de LEDs WS2812.
- Exibe caracteres (A-Z, a-z) no display OLED SSD1306.
- Processa eventos de botões (Botão A e Botão B) para alternar LEDs RGB e exibir o estado no display.
- Lida corretamente com o buffer serial para evitar atrasos ou necessidade de envio duplo.

##  Tecnologias Utilizadas
- **C/C++** para programação embarcada.
- **Pico SDK** para desenvolvimento na Raspberry Pi Pico.
- **I2C** para comunicação com o display OLED SSD1306.
- **PIO e DMA** para controle eficiente da matriz WS2812.

##  Autor
- **Kalel Ezveither**

## Vídeo de teste 
https://drive.google.com/file/d/1Pa0sIWiDVlHjdg634fzXcxU1r7-KiNwS/view?usp=sharing

https://drive.google.com/file/d/1Pa0sIWiDVlHjdg634fzXcxU1r7-KiNwS/view?usp=sharing
