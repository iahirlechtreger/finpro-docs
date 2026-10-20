SITIO DE DOCUMENTACIÓN DE FINPRO (sitio propio, estático)

Diseño como la maqueta: barra lateral con títulos colapsables y sus
subtítulos adentro, que te llevan directo a cada parte de la misma página.
Los requests de la API tienen pestañas de lenguaje (cURL, JavaScript,
Python, PHP, Java) que cambiás con un clic; el lenguaje elegido se aplica
a todos los bloques. No usa Mintlify: son archivos estáticos.

CONTENIDO
- index.html   -> el sitio entero (contenido embebido)
- images/      -> las capturas

PROBARLO: doble clic en index.html.

PUBLICARLO (elegí una)
1) Netlify: app.netlify.com -> "Add new site" -> "Deploy manually" y
   arrastrá esta carpeta. Después se le pone docs.finpro.com.ar.
2) GitHub Pages: subí esta carpeta a un repo y activá Pages.
3) Cualquier hosting estático: subí index.html + images/.

BOTÓN "DOCUMENTACIÓN" DEL PORTAL -> apuntar a la URL del sitio (pestaña nueva):
  <a href="https://docs.finpro.com.ar" target="_blank" rel="noopener">Documentación</a>

EDITAR: el contenido viene de los .mdx de finpro-docs y se arma con
build_site.py. Editás texto y se regenera el sitio.

REVISAR ANTES DE PUBLICAR
- La URL base de la API es mw-dev.finpro.com.ar (desarrollo): confirmá cuál
  va en la documentación pública.
- Las capturas son pantallas reales del portal: que no quede dato sensible.
