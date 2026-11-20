# Escaneo de retornos (PDA)

Pantalla de recepción de retornos de paqueterías para el almacén. Es la misma pantalla de la app de Apps Script, publicada aquí con GitHub Pages para poder usar la **cámara en vivo** del teléfono. Google bloquea la cámara en vivo dentro de Apps Script.

La página no guarda datos. Cada escaneo se envía a la hoja de cálculo por medio de la aplicación web de Apps Script (`doPost`), protegida con un código de acceso.

## Configurar un teléfono o PDA

1. El responsable comparte el **enlace de configuración** (ver abajo).
2. Ábrelo en Chrome. La página guarda la conexión en el teléfono y quita los datos de la barra de direcciones.
3. Menú ⋮ → **Agregar a pantalla principal**.
4. Toca 📷 y luego **Permitir** cuando pida la cámara.

Si la página pide **Conectar con la hoja**, escribe la URL de la app (termina en `/exec`) y el código de acceso.

## Enlace de configuración

```
https://fcoramirezsalda-hub.github.io/mx-returns/#api=<URL de la app /exec>&k=<código de acceso>
```

La URL `/exec` y el código **no se guardan en este repositorio**: viajan solo en el enlace (después de `#`, que el navegador no envía a GitHub) y quedan en el teléfono.

## Actualizar la pantalla

`index.html` es una copia de `Index.html` del proyecto de Apps Script. Si cambia la pantalla, reemplaza `index.html` aquí y en Apps Script con el mismo archivo.
