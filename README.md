# Amati corre

Videojuego tipo *runner* de tres carriles (estilo Subway Surfers) en un solo archivo, sin dependencias.
Amati corre, atrapa **técnicas** y **herramientas** de estudio en lugar de monedas y esquiva distracciones. **Sable**, la policía, la persigue.

## Cómo se juega

- **Carriles:** ← → (o A / D). **Saltar:** ↑ o Espacio. **Deslizar:** ↓. **Pausa:** P o Esc. **Sonido:** M.
- **Táctil:** desliza el dedo en cualquier dirección. **Control:** stick o cruceta, A para empezar, Start para pausar.
- **Obstáculos:** bloques bajos (se saltan), pancartas de notificaciones (se pasan deslizando) y bloques altos (se esquivan cambiando de carril).
- **Sable:** el primer choque la acerca durante 9 segundos y rompe tu combo. Un segundo choque en ese lapso, y te atrapa (fin de la partida). Si aguantas sin chocar, se aleja.
- **Poderes:** Pomodoro (escudo contra un choque), Feynman (puntos dobles, 8 s) y Respiración (todo más lento, 6 s).
- **Combo:** cada 4 tarjetas seguidas sube el multiplicador, hasta x5. Un choque lo reinicia.

## Abrirlo

- **Local:** abre `index.html` en Chrome, Edge o Firefox.
- **GitHub Pages:** sube la carpeta al repositorio, ve a *Settings → Pages → Deploy from a branch → `main` / `(root)`* y abre `https://<usuario>.github.io/<repositorio>/`.

## Archivos

```
index.html        Juego completo (HTML + CSS + JavaScript)
assets/amati.png  Imagen de Amati (opcional; si falta, se dibuja en el lienzo)
assets/sable.png  Imagen de Sable (opcional; si falta, se dibuja en el lienzo)
.nojekyll         Evita el procesamiento de Jekyll en GitHub Pages
```

## Personalización

Las listas `TECH` y `TOOLS` (inicio del `<script>`) contienen los nombres de las tarjetas, y `SAY_*` las frases de Sable. Cambia los nombres por los del repositorio de Amati si es necesario.
La música y los sonidos se sintetizan con Web Audio; no hay archivos de audio. El juego no recopila datos ni usa servidor; solo guarda en el dispositivo la mejor puntuación y la preferencia de sonido.
