# 🧟 Apocalipsis Zombie

Un juego de acción 2D desarrollado con **Pygame Zero** en el que controlas a Eireen, una heroína que debe sobrevivir a oleadas de zombis en un escenario apocalíptico.

---

## 🎮 Descripción

Eireen debe defenderse de zombis que aparecen desde ambos lados de la pantalla. Dispara proyectiles, esquiva enemigos, recoge corazones y sube de nivel para aumentar tu poder de ataque. ¡Sobrevive el mayor tiempo posible y acumula el mayor puntaje!

---

## 🕹️ Controles

| Acción       | Tecla / Botón              |
|--------------|----------------------------|
| Mover izquierda | ← o `A`                |
| Mover derecha   | → o `D`                |
| Saltar          | `Espacio`, ↑ o `W`     |
| Disparar        | Clic izquierdo del ratón |

---

## ⚙️ Mecánicas del juego

- **Enemigos:** Los zombis aparecen cada 4 segundos desde la izquierda o derecha de la pantalla con movimiento tambaleante (pausas aleatorias).
- **Vida de zombis:** A partir de cierto puntaje, los zombis tienen más vida y pueden requerir varios disparos.
- **Corazones:** Algunos zombis eliminados dejan caer un corazón que recupera 1 punto de vida de Eireen.
- **Niveles:** Cada vez que eliminas suficientes zombis, subes de nivel. A partir del nivel 5, aumenta tu poder de ataque.
- **Game Over:** El juego termina cuando Eireen pierde toda su vida al colisionar con los enemigos.

---

## 📊 HUD (Interfaz en pantalla)

| Elemento  | Descripción                        |
|-----------|------------------------------------|
| Puntaje   | Número de zombis eliminados        |
| Vida      | Puntos de vida actuales de Eireen  |
| Nivel     | Nivel actual del jugador           |

---

## 🗂️ Estructura del proyecto

```
click-al-gato/
│
├── main.py               # Código principal del juego
├── images/               # Sprites y fondos
│   ├── apocalipsis.png
│   ├── parada_derecha.png
│   ├── parada_izquierda.png
│   ├── correr_derecha.png
│   ├── correr_izquierda.png
│   ├── atacando_derecha.png
│   ├── atacando_izquierda.png
│   ├── bola_ataque.png
│   ├── zombie1.png / zombie2.png / zombie3.png
│   ├── zombie1_izquierda.png / zombie2_izquierda.png / zombie3_izquierda.png
│   ├── explosion.png
│   └── heart.png
└── README.md
```

---

## 🛠️ Requisitos

- Python 3.7+
- [Pygame Zero](https://pygame-zero.readthedocs.io/)

### Instalación

```bash
pip install pgzero
```

### Ejecución

```bash
pgzrun main.py
```

---

## 📈 Progresión de dificultad

| Condición             | Efecto                                      |
|-----------------------|---------------------------------------------|
| Puntaje ≥ 5           | Zombis comienzan a tener más vida (1–8)     |
| Puntaje ≥ 20          | Zombis tienen hasta 15 puntos de vida       |
| Puntaje ≥ 7           | Los zombis pueden soltar corazones al morir |
| Cada `meta` zombis eliminados | Sube de nivel (+3 a la meta)        |
| Nivel ≥ 5 (`poder`)   | Aumenta el ataque de Eireen                 |

---

## 👩‍💻 Créditos

Desarrollado con Pygame Zero. Personaje principal: **Eireen**.
