# Andro-Kontrol

**Maneja el móvil hablando y moviendo la cabeza.** Pensado para quien no puede
usar las manos, o no siempre.

- **Un puntero** que se mueve con la cara: la cámara frontal sigue tu nariz.
  También se puede mover **por voz**, con las direcciones de la brújula
  («norte», «este cincuenta»…).
- **Comandos de voz** para todo lo demás: pulsar, pulsación larga, atrás,
  inicio, recientes, desplazar, abrir apps, cerrar, salir, pestañas… y los
  botones de cualquier app por su nombre («enviar», «buscar», «pulsa
  descargar»).
- **Dictado**: cuando aparece el cursor en un campo de texto, dictas y dices
  «entra» para escribirlo. El teclado del sistema no hace falta.
- **El teléfono por voz**: «responde», «cuelga», «llama a Marta». Mientras
  suena el tono sigue encendido; con la llamada descolgada se aparta, y vuelve
  en los silencios para que puedas colgar hablando.
- **Ir a un sitio**: «conduce a la playa», «pasea a la farmacia», «pasea en
  bici al parque». Se lo pasa a tu app de navegación con el medio ya elegido, y
  si la ubicación está apagada la enciende él. Para terminar, «salir».
- **WhatsApp**: «guasea a Marta» abre su chat y ya puedes dictar el mensaje.
- **Música y vídeo**: reproduce, pausa, siguiente canción, volumen…
- **Convive con tu asistente**: si dices «alexa», Andro-Kontrol se apaga solo
  y vuelve cuando ella termina de hablar, así no confunde su voz con órdenes
  tuyas. La música no le afecta.

- **Bloqueo por voz** (opcional, y viene apagado): un candado que solo abre tu
  voz diciendo tu santo y seña. Si no te reconoce, manda el móvil a su pantalla
  de bloqueo, y puede tapar la pantalla mientras está cerrado. Lee el aviso de
  más abajo antes de encenderlo.
- **El puntero se puede esconder** sin apagarlo: «oculta el puntero» deja de
  dibujarlo, pero sigue moviéndose, pulsando y desplazando la pantalla.

> **Versión 1.0.** Se usa a diario y está probada en un Motorola Moto G31 con
> Android 12. En otros móviles puede haber diferencias, sobre todo en lo que
> depende del fabricante (los ajustes de ubicación, por ejemplo). Si encuentras
> un fallo, se agradece el aviso.

## Aviso sobre el bloqueo por voz

**Encenderlo es decisión tuya, y el riesgo también.** Úsalo con precaución y
sabiendo lo que hace y lo que no:

- **No es seguridad fuerte.** Una voz se puede grabar e imitar, y el parecido
  se mide con un margen. Quien guarda el móvil de verdad es su propio bloqueo
  (huella, PIN o patrón): esto es una capa más encima, nunca un sustituto.
- **Puede no reconocerte**: si exiges mucho parecido, si estás afónico, si hay
  ruido o si el micrófono está tapado. No te deja sin móvil —sigues entrando
  con tu huella o tu PIN y puedes apagar Andro-Kontrol con su botón—, pero
  incordia.
- **Manda el móvil a la pantalla de bloqueo** en cada intento que no reconoce,
  y cuando se cumplen las esperas.

Con Andro-Kontrol apagado no hay candado: ni se bloquea ni se ve, porque
apagado no escucha y no habría forma de abrirlo hablando.

Se enciende, se apaga y se ajusta en **⋮ → Ajustes → Bloqueo por voz**, con
Andro-Kontrol apagado: allí se graba el perfil de voz y el santo y seña, se
marca o desmarca la casilla, y se ajustan el parecido exigido (de partida
38 %, con tope 47 % para que no puedas dejarte fuera) y si quieres que **tape la
pantalla** mientras está cerrado —pantalla negra con el candado grande; la
salida, si la voz fallara, es mantener el candado pulsado 5 segundos, que no
abre el móvil: apaga Andro-Kontrol y lo manda a su pantalla de bloqueo—. El
manual lo explica entero.

## Descarga

La versión de cada momento está en la pestaña
[**Releases**](../../releases). Más información y explicación en
[pipataki.net](https://pipataki.net/andro-kontrol.html).

También hay **manual en PDF**, en español e inglés, en cada release.

**Para instalarla:** descarga la APK en el móvil y ábrela con **Archivos
(Files) de Google**. Android pedirá permiso para instalar apps de origen
desconocido, y Play Protect puede analizarla antes; es lo normal en cualquier
app que no venga de Google Play.

Con algunos gestores de archivos Android no permite instalar: no es cosa de
Andro-Kontrol, es que la app que abre el fichero necesita el permiso de
instalar aplicaciones.

### Comprobar que la APK es la nuestra

Firma del certificado con el que se firman todas las versiones:

```
SHA-256: 40:EA:E6:CA:4A:6C:CE:5D:38:D6:61:A4:8D:9B:64:18:25:4F:01:3E:D7:75:83:4A:98:3B:E9:82:73:AF:C2:29
```

## Qué necesita

- Android 8 o superior, procesador ARM de 64 bits.
- **Permisos**, que se conceden desde la propia app (menú ⋮ → Ajustes):
  - **servicio de accesibilidad**: es lo que dibuja el puntero y pulsa por ti;
  - **cámara**: para seguir la nariz;
  - **micrófono**: para los comandos y el dictado;
  - **teléfono**: para apartarse cuando entra una llamada;
  - **responder llamadas**: para descolgar y colgar hablando;
  - **llamar y agenda**: para llamar a un contacto diciendo su nombre;
  - **modificar ajustes del sistema**: para mantener la pantalla en vertical
    mientras está encendida.

## Privacidad

- **La imagen de la cámara no sale del teléfono.** La cara se analiza ahí
  mismo y de ella solo sale una posición para el puntero.
- **Los comandos de voz se reconocen en el propio teléfono**, sin conexión.
- **El dictado usa el reconocedor de voz del sistema.** En el móvil de pruebas
  funcionó sin conexión, pero eso depende del teléfono y de su configuración.
- Andro-Kontrol **no envía nada a ningún servidor** y no lleva publicidad ni
  medición de uso.
- **No deja rastro de lo que oye.** El registro del móvil (`adb logcat`) viene
  apagado; solo apunta órdenes, dictado y nombres de contactos si enciendes a
  propósito *Registro para pruebas*, en ⋮ → Ajustes → Pruebas, para buscar un
  fallo. Los errores sí se apuntan siempre, y no llevan lo que has dicho.

## Licencia

Andro-Kontrol es **© 2026 pipataki. Todos los derechos reservados.** Este
repositorio contiene solo las descargas: el código fuente no se publica.

Lleva dentro componentes de terceros con licencia **Apache 2.0**, a los que hay
que dar crédito:

| Componente | Autor |
|---|---|
| Vosk (vosk-android) y los modelos `vosk-model-small-es-0.42` y `vosk-model-spk-0.4` | Alpha Cephei Inc. / AC Technologies LLC |
| MediaPipe Tasks Vision y el modelo `face_landmarker.task` | Google LLC |
| AndroidX CameraX | The Android Open Source Project |
| JNA | Java Native Access project |

El robot del icono es un dibujo propio: no es el androide de Google.

## Contacto

[pipataki@pipataki.net](mailto:pipataki@pipataki.net)

También puedes abrir un [issue](../../issues) para contar un fallo o pedir algo.

---

Hay un proyecto hermano para el ordenador, **VoiceController** (software libre,
LGPLv3): [github.com/pipataki/VoiceController](https://github.com/pipataki/VoiceController).
