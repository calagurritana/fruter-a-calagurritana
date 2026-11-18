# Segunda campaña Meta Ads: cama Nino de pana (RiojoHome)

Preparado el 18-11-2026 con datos de Shopify (www.riojohome.com, últimos 90 días) y de Meta Ads.

## ✅ Estado: campaña PUBLICADA el 18-11-2026

Cuenta publicitaria **Riojohome** (2816733155395657), la que tiene el píxel 1863401214833955.

| Nivel | Nombre | ID |
|---|---|---|
| Campaña | NINO-PANA \| Ventas \| ES \| Nov-Dic 26. Ventas, 20 €/día de presupuesto de campaña, puja por menor coste | 52571512716856 |
| Conjunto | Amplio \| España \| 25+ \| Compra. Evento Compra del píxel, España, 25–65, público Advantage+, ubicaciones automáticas | 52571512725656 |
| Anuncio | AD1 Producto-Invierno: cama sola, 2 textos y 3 titulares | 52571512962456 |
| Anuncio | AD2 Lavable-Golden: golden en la terraza, 2 textos y 3 titulares | 52571512962856 |
| Anuncio | AD3 Carrusel: 3 fotos | 52571512964456 |

- Enlace: ficha de la variante de pana (`?variant=54000292987216`). UTM:
  `utm_source=meta&utm_medium=paid&utm_campaign=nino-pana-ventas&utm_content={{ad.name}}`.
- Botón: "Comprar". Página de Facebook RiojoHome e Instagram @riojohome_.
### Actualización 18-11-2026 (tarde)

- **Creatividades nuevas en formato 4:5 y en español** (en `campanas/creatividades/`): salón con el
  bulldog, siesta, lavable y beneficios. Ya están subidas a Meta.
- **Anuncios nuevos en borrador**, pendientes de revisar y publicar:

  | Anuncio | ID |
  |---|---|
  | AD4 Salon-Bulldog v2 | 52571513873056 |
  | AD5 Siesta-Golden v2 | 52571513892456 |
  | AD6 Lavable-Golden v2 | 52571513894456 |
  | AD7 Carrusel v2 | 52571513909256 |

  Al publicarlos, pausar AD1–AD3.
- **Política de devoluciones** publicada en https://www.riojohome.com/pages/politica-de-devoluciones
  y enlazada en el pie de página como "Devoluciones". Falta copiarla también en Ajustes → Políticas
  → Política de reembolso: la API no tiene permiso para escribir ahí.
- **Excluir Canarias, Baleares, Ceuta y Melilla:** hay que hacerlo a mano en el conjunto de anuncios.
  La conexión con Meta no permite buscar los códigos de esas regiones.

- **Lo que falta respecto al plan:**
  - No se pudo usar la foto del bulldog: Meta no la pudo descargar y la subida manual no tenía permiso.
  - Canarias, Ceuta y Melilla no están excluidas.
  - No hay Reel.
  - Los arreglos de la tienda (sección 3) siguen pendientes.

---

## 1. Análisis de la primera campaña: `flame-heater-ventas`

Producto: Flame Heater (calefactor efecto chimenea), 39,99 €.

### Lo que ve Meta

La campaña es una **publicación promocionada** ("🎄 Esta Navidad, regala calor."). Está en **otra
cuenta publicitaria (266863922595644), sin negocio ni píxel**, y sigue **activa** a 2 €/día desde el 11-11-2026.

| Métrica | Valor |
|---|---|
| Objetivo | **Interacción** (no ventas) |
| Gasto | 14,01 € |
| Impresiones / alcance | 4.778 / 3.007 personas |
| Clics en el enlace | 85 (0,16 € por clic) |
| Visitas a la página, carritos, compras | **No se miden**: esa cuenta no tiene el píxel |

**Conclusión:** Meta repartió el anuncio entre gente que da "me gusta" y hace clic, no entre gente
que compra. De 85 clics, Shopify solo registró unas 36 visitas y ninguna compra. Con un objetivo de
interacción y sin píxel, Meta no puede aprender quién compra.

### Lo que ve Shopify

| Paso del embudo | Campaña (UTM `flame-heater-ventas`) | Facebook/Instagram sin UTM* |
|---|---|---|
| Visitas | 13 (9 móvil, 4 ordenador) | 23 (15 FB España, 5 IG España, 3 FB Reino Unido) |
| Añadieron al carrito | 2 (15 %) | 3 |
| Llegaron al pago | 1 | 2 |
| **Compras** | **0** | **0** |
| Rebote | 78 % móvil, 100 % ordenador | — |

