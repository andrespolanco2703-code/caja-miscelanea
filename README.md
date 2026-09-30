# Caja Miscelánea · APK para Android (funciona sin internet)

Esta carpeta convierte la app en un archivo **APK** que se instala en Android y funciona **sin internet**.
Todo se guarda en el propio teléfono. El APK se construye gratis en la nube de GitHub: no necesitas
instalar nada en tu computador.

## Cómo obtener el APK
1. Crea una cuenta gratis en github.com.
2. Crea un repositorio nuevo (botón **New**), con el nombre que quieras.
3. Entra al repositorio y usa **Add file → Upload files**. Arrastra TODO el contenido de esta carpeta.
   Comprueba que se suban `www`, `resources`, `package.json`, `capacitor.config.json` y la carpeta oculta
   **`.github`** (si tu computador la oculta, activa "mostrar archivos ocultos"). Pulsa **Commit changes**.
4. Abre la pestaña **Actions**. Verás "Construir APK" en marcha (tarda unos 5 a 10 minutos).
   Si no arrancó sola: entra a "Construir APK" → **Run workflow**.
5. Cuando tenga la marca verde, abre esa ejecución y baja a **Artifacts**: descarga **caja-miscelanea-apk**.
   Es un zip; dentro está `caja-miscelanea.apk`.
6. Pasa el APK al celular (cable, WhatsApp, Drive o correo), ábrelo y acepta
   **"Instalar apps de origen desconocido"** cuando Android lo pida.

## Cosas que debes saber
- **Solo Android.** En iPhone no se pueden instalar APK; allí se usa la versión web instalable.
- Es un APK de pruebas (firma "debug"): sirve para instalar en tus teléfonos, no para subir a Play Store.
- **Los datos viven solo en ese teléfono.** Si desinstalas la app o borras sus datos, se pierden. Usa
  Ajustes ⚙ → **Exportar copia** con frecuencia y guarda el archivo en Drive o WhatsApp; se recupera con **Importar copia**.
- Cada teléfono tiene sus propios datos (no se sincronizan entre sí).
- El escáner con la cámara depende de que tu teléfono lo permita. Si no funciona, un lector de códigos USB/Bluetooth sí,
  porque escribe el código como un teclado.
- Para actualizar la app: cambia `www/index.html` en GitHub y espera a que se construya un APK nuevo.
