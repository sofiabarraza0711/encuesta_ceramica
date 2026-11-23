# Cuestionario para ceramistas 🌸

Página web simple (un solo archivo `index.html`) para celular. El cliente completa el cuestionario y al final toca **«Enviar respuestas por WhatsApp»**: se abre el chat con el número `5493856232931` y el mensaje ya armado con todas sus respuestas.

## Subir a GitHub Pages

1. Creá un repositorio en GitHub y subí el archivo `index.html` (puede estar en la raíz).
2. En el repo: **Settings → Pages**.
3. En *Build and deployment*, elegí **Deploy from a branch** → rama `main` → carpeta `/ (root)` → **Save**.
4. Esperá un minuto y GitHub te da la URL, por ejemplo:
   `https://TU-USUARIO.github.io/TU-REPO/`
5. Abrí esa URL desde el celular y compartila con quien tenga que responder.

## Cambiar el número de WhatsApp

En `index.html`, cerca del final, buscá esta línea y editá el número (con código de país, sin `+` ni espacios):

```js
const WHATSAPP_NUMBER = "5493856232931";
```

Si lo dejás vacío (`""`), se abre WhatsApp para que la persona elija el contacto.

## Notas

- No necesita instalación ni dependencias: funciona con abrir el archivo o desde GitHub Pages.
- Las preguntas con «Sí/No» y opciones avanzan solas al tocar; los campos numéricos tienen botón «No lo sé / saltar».
- El resumen agrupa las respuestas por sección y el mensaje de WhatsApp se genera automáticamente.