\* El navegador interno de Facebook/Instagram a veces borra el UTM. Esas 23 visitas seguramente
también vienen de los anuncios.

En toda la tienda: 453 visitas en 90 días y **0 ventas reales**. El único pedido (#1001, 12,99 €) es de prueba y está reembolsado.

### Diagnóstico

1. **Llegó muy poco tráfico.** Unas 13–36 visitas no bastan para que Meta aprenda. Una campaña
   de ventas necesita unas 50 compras por semana para salir de la fase de aprendizaje. Con un
   producto de 40 € y poco presupuesto, el algoritmo no tuvo datos con los que optimizar.
2. **El anuncio no fallaba tanto: la caída fue en la página y en el pago.** El 15 % de
   añadidos al carrito es razonable. Se perdió gente en el carrito y en el pago, lo que apunta
   a falta de confianza (tienda nueva, sin reseñas, sin política de devoluciones) o a sorpresas
   en el pago (plazo de entrega que no se conoce).
3. **Falta la política de devoluciones.** `/policies/refund-policy` da error 404. Para
   compras de más de 70 € es de lo primero que mira un cliente desconfiado.
4. **El tráfico está "sucio".** 291 de las 453 visitas son de EE. UU., sin origen y sin ningún
   carrito, así que son bots. 80 visitas cayeron en `/password`, la tienda bloqueada con
   contraseña. No hay que fiarse del número total de visitas.
5. **La tienda parece genérica.** El pie de página dice "Pequeños calefactores para inviernos
   más felices" y el catálogo mezcla calefactores, ollas, afeitadoras y una cama de perro de
   75–200 €. Para un producto premium eso resta confianza.

### Lo que está bien (no hay que tocarlo)

- **El píxel de Meta (ID 1863401214833955) está instalado** con la app Facebook & Instagram,
  con todos los eventos compartidos y la API de conversiones activa ("optimized"). Las compras
  se van a medir bien.
- **Judge.me está instalado**, pero el producto Nino aún no tiene reseñas.

### Qué cambia en la segunda campaña por todo esto

| Problema de la 1.ª | Ajuste en la 2.ª |
|---|---|
| Poco tráfico, Meta no aprende | 1 campaña, 1 conjunto de anuncios y público amplio, para concentrar todo el presupuesto |
| Pérdidas en carrito y pago | Arreglar la página **antes** de lanzar (sección 3) |
| No hay datos de compra | Optimizar por **Compra**, con reglas claras para no quemar dinero (sección 7) |
| Producto barato (margen pequeño) | La cama Nino cuesta 75–195 €, así que hay **más margen para pagar cada venta** |
| UTM que se pierde | UTM en la URL y en el parámetro de URL del anuncio (sección 5) |
| Fechas | Aprovechar **Black Friday (27-11)** y **Navidad** |

---

## 2. El producto: cama cesta Nino de pana Beige Vainilla

- Ficha en Shopify: "Cama cesta para perro Nino – Bouclé o Pana" (tejido Pana Beige Vainilla).
- Puntos fuertes: borde acolchado en los cuatro lados, funda con cremallera lavable a 30 °C,
  35.000 ciclos Martindale, fabricada en Polonia y dos rellenos (Classic o Memory Foam).
- Envío: las variantes de **pana** tienen **envío gratis a España** (perfil general).

| Talla | Medidas | Classic Foam | Memory Foam |
|---|---|---|---|
| XS | 70×55×30 | 75,60 € | 88,83 € |
| S | 80×60×30 | 86,94 € | 109,62 € |
| M | 100×75×35 | 103,95 € | 137,97 € |
| L | 115×85×35 | 120,96 € | 170,10 € |
| XL | sin medidas publicadas | 136,08 € | 194,67 € |

### Cuánto puedes pagar por cada venta (CPA máximo)

Los precios llevan IVA. La fórmula es:

> **CPA máximo = (precio ÷ 1,21) − coste del proveedor − envío que pagas tú − comisiones (≈ 3 %)**

Ejemplo con una cama XS Classic de 75,60 € y un coste **supuesto** de 40 €:
75,60 ÷ 1,21 = 62,48 → 62,48 − 40 − 1,90 = **≈ 20 € de CPA máximo**. Las tallas M y L dejan
bastante más.

**Necesito tu coste real por talla** para fijar la cifra exacta. En Shopify el campo "coste"
está vacío.

> ⚠️ **Ojo con el envío.** Las variantes de **bouclé** usan el perfil "Hertwill Shipping —
> Large", que cobra **16,73 € a España**. Las de **pana** usan el envío gratis. Si el proveedor
> también te cobra ~16,73 € por enviar la pana, ese dinero sale de tu margen. Compruébalo.

---

## 3. Arreglos en la tienda ANTES de lanzar (lo más importante)

Por orden de impacto:

1. **Crear la política de devoluciones** (Ajustes → Políticas): 14 días, quién paga la
   devolución y cómo se pide. Ahora mismo da 404.
2. **Poner el plazo de entrega en la ficha**, por ejemplo "Entrega en X–Y días laborables" (el
   plazo real del proveedor desde Polonia). Para Navidad, añadir la fecha límite: "Pide antes del
   XX/12 y llega para Navidad".
3. **Poner "Envío gratis a España" en la ficha**, junto al precio. Ahora solo sale en la cabecera
   ("Envío a toda España") y no deja claro que es gratis.
4. **Redondear los precios**: 75,60 → 74,90; 88,83 → 89,90; 86,94 → 84,90; 109,62 → 109,90;
   103,95 → 104,90; 137,97 → 139,90; 120,96 → 119,90; 170,10 → 169,90; 136,08 → 134,90;
   194,67 → 194,90. Precios como 83,16 € parecen calculados por una máquina y restan confianza.
5. **Publicar las medidas de la XL.** Ahora pone "escríbenos", y eso frena la compra.
6. **Cambiar el pie de página** ("Pequeños calefactores…") por algo general, como "Cosas bonitas
   y cómodas para tu casa".
7. **Reseñas**: pedir a 3–5 conocidos o clientes que la hayan probado que dejen una reseña en
   Judge.me con foto. Si no hay ninguna, no inventarlas.
8. **Ficha**: tipo de producto "Camas para perros" y etiquetas `perro`, `cama perro`, `mascotas`.
   Crear una colección "Mascotas".
9. Hacer una compra de prueba con la variante de pana para comprobar el precio final y el envío
   en el pago.

---

## 4. Estructura de la campaña en el Administrador de anuncios

```
CAMPAÑA:  NINO-PANA | Ventas | ES | Nov-Dic 26
  Objetivo:              Ventas
  Configuración:         Campaña de ventas Advantage+ (o manual con presupuesto Advantage+ de campaña)
  Ubicación conversión:  Sitio web
  Píxel / evento:        1863401214833955 / Compra
  Atribución:            7 días clic + 1 día visualización
  Presupuesto:           20 €/día (fase 1). Ver calendario en la sección 6
  │
  └── CONJUNTO: Amplio | España | 25-65
        Ubicación:  España, SIN Canarias, Ceuta ni Melilla (aduanas e IVA distinto)
        Edad:       25–65, todos los géneros
        Público:    Advantage+ con sugerencias de intereses: Perros, Dueños de mascotas,
                    Cachorros, Decoración del hogar, Diseño de interiores
        Ubicaciones: Advantage+ (automáticas)
        Excluir:    compradores de los últimos 180 días (cuando los haya)
        │
        ├── AD1  Salón: foto del bulldog en el salón (estático 4:5)
        ├── AD2  Invierno: "que no duerma en el suelo frío" (estático 4:5)
        ├── AD3  Carrusel de beneficios (5 tarjetas)
        ├── AD4  Reel 9:16 de 15 s
        └── AD5  Regalo de Navidad (se activa el 2-12)
```

**Por qué solo un conjunto de anuncios:** con 20–30 €/día, repartir el dinero en varios
públicos hace que ninguno junte datos. Un público amplio con el píxel funcionando deja a Meta
buscar a los compradores.

**Retargeting (desde la semana 2):** cuando haya más de 300 visitas a la ficha, crear un segundo
conjunto con 5 €/día. Público: quien vio el producto o añadió al carrito en los últimos 14 días
y no compró. Anuncio: reseñas, envío gratis y devolución fácil, más el código de Black Friday.

---

## 5. URL de destino y UTM

Enlazar directamente a la variante de pana para que se vea la foto beige y el precio más bajo:

```
https://www.riojohome.com/products/nino-boucle-dog-basket-bed-taupe?variant=54000292987216
```

En el campo **"Parámetros de URL"** del anuncio:

```
utm_source=meta&utm_medium=paid&utm_campaign=nino-pana-ventas&utm_content={{ad.name}}&utm_term={{adset.name}}
```

Así, en Shopify → Análisis → Sesiones por `utm_campaign`, se ve qué anuncio trae ventas.

---

## 6. Calendario y presupuesto

| Fase | Fechas | Presupuesto/día | Anuncios activos | Objetivo |
|---|---|---|---|---|
| 0. Preparar | 18–19 nov | — | — | Arreglos de la sección 3 y creatividades |
| 1. Test | 20–26 nov | 20 € | AD1–AD4 | Encontrar los 1–2 anuncios ganadores |
| 2. Black Friday | 27 nov – 1 dic | 30 € (+50 %) | Ganadores + versión con oferta | Vender con oferta |
| 3. Navidad | 2–14 dic | 25–40 € según resultados | Ganadores + AD5 Navidad | Regalo antes de la fecha límite de envío |
| 4. Post-Navidad | desde 15 dic | bajar o pausar | Retargeting | Según margen |

**Gasto máximo de referencia:** unos 140 € en la fase 1, 150 € en la 2 y 300–500 € en la 3.
Solo se sube si las reglas de la sección 7 lo permiten.

**Oferta de Black Friday** (crear un descuento automático en Shopify): **-15 % en todas las
camas Nino** del 27-11 al 1-12, o el código `NINO15`. Calcula antes con tu coste que el -15 % no
te deja sin margen.

---

## 7. Reglas de optimización (qué mirar y cuándo tocar)

**No tocar nada durante las primeras 72 horas.** Cada cambio grande reinicia el aprendizaje.

| Métrica (en Meta) | Bien | Alarma | Acción |
|---|---|---|---|
| CTR de enlace | > 1,2 % | < 0,7 % tras gastar 15 € en el anuncio | Pausar ese anuncio |
| CPC de enlace | < 0,60 € | > 1,20 € | Cambiar el gancho o la imagen |
| Frecuencia (7 días) | < 2 | > 3 | Meter creatividades nuevas |
| Coste por añadido al carrito | < 12 € | > 25 € | Revisar precio y ficha |
| Visita → carrito (Shopify) | > 8 % | < 3 % | El problema está en la ficha, no en el anuncio |
| Carrito → compra | > 25 % | < 10 % | Revisar el pago: envío, plazos, confianza |
| CPA (coste por compra) | < CPA máximo | > 1,5 × CPA máximo | Pausar o cambiar creatividades |

**Reglas fijas:**
- Si llevas gastado **2 × el CPA máximo sin ninguna compra pero con carritos**, aguanta: el
  problema está en la ficha o el pago. Revisa la sección 3.
- Si llevas gastado **2 × el CPA máximo sin compras ni carritos**, el anuncio no conecta. Cambia
  las creatividades.
- Para **escalar**, sube como máximo un 20–30 % cada 2–3 días si el CPA está por debajo del
  máximo.
- Si en 7 días hay muy poca entrega (Meta no consigue gastar), cambia temporalmente el evento a
  **Añadir al carrito**. Vuelve a Compra cuando haya más de 10 compras.

---

## 8. Creatividades

> ⚠️ **No uses las infografías del proveedor tal cual.** Tienen el texto en **francés** y el logo
> **"Purré"**. Rehazlas en español en Canva con el logo de RiojoHome. Las fotos de ambiente
> (bulldog en el salón, golden en la terraza) sí sirven. En diciembre, mejor las de interior.

### AD1: "El más bonito de tu salón" (estático 4:5)
- Imagen: el bulldog francés durmiendo en la cama de pana, en un salón luminoso.
- Texto sobre la imagen: **"Su rincón favorito. El más bonito de tu salón."** y debajo
  "Envío gratis · Desde 74,90 €".

### AD2: "Invierno" (estático 4:5)
- Imagen: la cama vacía en primer plano, con textura de pana, o el perro acurrucado.
- Texto sobre la imagen: **"Este invierno, que no duerma en el suelo frío ❄️"**.

### AD3: Carrusel de 5 tarjetas
1. Bulldog en el salón: "Cama Nino de pana"
2. Primer plano de la pana: "Pana aterciopelada de 350 g/m²"
3. Cremallera de la funda: "Funda lavable a 30 °C"
4. Esquema de tallas XS–XL: "Mídelo tumbado y elige su talla"
5. Golden retriever: "Classic o Memory Foam: tú eliges"

### AD4: Reel de 15 s (9:16)
Lo ideal es grabarlo con un perro de verdad (tuyo o de un amigo). Si no, monta las fotos con
zoom suave y texto.

| Segundos | Imagen | Texto en pantalla |
|---|---|---|
| 0–2 | Perro durmiendo en el suelo o en un cojín plano | "¿Tu perro duerme así? 👀" |
| 2–5 | Se sube a la cama Nino y se acurruca | "Mejor así 🐶💤" |
| 5–8 | Primer plano de la pana y del borde acolchado | "Borde acolchado en los 4 lados" |
| 8–11 | Abrir la cremallera de la funda | "Funda lavable a 30 °C" |
| 11–15 | Plano del salón con la cama | "Envío gratis · riojohome.com" |

Música: tendencia tranquila o acústica de la biblioteca de Meta.

### AD5: Navidad (a partir del 2-12)
- Imagen: la cama con un lazo rojo o una mantita navideña.
- Texto sobre la imagen: **"El regalo que sí va a usar 🎁"** y debajo "Pide antes del XX/12".

---

## 9. Textos de los anuncios

### Textos principales

**Texto A (decoración + perro):**
> 🐾 El rincón favorito de tu perro… y el más bonito de tu casa.
>
> La cama Nino en pana beige vainilla tiene un borde acolchado en los 4 lados para que se
> acurruque y apoye la cabeza, y queda preciosa en el salón.
>
> ✔️ Funda con cremallera, lavable a 30 °C
> ✔️ Pana resistente de 35.000 ciclos Martindale
> ✔️ Classic o Memory Foam
> ✔️ Envío gratis a España
>
> 👉 Elige su talla (XS a XL) y dale el descanso que se merece.

**Texto B (invierno):**
> ❄️ Llega el frío y el suelo no es sitio para dormir.
>
> La cama Nino lo envuelve con su borde acolchado y su pana aterciopelada para que pase el
> invierno calentito y en su sitio (y no en tu sofá 😅).
>
> Funda lavable · Memory Foam opcional para perros grandes o mayores · Envío gratis.

**Texto C (problema → solución, lavable):**
> ¿Pelos, barro y babas? 🐶
> La funda de la cama Nino se quita con cremallera y va a la lavadora a 30 °C. Siempre limpia y
> siempre bonita.
>
> Pana beige vainilla · Fabricada en Europa · Envío gratis a España.

**Texto Black Friday (27-11 a 1-12):**
> 🖤 BLACK FRIDAY: -15 % en la cama Nino
> Solo hasta el lunes. Su rincón favorito, más bonito y más barato que nunca.
> Envío gratis a España 🐾

**Texto Navidad:**
> 🎁 Este año, el regalo que sí va a usar (todos los días).
> Cama Nino de pana con funda lavable y envío gratis. Pide antes del XX/12 y llega para Navidad.

### Titulares (para probar varios)
1. Cama Nino de pana · Envío gratis
2. Su rincón favorito, desde 74,90 €
3. Que no duerma en el suelo frío
4. Funda lavable a 30 °C
5. El regalo que sí va a usar 🎁

### Descripción
"Envío gratis a España · Devolución en 14 días"

### Botón
**Comprar**

---

## 10. Lista de comprobación del lanzamiento

- [ ] Política de devoluciones publicada
- [ ] Plazo de entrega y "Envío gratis" visibles en la ficha
- [ ] Precios redondeados y medidas de la XL publicadas
- [ ] Pie de página cambiado
- [ ] Compra de prueba con la variante de pana hecha y reembolsada
- [ ] Coste del proveedor por talla apuntado y CPA máximo calculado
- [ ] Creatividades en español, sin el logo de Purré ni texto en francés
- [ ] Campaña de Ventas con el evento Compra del píxel 1863401214833955
- [ ] Canarias, Ceuta y Melilla excluidas
- [ ] URL con `?variant=54000292987216` y parámetros UTM puestos
- [ ] Descuento de Black Friday creado en Shopify (programado del 27-11 al 1-12)
- [ ] Recordatorio para revisar los datos a las 72 h (23-11) y cada 2–3 días después
