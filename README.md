# Casita Sebita 3D — Espacio Interactivo con Colisiones y Físicas (Three.js)

Proyecto web 3D interactivo generado a partir del modelo **`casitaSebita.skp`** (SketchUp 2024) y optimizado a **12.3 MB** (`casitaSebita.glb`) para ejecutarse directamente en **GitHub Pages** sin requerir Git LFS ni servidores externos.

## Características incluidas

- **Cámara en primera persona (`PointerLockControls` + Drag 360° + Soporte Móvil):** Camina con `W`, `A`, `S`, `D` o las flechas del teclado, corre con `Shift`, salta con `Espacio` y agáchate con `Ctrl`.
- **Motor espacial de colisiones exactas (Grid Espacial 2D + Cápsula multicapa contra triángulos reales):** Detecta paredes, desniveles, mesadas de cocina, alacenas, mesa comedor, heladera, termotanque y equipamiento. Cuando abres una puerta, el colisionador permite atravesar el vano libremente.
- **Puertas con bisagra real y 29 cajones con corredera telescópica (`Tecla E` o Clic izquierdo):**
  - Puerta principal de entrada, puerta de habitación y puerta de baño en **Egger H3012 ST22 Coco Bolo**.
  - Alacenas rebatibles superiores e inferiores y cajoneras bajo mesada en **Egger H3433 ST22 Pino Aland Polar**.
  - Racks de TV y torres con puertas verticales y cajones en **Egger H3349 ST19 Roble Kaisersberg** y **U732 PG Gris Macadán**.
- **Físicas dinámicas de objetos (`Tecla F`):** Lanza o patea pelotas de fútbol y empuja objetos con masa, gravedad (`-18 m/s²`), fricción y rebote contra paredes y muebles.
- **Control de iluminación y capas:** Enciende/apaga las luces interiores de 4000K (`Tecla L`), usa la linterna de mano (`Tecla T`), ajusta la hora solar del día (06:00 a 22:00 hs) u oculta el techo (`Tecla C`) para inspeccionar la planta libre desde arriba.

## Cómo subirlo a GitHub Pages paso a paso

1. Crea un repositorio nuevo y público en [github.com/new](https://github.com/new) (por ejemplo, `casita-sebita-3d`).
2. Abre una terminal (`PowerShell` o `CMD`) dentro de esta carpeta descomprimida y ejecuta:

```bash
git init
git add index.html casitaSebita.glb README.md
git commit -m "Subir espacio 3D Casita Sebita con colisiones y fisicas"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/casita-sebita-3d.git
git push -u origin main
```

3. En GitHub, entra a **Settings → Pages**, en **Build and deployment → Branch** selecciona `main` y `/ (root)` y haz clic en **Save**.
4. En menos de 1 minuto tu espacio 3D estará online en:
   `https://TU_USUARIO.github.io/casita-sebita-3d/`
