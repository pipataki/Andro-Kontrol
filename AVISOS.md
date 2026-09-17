# Avisos legales de Andro-Kontrol

Andro-Kontrol es **© 2026 pipataki**. Todos los derechos reservados. Se
reparte solo la APK firmada; las fuentes no se publican.

## Componentes de terceros

Andro-Kontrol incluye estos componentes, todos bajo la **licencia Apache
2.0**, cuyo texto completo está en `APACHE-2.0.txt`:

| Componente | Autor | Para qué se usa |
|---|---|---|
| Vosk (vosk-android 0.3.47) | Alpha Cephei Inc. | reconocimiento de voz de los comandos, en el móvil |
| Modelo de voz `vosk-model-small-es-0.42` | AC Technologies LLC | el vocabulario español de esos comandos |
| MediaPipe Tasks Vision 0.10.14 | Google LLC | detección de la cara para mover el puntero con la nariz |
| Modelo `face_landmarker.task` | Google LLC | los 478 puntos de la cara |
| AndroidX CameraX 1.3.4 | The Android Open Source Project | acceso a la cámara frontal |
| JNA 5.13.0 | Java Native Access project (doble licencia; se usa bajo Apache 2.0) | puente de Vosk con su parte nativa |

El dictado usa el reconocimiento de voz que ya trae el móvil (en el
teléfono de pruebas, *Servicios de voz de Google*): no va dentro de la APK.

## Privacidad

- **La imagen de la cámara no sale del teléfono**: la cara se analiza ahí
  mismo y de ella solo sale una posición para el puntero.
- **Los comandos de voz se reconocen en el teléfono**, sin conexión.
- **El dictado lo hace el reconocedor del sistema.** En el teléfono de
  pruebas trabajó sin conexión (reconocimiento en el dispositivo), pero eso
  depende del móvil y de su configuración.
- Andro-Kontrol no envía nada a ningún servidor.
