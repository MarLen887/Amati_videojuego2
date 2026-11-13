# Amati corre

Videojuego *runner* **en 3D real** de tres carriles (estilo Subway Surfers) en un solo archivo, sin dependencias externas (motor WebGL propio). Requiere un navegador con WebGL.
Amati corre, atrapa **tarjetas** de colores (sin nombres) en lugar de monedas y esquiva distracciones. **Sable**, la policía, la persigue. Amati es un colibrí zoomorfo con alas que aletean; Sable corre con brazos y piernas animados.

## Cómo se juega

- **Carriles:** ← → (o A / D). **Saltar:** ↑ o Espacio. **Deslizar:** ↓. **Pausa:** P o Esc. **Sonido:** M.
- **Táctil:** desliza el dedo en cualquier dirección. **Control:** stick o cruceta, A para empezar, Start para pausar.
- **Obstáculos:** bloques bajos (se saltan), pancartas de notificaciones (se pasan deslizando) y bloques altos (se esquivan cambiando de carril).
- **Sable:** el primer choque la acerca durante 9 segundos y rompe tu combo. Un segundo choque en ese lapso, y te atrapa (fin de la partida). Si aguantas sin chocar, se aleja.
- **Poderes:** Pomodoro (escudo contra un choque), Feynman (puntos dobles, 8 s) y Respiración (todo más lento, 6 s).
- **Combo:** cada 4 tarjetas seguidas sube el multiplicador, hasta x5. Un choque lo reinicia.

- **Niveles:** cada 18 s sube el nivel: más velocidad, más obstáculos, filas dobles y Sable te sigue durante menos tiempo. El cielo cambia (día, atardecer, noche, neón). La partida termina cuando Sable te atrapa.

## Abrirlo

- **Local:** abre `index.html` en Chrome, Edge o Firefox.
- **GitHub Pages:** sube la carpeta al repositorio, ve a *Settings → Pages → Deploy from a branch → `main` / `(root)`* y abre `https://<usuario>.github.io/<repositorio>/`.

## Archivos

```
index.html        Juego completo (HTML + CSS + JavaScript)
assets/amati-logo.jpg  Logo de Amati (pantalla de inicio; opcional)
assets/sable.png       Imagen de Sable (pantalla de inicio y emblema; opcional)
.nojekyll         Evita el procesamiento de Jekyll en GitHub Pages
```

## Personalización

`CARD_COLS` define los colores de las tarjetas, `THEMES` los cielos por nivel y `SAY_*` las frases de Sable.
Los personajes 3D se construyen con piezas procedimentales. La música y los sonidos se sintetizan con Web Audio; no hay archivos de audio. El juego no recopila datos ni usa servidor; solo guarda en el dispositivo la mejor puntuación y la preferencia de sonido.
