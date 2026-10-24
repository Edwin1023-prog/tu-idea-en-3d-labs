# Tu Idea en 3D — Laboratorios

Dos páginas web independientes (HTML + CSS + JS, sin backend) del trabajo
"Tu Idea en 3D: CRISP-DM y KPIs":

- `index.html` — página de entrada con enlaces a las dos apps.
- `laboratorio-precios.html` — importar datos, limpieza, curva de demanda,
  utilidad y simulación de escenarios de precio.
- `laboratorio-confusion.html` — calculadora de matriz de confusión con
  9 casos precargados y un ejercicio de regla de clasificación.

No necesitan servidor ni build: son archivos estáticos, se abren tal cual
en el navegador y también se pueden desplegar directo en Vercel, Netlify,
GitHub Pages o cualquier hosting estático.

## Subir a GitHub (sin usar la terminal)

1. Entra a https://github.com/new (con tu usuario `Edwin1023-prog`).
2. Ponle un nombre al repositorio, por ejemplo `tu-idea-en-3d-labs`, y
   márcalo como público o privado, como prefieras. Crea el repositorio
   (no marques "Add a README", para que quede vacío).
3. En la página del repo recién creado, haz clic en **"uploading an
   existing file"** (o en "Add file" → "Upload files").
4. Arrastra los tres archivos `.html` de esta carpeta (o todo el
   contenido descomprimido del zip) a la ventana del navegador.
5. Baja y haz clic en **"Commit changes"**.

Listo — el código ya está en tu GitHub.

## Desplegar en Vercel (importando desde GitHub)

1. Entra a https://vercel.com/new con tu cuenta
   (`edwinisaacalbarracinmolina-5960`).
2. Conecta tu cuenta de GitHub si todavía no lo has hecho (Vercel te lo
   pide la primera vez) y dale permiso para ver tus repositorios.
3. Busca el repositorio que acabas de crear (`tu-idea-en-3d-labs`) en la
   lista y haz clic en **"Import"**.
4. Vercel detecta que es un sitio estático: no hay que tocar ningún
   ajuste de framework ni de build — deja todo como está.
5. Haz clic en **"Deploy"**. En menos de un minuto te da una URL pública
   (algo como `tu-idea-en-3d-labs.vercel.app`) con las dos apps en línea.

Cada vez que subas un cambio nuevo al repositorio de GitHub, Vercel
vuelve a desplegar automáticamente.
