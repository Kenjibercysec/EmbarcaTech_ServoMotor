# EmbarcaTech Servo Motor Project

Este projeto controla um servo motor usando a placa Raspberry Pi Pico W.

## Descrição

O código neste repositório permite controlar um servo motor conectado ao pino GPIO 28 da Raspberry Pi Pico W. O servo motor pode ser movido para diferentes posições (0, 90 e 180 graus) e também pode realizar uma movimentação suave entre essas posições.

## Arquivos

- `ServoMotor.c`: Contém o código fonte principal para controlar o servo motor.
- `CMakeLists.txt`: Arquivo de configuração do CMake para compilar o projeto.

## Dependências

- Raspberry Pi Pico SDK
- Biblioteca `hardware_pwm` do Pico SDK
- Biblioteca `pico_stdlib` do Pico SDK
- Biblioteca `pico_time` do Pico SDK

## Compilação e Execução

1. Certifique-se de que o Raspberry Pi Pico SDK está instalado e configurado corretamente.
2. Clone este repositório.
3. Navegue até o diretório do projeto.
4. Execute os seguintes comandos para compilar e carregar o código na Raspberry Pi Pico W:

```sh
mkdir build
cd build
cmake ..
ninja
```

5. Carregue o arquivo binário gerado na Raspberry Pi Pico W.

## Uso

Após carregar o código na Raspberry Pi Pico W, o servo motor será inicializado e se moverá para as posições 180, 90 e 0 graus, com uma pausa de 5 segundos entre cada movimento. Em seguida, o servo motor realizará uma movimentação suave entre as posições 0 e 180 graus continuamente.

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
