# JARVIS Android Starter

Prototipo Android en Kotlin + Jetpack Compose, pensado como punto de partida para un asistente personal estilo JARVIS.

## Incluye
- Interfaz oscura con acentos azul cian.
- Chat local con respuestas de demostración.
- Historial de chat y recuerdos persistentes en almacenamiento privado de la aplicación.
- Comandos de memoria: `Recuerda que ...` y `¿Qué recuerdas?`.
- Reconocimiento de voz al tocar el micrófono y respuestas habladas con TextToSpeech.
- Selector de aplicaciones para memoria opcional de notificaciones: WhatsApp, Telegram, Instagram, Gmail y Mensajes SMS.
- Servicio de Android Notification Listener: guarda localmente título y texto de las notificaciones de las aplicaciones seleccionadas, con un límite de 250 registros.
- Pantalla para revisar y borrar el historial de notificaciones.

## Activar memoria de notificaciones
1. Instala y abre la app.
2. Toca el ícono de notificaciones en la esquina superior derecha y elegí las aplicaciones deseadas.
3. Toca **Permitir notificaciones**.
4. En los ajustes de Android, habilitá el acceso de notificaciones para JARVIS.
5. Cuando lleguen nuevas notificaciones de las aplicaciones seleccionadas, JARVIS podrá guardar el texto que Android le entregue.

Para consultar los avisos guardados, probá `¿Qué notificaciones tengo de WhatsApp?` o tocá **Ver historial**.

## Límites y privacidad
- Esto NO permite leer automáticamente todos los chats antiguos ni abrir bases de datos privadas de WhatsApp u otras aplicaciones. Solo guarda lo que aparece en notificaciones nuevas y que Android entrega al servicio; el contenido puede estar oculto o incompleto según los ajustes de notificación.
- El usuario debe habilitar manualmente el acceso especial a notificaciones y seleccionar las apps. Desactivar el acceso en Ajustes detiene la captura.
- Los textos de las notificaciones pueden contener información privada. En esta versión se guardan localmente en las preferencias privadas de la app, sin cifrado adicional ni envío a servidores. No uses esta versión en un teléfono compartido; borra el historial cuando ya no lo necesites.
- El prototipo no está conectado a una IA real ni a un backend; las respuestas generales siguen siendo reglas locales.
- Todavía no incluye ventana flotante ni activación continua al decir “JARVIS”.
- El proyecto no ha sido compilado ni probado en un dispositivo Android en esta sesión.

## Abrir el proyecto
1. Descargá y descomprimí el ZIP.
2. Abrí la carpeta `JARVIS_Android_Starter` desde Android Studio.
3. Usá JDK 17 y esperá a que Gradle descargue dependencias.
4. Conectá un Android o iniciá un emulador y pulsá Run.

No pongas claves privadas de servicios de IA dentro del APK. Para conectar una IA online, usá un backend seguro.
