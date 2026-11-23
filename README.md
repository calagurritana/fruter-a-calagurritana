# RiojoHome 🍐🏠

Tienda online de la **Frutería Calagurritana**: tus clientes ven los productos, hacen su pedido
y te llega por **WhatsApp** (o por email). Tú metes y cambias los productos desde el móvil.

Es una app web: se abre en cualquier navegador y se puede **instalar en el móvil** como una app
(«Añadir a pantalla de inicio»). No necesita servidor ni pagar nada.

## Qué puede hacer

**Para tus clientes**
- Ver los productos por categorías, buscar, ver ofertas y destacados.
- Añadir al pedido (al peso de medio en medio kilo, o por unidad, docena, manojo, bandeja…).
- Elegir envío a domicilio o recogida en tienda, con envío gratis a partir de un importe y pedido mínimo.
- Enviar el pedido: se abre WhatsApp con el pedido ya escrito para mandártelo.

**Para ti (Gestión)**
- Añadir, editar, duplicar y borrar productos, con **foto hecha con el móvil** o un icono.
- Cambiar precios y marcar «Agotado» directamente desde la lista, sin abrir cada producto.
- Ofertas (precio anterior tachado), destacados, origen y descripción.
- Crear, renombrar, ordenar y borrar categorías.
- Ajustes: nombre, frase, horario, teléfono, email, **WhatsApp donde recibir pedidos**, gastos de envío.
- Copias de seguridad.

## Cómo entrar en Gestión

Abajo del todo de la tienda pulsa **«Acceso gestión»**.

- PIN inicial: **1234** → cámbialo en *Gestión → Ajustes*.
- Lo primero: en *Ajustes* pon tu **número de WhatsApp** para recibir los pedidos.
- Los productos que vienen son de **ejemplo, con precios orientativos**. Cámbialos o bórralos
  en *Publicar y copias → Borrar todos los productos*.

## Ponerla en internet (gratis, con GitHub Pages)

1. En GitHub, entra en el repositorio → **Settings** → **Pages**.
2. En *Build and deployment* elige **Deploy from a branch**, rama **main** y carpeta **/ (root)**. Guarda.
3. En un par de minutos tendrás la dirección de tu tienda, por ejemplo:
   `https://calagurritana.github.io/fruter-a-calagurritana/`
4. Abre esa dirección en tu móvil y pulsa «Añadir a pantalla de inicio» para tenerla como app.

## Cómo actualizar los productos que ven tus clientes

Los cambios que haces en Gestión se guardan **en tu móvil**. Para que los vean todos:

1. En *Gestión → Publicar y copias* pulsa **Descargar productos.json**.
2. En GitHub, en el repositorio, pulsa **Add file → Upload files**, sube ese archivo
   (sustituye al que hay) y pulsa **Commit changes**.
3. En uno o dos minutos la tienda mostrará los cambios a todo el mundo.

La app te avisa con un cartel cuando tienes cambios sin publicar.

> Consejo: las fotos se reducen solas, pero cuantas menos fotos, más rápido carga la tienda.

## Archivos

| Archivo | Para qué sirve |
| --- | --- |
| `index.html` | La app completa (tienda + gestión). |
| `productos.json` | Los productos, categorías y ajustes que ven tus clientes. |
| `manifest.webmanifest`, `sw.js`, `icon*.png`, `icon.svg` | Para instalarla como app y que funcione sin conexión. |
| `DOCTYPE.html` | La página antigua (ya no se usa). |
