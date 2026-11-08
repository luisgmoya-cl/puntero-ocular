# Control_Mente · Lector facial por webcam

Página web que analiza tu cara en tiempo real a través de la webcam. Usa [MediaPipe Face Landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/face_landmarker) para estimar:

- **Emociones aparentes:** alegría, sorpresa, enfado, tristeza, desagrado, concentración y neutral. Se calculan a partir de los movimientos de los músculos de la cara.
- **Mirada:** hacia dónde miras.
- **Cabeza:** giro, inclinación y ladeo.
- **Parpadeo:** número de parpadeos y parpadeos por minuto.
- **Juego "responde sin hablar":** detecta si asientes (sí) o niegas (no) con la cabeza.

> **Aviso:** ningún software puede leer pensamientos con una cámara. El programa interpreta señales que se ven en la cara, y las expresiones no siempre reflejan lo que sientes.

## Uso

1. Abre `index.html` en Chrome o Edge. Puedes abrirlo como archivo local o servirlo, por ejemplo con `python3 -m http.server`.
2. Pulsa **Activar cámara** y da permiso para usarla.
3. La primera vez necesita internet para descargar el modelo de análisis facial.

Todo el análisis se hace en el navegador y no se envía ninguna imagen a ningún servidor.
