# Plan de Desarrollo: Página Interactiva de Cumpleaños para Roxana 🎉

Este documento describe la propuesta y el plan técnico para arreglar y potenciar la página de cumpleaños de **Roxana**, creada con cariño por **Genesis**.

---

## 1. Diagnóstico del Estado Actual

1. **Codificación de caracteres (Encoding)**:
   - El archivo actual presenta caracteres extraños (`` y `??`) en títulos, tildes, la letra 'ñ' y emojis.
2. **Las 10 Fotos de recuerdos en la carpeta**:
   - Hay 10 imágenes en formato JPEG listas en la carpeta, pero actualmente no se muestran de forma predeterminada (el usuario tendría que seleccionarlas manualmente cada vez).
3. **Música de fondo (Tokyo Drift)**:
   - La canción `ytmp3free.cc_tokyo-drift-traduccion-al-espaol-rapidos-y-furiosos-reto-tokyo-youtubemp3free.org.mp3` está en la carpeta pero no está conectada automáticamente.
   - Además, las políticas de seguridad de los navegadores modernos impiden que el audio empiece a sonar solo ("autoplay") sin que el usuario haga clic primero en la pantalla.
4. **Mensaje personal**:
   - Falta el texto final de dedicatoria para Roxana.

---

## 2. Propuesta de Mejoras e Interactividad

### A. Pantalla de Inicio / Bienvenida (Splash Screen) ✨
- Para que la música comience a sonar automáticamente en segundo plano sin violar las políticas del navegador, crearemos una pantalla de bienvenida animada:
  - Mensaje introductorio: *"Una sorpresa especial para Roxana ✨"*.
  - Botón interactivo central con animación brillante: *"Toca para comenzar 🎁"* o *"Iniciar sorpresa 🎵"*.
  - Al presionarlo:
    - Comienza a sonar la música de fondo (Tokyo Drift) de inmediato.
    - Se activa una lluvia festiva de confeti y corazones.
    - La pantalla de bienvenida se desvanece suavemente dando paso a la página principal.

### B. Galería Interactiva con las 10 Fotos 📸
- Las 10 fotos de la carpeta se cargarán automáticamente en un diseño de tarjetas moderno y estético.
- **Visor en pantalla completa (Lightbox)**:
  - Al hacer clic en cualquier foto, se abrirá en grande con fondo desenfocado.
  - Flechas de navegación: **Anterior (◀)** y **Siguiente (▶)**.
  - Contador: *"Foto X de 10"*.
  - Compatible con gestos en celular (deslizar) y con teclado (flechas y tecla Esc).

### C. Música de Fondo y Controles 🎵
- Vinculación directa al archivo de audio local.
- Botón flotante discreto en la esquina de la pantalla para pausar/reanudar la música en cualquier momento.
- Efecto de vinilo girando en la sección de música cuando la canción esté sonando.

### D. Restauración de Textos y Emojis 🍣🎬
- Restauración limpia en codificación UTF-8 de todas las secciones:
  - *Sushi* 🍣
  - *Películas* 🎬🍿
  - *Paintball* 🎯💥
  - *Lugares de juegos* 🕹️👾
  - *Y mucho más* ✨💖
  - Planes futuros: *Patinaje sobre hielo* ⛸️, *Carritos chocones de Scala Shopping* 🏎️, *Mariscos* 🦐.

### E. Carta / Mensaje Interactivo 💌
- La sección de mensaje tendrá un diseño de sobre o tarjeta que se puede abrir con un toque para revelar la dedicatoria especial.

---

## 3. Plan de Pasos a Seguir

1. **Respaldo de seguridad**: Guardar una copia intacta del archivo original.
2. **Generación del archivo principal `index.html`**: Con estructura HTML5 semántica y codificación UTF-8 pura.
3. **Integración de la pantalla de bienvenida y disparador de audio**: Con transiciones fluidas en CSS.
4. **Montaje de la galería con las 10 fotos y visor lightbox**.
5. **Configuración de audio de fondo Tokyo Drift con controles interactivos**.
6. **Revisión responsive**: Garantizar que se vea y funcione a la perfección en teléfonos móviles y computadoras.
