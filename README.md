# MemHero: EXPROM 2025 Edition

![Estado del Proyecto](https://img.shields.io/badge/Estado-Terminado-success)
![Licencia](https://img.shields.io/badge/Licencia-MIT-blue)
![Tech](https://img.shields.io/badge/HTML5-TailwindCSS-00f3ff)

> El desafio definitivo de Administracion de Memoria.
> Una experiencia arcade de ritmo para aprender Sistemas Operativos al estilo Cyberpunk.

---

## Descripcion

MemHero es un simulador interactivo y educativo desarrollado para la EXPROM 2025. Gamifica conceptos complejos de la gestion de memoria en Sistemas Operativos (especificamente la Paginacion de Memoria Virtual), transformando la teoria en un desafio de velocidad y precision.

El jugador asume el rol del Kernel (Nucleo) del sistema y debe gestionar las solicitudes de paginas (notas musicales) que caen hacia la CPU, decidiendo en milisegundos si realizar una carga, un acierto (hit) o un reemplazo de victima segun el algoritmo seleccionado.

## Caracteristicas Principales

* **Motor Velocity:** El juego aumenta de velocidad progresivamente. Un solo error destruye la pagina (Muerte Subita).
* **3 Modos de Algoritmo:**
    * **FIFO (First-In, First-Out):** Reemplaza la pagina mas antigua.
    * **LRU (Least Recently Used):** Reemplaza la pagina menos usada recientemente.
    * **OPT (Optimo):** Algoritmo teorico que mira al futuro para decidir.
* **Estetica Cyberpunk/Synthwave:** Interfaz inmersiva con fondo animado, horizonte de neon y efectos visuales reactivos.
* **Audio Sintetizado:** Efectos de sonido de 8-bits generados en tiempo real mediante Web Audio API (sin archivos externos).
* **Diseno Hibrido:** Totalmente jugable en Escritorio (Teclado/Mouse) y Moviles (Tactil).
* **Sistema de Pausa Completo:** Menu de pausa accesible para reanudar o abandonar la partida.

## Controles

El juego detecta automaticamente el dispositivo:

| Accion | Teclado (Opcion A) | Teclado (Opcion B) | Movil / Mouse |
| :--- | :---: | :---: | :---: |
| Marco 0 (Izq) | 1 | A | Toque / Clic |
| Marco 1 (Centro)| 2 | S | Toque / Clic |
| Marco 2 (Der) | 3 | D | Toque / Clic |
| Pausar | P o ESC | P o ESC | Boton [P] |
| Menu / Nav | Flechas / Enter | W / S / Enter | Tactil |

## Instalacion y Uso

Este proyecto es una Single Page Application (SPA) contenida en un solo archivo HTML, por lo que no requiere instalacion de dependencias de Node.js ni servidores complejos.

### Opcion 1: Ejecucion Directa
1.  Clona este repositorio o descarga el archivo .html.
2.  Abre el archivo index.html (o el nombre que le hayas dado) en cualquier navegador moderno (Chrome, Firefox, Edge, Safari).
3.  Juega.

### Opcion 2: GitHub Pages (Recomendado)
1.  Ve a la pestana Settings de tu repositorio.
2.  Entra en la seccion Pages.
3.  En Source, selecciona la rama main (o master).
4.  Tu juego estara disponible online en minutos.

## Tecnologias Utilizadas

* **HTML5 Semantico:** Estructura del juego.
* **CSS3 & Tailwind CSS (CDN):** Estilizado rapido, animaciones (keyframes), diseno responsivo y efectos de neon (box-shadow, text-shadow).
* **Vanilla JavaScript (ES6+):**
    * Logica del Game Loop (requestAnimationFrame).
    * Manipulacion del DOM.
    * Web Audio API para sintesis de sonido.
    * Gestion de eventos (Touch, Keyboard, Mouse).

## Conceptos Academicos Abordados

Este proyecto sirve como herramienta didactica para visualizar:
1.  **Fallos de Pagina (Page Faults):** Cuando ocurren y como se manejan.
2.  **Working Set:** Gestion de los marcos limitados en memoria fisica.
3.  **Localidad de Referencia:** Simulacion de patrones de acceso a memoria.
4.  **Overhead:** El costo de tomar decisiones de reemplazo.
5.  **Thrashing (Hiperpaginacion):** Visualizacion del colapso del sistema cuando la velocidad de fallos supera la capacidad de procesamiento (representado por el Game Over).

## Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar el codigo, anadir nuevos algoritmos (como Second Chance o Clock) o mejorar los graficos:

1.  Haz un Fork del proyecto.
2.  Crea una rama para tu Feature (git checkout -b feature/NuevaCaracteristica).
3.  Haz Commit (git commit -m 'Add: Nueva caracteristica').
4.  Haz Push (git push origin feature/NuevaCaracteristica).
5.  Abre un Pull Request.

## Licencia

Este proyecto esta bajo la Licencia MIT - ver el archivo LICENSE para mas detalles.

---
**Desarrollado para la EXPROM 2025**
