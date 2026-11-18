# Cómo presentar el Taller 2 con el guion en el Mac

La presentación va al proyector y el guion queda en la pantalla del Mac. Las dos ventanas están sincronizadas: desde el guion se cambian las láminas del proyector.

## Montaje

1. Conecta el proyector y deja las pantallas **extendidas**, no duplicadas (Ajustes del Sistema → Pantallas → «Extender»).
2. En la Terminal, levanta el servidor:

   ```bash
   cd ~/UNAB/Talleres-Infraestructura-TI/"Taller 2" && python3 -m http.server 8800
   ```

3. En Chrome, abre `http://localhost:8800/Entrega2_GRUPO6_NRC8485.html`, **arrastra esa ventana al proyector**, haz clic en ella y presiona `F` para pantalla completa.
4. En otra ventana de Chrome, en el Mac, abre `http://localhost:8800/presentador.html` y ponla en pantalla completa con `Ctrl + Cmd + F`.
5. **Haz clic una vez en la ventana del guion** para que reciba el teclado. Desde ahí manejas todo.

El punto verde arriba a la izquierda del guion indica que está conectado con la presentación.

## Teclas (en la ventana del guion)

| Tecla | Qué hace |
|---|---|
| `→` | Siguiente lámina en el proyector |
| `←` | Lámina anterior |
| Espacio | Inicia o pausa el cronómetro |
| `R` | Reinicia el cronómetro |
| `+` / `−` | Agranda o achica el texto del guion |

El guion muestra quién habla, el tramo de tiempo de la lámina, el texto, la lámina en pantalla y la siguiente. Cuando la siguiente la presenta otra persona, lo avisa en amarillo. El cronómetro dice si van adelantados o atrasados según el tramo de cada lámina, y se pone amarillo a los 9 minutos y rojo a los 10.

## Reparto (Martín no presenta)

| Integrante | Láminas | Tiempo |
|---|---|---|
| Benjamín | 1–2 y 11 | 0:00–1:30 y 9:30–10:00 |
| Francisco | 3–5 (servicios y costos) | 1:30–4:45 |
| Julián | 6–8 (sensibilidad, arquitectura y recomendación) | 4:45–7:30 |
| Matías | 9–10 (migración y riesgos) | 7:30–9:30 |

## Si algo falla

- **El guion no mueve el proyector:** usa las flechas haciendo clic en la ventana del proyector. La presentación funciona sola.
- **Las dos ventanas tienen que estar en el mismo Chrome** (no una en Safari y otra en Chrome).
- **El computador de la sala no es el tuyo:** usa `Entrega2_GRUPO6_NRC8485 - Presentacion.pdf` o abre el HTML desde un pendrive, y lleva el guion en PDF (hay versión con y sin Martín).
- Para detener el servidor: `Ctrl + C` en la Terminal.
