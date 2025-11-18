# 🧩 Cáliz de Fuego – Nand2Tetris 

**Cáliz de Fuego** es un proyecto desarrollado en el lenguaje **Jack** del curso **Nand2Tetris**, basado parcialmente en la película *Harry Potter y el Cáliz de Fuego* —específicamente en la tercera prueba del Torneo de los Tres Magos— y utilizando como base el repositorio original *MazeEscaper* de **hbusul**.

Repositorio original de referencia:  
[GitHub – hbusul](https://github.com/hbusul/MazeEscaper)

---

## 🎥 Video explicativo
https://youtu.be/DNFeIoZ0-ew?si=PTNjIVdQRo2D2tOb

---

## 📘 Descripción General

Cáliz de Fuego es un juego tipo laberinto donde el jugador navega a través de un mapa, evitando obstáculos y buscando la meta.

Este proyecto está construido completamente en **Jack** e implementa:

- Lógica de movimiento del jugador  
- Ciclo de actualización y renderizado  
- Detección de obstáculos  
- Control por teclado  
- Dibujado con la API nativa `Screen`  

---

## 📁 Estructura del Proyecto

<pre>
Caliz-de-Fuego---Nand2Tetris/
│── src/
│  ├── ExtendedMath.jack 
│  ├── Main.jack 
│  ├── MazeDrawer.jack 
│  ├── MazeGenerator.jack
│  ├── Obstacles.jack 
│  ├── Player.jack 
│  ├── PlayerController.jack 
│  ├── PlayHelper.jack 
│  ├── PseudoRand.jack 
│  └── Questions.jack 
└── README.md
</pre>

### 📄 Descripción de archivos

- **Main.jack**: Coordina todo el juego: inicializa el laberinto, los obstáculos, el generador aleatorio, el jugador y el controlador. También muestra las instrucciones y presenta el resultado final.
- **ExtendedMath.jack**: Proporciona funciones matemáticas adicionales necesarias para otros módulos, como cálculos de potencia.
- **MazeGenerator.jack**: Genera la estructura lógica del laberinto usando un algoritmo aleatorio basado en backtracking.
- **MazeDrawer.jack**: Dibuja el laberinto en pantalla a partir de la información generada por `MazeGenerator`.
- **Obstacles.jack**: Crea y gestiona los obstáculos dentro del laberinto y los coloca en posiciones aleatorias.
- **Player.jack**: Define al jugador, su posición y sus movimientos dentro del laberinto.
- **PlayerController.jack**: Controla la interacción del jugador: lectura del teclado, movimientos, detección de colisiones, puntaje y llegada a la meta.
- **PlayHelper.jack**: Dibuja el panel lateral con controles, instrucciones básicas y la sección visual del puntaje.
- **PseudoRand.jack**: Generador de números pseudoaleatorios utilizado para construir el laberinto, seleccionar obstáculos y manejar aspectos aleatorios del juego.
- **Questions.jack**: Administra el sistema de preguntas: elige preguntas aleatorias, muestra opciones y evalúa las respuestas del jugador.


---

## ▶️ Ejecución del Juego

### 1️⃣ Compilación
- Abre el [software de Nand2Tetris](https://nand2tetris.github.io/web-ide/compiler)
- Verifica estar en la sección `<> jack compiler`
- Carga la carpeta con los archivos `.jack`
- Presiona `Compile` y luego `Run`

### 2️⃣ En el `VM Emulator`
- Verifica que la velocidad de ejecución esté en `Fast`
- Presiona el botón ⏩ (junto a la velocidad)
- Habilita la opción del teclado para poder jugar

---

## 📝 Créditos

Este proyecto toma como referencia conceptual el repositorio:  
https://github.com/hbusul/MazeEscaper

---

## 📜 Licencia – EAFIT (Uso Académico)

Este proyecto es de código abierto y fue desarrollado con fines educativos como parte del curso de Organización de Computadores de la Universidad EAFIT.
