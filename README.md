Laberinto en RISC-V (Ripes)
CIIC 4081 
Autoras
Alanis Alvarado Gierbolini
Adriana Bonilla Romacho

Descripción del Proyecto
Este proyecto consiste en la implementación de un juego de laberinto utilizando ensamblador RISC-V (RV32I) en la plataforma Ripes.
El objetivo es controlar un pixel (jugador) dentro de una matriz de LED de 25x35 para navegar a través de un laberinto y alcanzar una salida, evitando colisiones con las paredes.

Funcionalidades
Dibujo del laberinto (25x35)
El laberinto se almacena en memoria como una matriz de caracteres (# y .) y se renderiza en la LED Matrix.
Jugador controlable
Representado por un pixel verde que inicia en la esquina superior izquierda.
Salida del laberinto
Representada por un pixel rojo en una posición específica.
Control con D-Pad
El movimiento del jugador se realiza mediante los botones direccionales del D-Pad en Ripes.
Detección de colisiones
El jugador no puede atravesar paredes.
Condición de victoria
Al llegar a la salida, toda la pantalla se pinta de color verde.

Requisitos
Ripes (versión desktop o web: https://ripes.me)
Activar los dispositivos:
LED Matrix
D-Pad

Instrucciones de Ejecución
Abrir Ripes
Ir a la pestaña Editor
Pegar el archivo laberinto.s
Hacer clic en Assemble 
Hacer clic en Run 
Utilizar el D-Pad (o teclado WASD) para mover el jugador

Notas Importantes
Las direcciones de memoria del D-Pad pueden variar según la configuración de Ripes.
Si la matriz no muestra el laberinto, puede ser necesario ajustar la dirección base del LED Matrix.

Conceptos Aplicados
Manejo de memoria en ensamblador
Subrutinas y uso de registros
Cálculo de offsets para acceso a matrices
Entrada/Salida mediante memoria mapeada (I/O)
Control de flujo y lógica de juego
