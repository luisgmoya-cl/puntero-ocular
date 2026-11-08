# Control_Mente · Lector facial por webcam

Página web que analiza tu cara en tiempo real a través de la webcam. Usa [MediaPipe Face Landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/face_landmarker) para estimar:

- **Emociones aparentes:** alegría, sorpresa, enfado, tristeza, desagrado, concentración y neutral. Se calculan a partir de los movimientos de los músculos de la cara.
- **Mirada:** hacia dónde miras.
- **Cabeza:** giro, inclinación y ladeo.
- **Parpadeo:** número de parpadeos y parpadeos por minuto.
- **Juego "responde sin hablar":** detecta si asientes (sí) o niegas (no) con la cabeza.

> **Aviso:** ningún software puede leer pensamientos con una cámara. El programa interpreta señales que se ven en la cara, y las expresiones no siempre reflejan lo que sientes.

## Clon digital (`clon.html`)

1. **Captura:** hace una foto de tu cara en posición neutra y la convierte en una malla de triángulos con tu propia imagen.
2. **Espejo (10 s):** el clon copia tus gestos en tiempo real y graba tu sonrisa, boca abierta, cejas arriba y ceño fruncido.
3. **IA:** el clon se mueve solo. Combina los gestos que te ha aprendido, parpadea, te sigue con la mirada y habla con síntesis de voz.

## Uso

1. Abre `index.html` (o `clon.html`) en Chrome o Edge. Puedes abrirlo como archivo local o servirlo, por ejemplo con `python3 -m http.server`.
2. Pulsa **Activar cámara** y da permiso para usarla.
3. La primera vez necesita internet para descargar el modelo de análisis facial.

Todo el análisis se hace en el navegador y no se envía ninguna imagen a ningún servidor.
