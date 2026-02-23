# Editor de plantilla con texto fijo

Página para superponer **texto en posiciones fijas** sobre una imagen plantilla y **guardar el resultado** como una nueva imagen.

## Uso

1. **Imagen plantilla**: Coloca tu imagen en la misma carpeta con el nombre `plantilla.png`  
   (o cambia la ruta en `index.html`, variable `CONFIG.imagenUrl`).

2. **Abrir**: Abre `index.html` en el navegador (o vía XAMPP: `http://localhost/seguro/`).

3. **Completar**: Escribe en los cuadros de texto. La vista previa se actualiza al escribir.

4. **Guardar**: Pulsa **"Guardar imagen"** para descargar la imagen con el texto aplicado (siempre en las mismas posiciones).

## Cambiar posiciones o campos

En `index.html`, dentro del `<script>`, edita el objeto `CONFIG.campos`. Cada elemento tiene:

- `id`: identificador del campo (y del input).
- `etiqueta`: texto del label en el formulario.
- `x`, `y`: posición en píxeles sobre la imagen (esquina superior izquierda del texto).
- `fontSize`: tamaño de fuente en píxeles.
- `color`: color del texto (ej. `'#000000'`).
- `maxAncho`: ancho máximo para el texto (opcional).

Puedes añadir o quitar campos modificando el array `CONFIG.campos`.
