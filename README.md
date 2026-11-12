# Tu Idea en 3D — Laboratorios

Cinco páginas web independientes (HTML + CSS + JS, sin backend) del trabajo
"Tu Idea en 3D: CRISP-DM y KPIs". Las cinco permiten subir tus propios datos
(CSV, TSV, JSON o Excel) y recalculan todo en el navegador, en vivo:

- `index.html` — página de entrada con enlaces a las cinco apps.
- `laboratorio-precios.html` — importar datos, limpieza, curva de demanda,
  utilidad y simulación de escenarios de precio.
- `laboratorio-clustering.html` — importar datos, elegir variables y número
  de segmentos (k), K-Medias con selección por ancho de silueta y
  validación de estabilidad por bootstrap.
- `laboratorio-confusion.html` — importar un archivo (clase real/predicha,
  o una columna numérica para el ejercicio de regla) o elegir uno de los
  9 casos precargados; matriz 2×2 editable y métricas en vivo.
- `laboratorio-regresion.html` — importar datos, elegir variable objetivo y
  hasta 4 predictoras; regresión lineal múltiple por mínimos cuadrados
  (coeficientes, pruebas t/F, VIF, diagnóstico de residuales) y un
  simulador de escenarios "qué pasaría si" con intervalos de confianza.
- `laboratorio-arboles.html` — importar datos, elegir qué predecir y con
  qué variables; árbol de decisión (CART, impureza de Gini) con
  profundidad y tamaño de hoja ajustables, matriz de confusión sobre un
  30% de datos de prueba, importancia de variables y un simulador de
  predicción con el camino completo por el árbol. Viene precargado con 9.240 leads reales del dataset Lead Scoring de Kaggle (no son datos de Tu Idea en 3D; ver sección 11 del documento CRISP-DM).

No necesitan servidor ni build: son archivos estáticos, se abren tal cual
en el navegador y también se pueden desplegar directo en Vercel, Netlify,
GitHub Pages o cualquier hosting estático.

## Subir a GitHub por primera vez (sin usar la terminal)

1. Entra a https://github.com/new (con tu usuario de GitHub).
2. Ponle un nombre al repositorio, por ejemplo `tu-idea-en-3d-labs`, y
   márcalo como público o privado, como prefieras. Crea el repositorio
   (no marques "Add a README", para que quede vacío).
3. En la página del repo recién creado, haz clic en **"uploading an
   existing file"** (o en "Add file" → "Upload files").
4. Arrastra los seis archivos de esta carpeta (los cinco `.html` y el
   `README.md`) a la ventana del navegador.
5. Baja y haz clic en **"Commit changes"**.

## Actualizar un repositorio que ya existe

Para subir una versión nueva de estos archivos (por ejemplo, después de
pedir un cambio), no hace falta borrar nada: en la página del repositorio
usa de nuevo **"Add file" → "Upload files"** y arrastra los archivos
actualizados. Si un archivo ya existe con el mismo nombre, GitHub lo
reemplaza automáticamente al hacer "Commit changes"; los que sean nuevos
(como `laboratorio-regresion.html` o `laboratorio-arboles.html`) simplemente se agregan.

## Desplegar en Vercel (importando desde GitHub)

1. Entra a https://vercel.com/new con tu cuenta de Vercel.
2. Conecta tu cuenta de GitHub si todavía no lo has hecho (Vercel te lo
   pide la primera vez) y dale permiso para ver tus repositorios.
3. Busca el repositorio que creaste (`tu-idea-en-3d-labs`) en la lista y
   haz clic en **"Import"**.
4. Vercel detecta que es un sitio estático: no hay que tocar ningún
   ajuste de framework ni de build — deja todo como está.
5. Haz clic en **"Deploy"**. En menos de un minuto te da una URL pública
   con las cinco apps en línea.

Cada vez que subas un cambio nuevo al repositorio de GitHub (paso
"Actualizar un repositorio que ya existe" arriba), Vercel vuelve a
desplegar automáticamente — no hay que repetir el paso de Vercel.
