# script impreso() — Interfaz de papel (2025)

**QR Resma A4** es una obra-código abierta: un único archivo HTML que genera 500 páginas A4 (orientación horizontal), cada una impresa con códigos QR únicos.  
Cada QR enlaza a fragmentos de archivos audiovisuales, sesiones y publicaciones relacionadas con el ecosistema de **La Casa Mutante** (2020–2025).  

> El conjunto forma una interfaz física: una web expandida sobre papel.

---

## 🌐 Descripción

El archivo [`qr_print_a0.html`](./qr_print_a0.html) traduce un conjunto de URLs a un entorno físico, creando una “resma digital impresa”.  
Cada hoja contiene una cuadrícula de códigos QR dispuestos según patrones aleatorios (“grid”, “wave”, “edificios”, “disperso”), y una fracción de las páginas incluye cartela.

La pieza funciona simultáneamente como:
- **Script técnico** reproducible, basado en web estándar (HTML, CSS, JS puro).
- **Instalación artística** que transforma código en materia impresa.
- **Archivo colectivo** accesible mediante interacción humana (escaneo).

---

## ⚙️ ¿Cómo usar?

1. Abrir el archivo (`qr_print_a0.html`) en un navegador moderno, preferentemente Google Chrome.
2. Esperar a que se generen las 500 páginas (esto puede tardar).
3. Imprimir contenido generado (Ctrl + P) en **A4 horizontal (landscape)**, **escala 100%**, sin márgenes adicionales.
4. Cada página contendrá:
   - Una cuadrícula de códigos QR únicos (≈ 50 mm c/u).
   - Una banda inferior con información o texto poético.

### Parámetros principales

Los valores se definen en la hoja de estilo:

```css
--page-w-mm: 297;    /* ancho A4 landscape en mm */
--page-h-mm: 210;    /* alto A4 landscape en mm */
--pages-count: 500;  /* número de hojas (resma completa) */
--qr-mm: 50;         /* tamaño del QR en mm */
--band-fraction: 0.12; /* proporción de hojas con cartela */
