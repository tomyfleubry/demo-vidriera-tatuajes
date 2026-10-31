---
name: Casa Tinta
description: Repertorio de obra enmarcada para una vidriera ficticia de tatuajes y piercing.
colors:
  bone: "#F4F1EC"
  ink: "#16130E"
  red: "#B3352B"
  stone: "#8A8378"
  paper: "#fffdfa"
typography:
  display:
    fontFamily: "Bebas Neue, sans-serif"
    fontSize: "96px"
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: "-0.015em"
  display-mid:
    fontFamily: "Bebas Neue, sans-serif"
    fontSize: "88px"
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: "-0.015em"
  display-tablet:
    fontFamily: "Bebas Neue, sans-serif"
    fontSize: "76px"
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: "-0.015em"
  display-mobile:
    fontFamily: "Bebas Neue, sans-serif"
    fontSize: "80px"
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: "-0.015em"
  headline:
    fontFamily: "Bebas Neue, sans-serif"
    fontSize: "64px"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "-0.015em"
  headline-mobile:
    fontFamily: "Bebas Neue, sans-serif"
    fontSize: "52px"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "-0.015em"
  title:
    fontFamily: "Bebas Neue, sans-serif"
    fontSize: "36px"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "-0.015em"
  artist-title:
    fontFamily: "Bebas Neue, sans-serif"
    fontSize: "42px"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "-0.015em"
  work-title:
    fontFamily: "Bebas Neue, sans-serif"
    fontSize: "30px"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "-0.015em"
  body:
    fontFamily: "Manrope, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
  hero-lead:
    fontFamily: "Manrope, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.65
  action:
    fontFamily: "Manrope, sans-serif"
    fontSize: "14px"
    fontWeight: 700
    lineHeight: 1.4
  action-mobile:
    fontFamily: "Manrope, sans-serif"
    fontSize: "13px"
    fontWeight: 700
    lineHeight: 1.4
  caption:
    fontFamily: "Manrope, sans-serif"
    fontSize: "13px"
    fontWeight: 400
    lineHeight: 1.6
rounded:
  photo: "6px"
  panel: "18px"
  capsule: "999px"
  circle: "50%"
spacing:
  xs: "8px"
  sm: "12px"
  caption: "16px"
  compact: "20px"
  md: "24px"
  panel: "28px"
  lg: "32px"
  gutter-desktop: "40px"
  section-mobile: "68px"
  section-desktop: "96px"
components:
  button-primary:
    backgroundColor: "{colors.red}"
    textColor: "{colors.bone}"
    typography: "{typography.action}"
    rounded: "{rounded.capsule}"
    padding: "14px 24px"
    height: "50px"
  button-primary-hover:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.bone}"
  button-secondary:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    typography: "{typography.action}"
    rounded: "{rounded.capsule}"
    padding: "14px 24px"
    height: "50px"
  button-secondary-hover:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.bone}"
  button-mobile:
    typography: "{typography.action-mobile}"
    padding: "14px 20px"
    height: "48px"
  filter:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.capsule}"
    padding: "10px 20px"
    height: "44px"
  filter-selected:
    backgroundColor: "{colors.red}"
    textColor: "{colors.bone}"
  price-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.panel}"
    padding: "28px"
  navigation:
    backgroundColor: "{colors.bone}"
    textColor: "{colors.ink}"
  faq:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    padding: "22px 0"
  whatsapp-floating:
    backgroundColor: "{colors.red}"
    textColor: "{colors.bone}"
    rounded: "{rounded.circle}"
    height: "58px"
    width: "58px"
---

# Design System: Casa Tinta

## Overview

**Creative North Star: "Repertorio de obra enmarcada"**

Este documento se estableció antes de implementar index.html. La presente
ampliación conserva esa dirección y la reconcilia con los tokens, componentes
y estados de la implementación final; no inicia una identidad nueva.

Un repertorio de piezas impresas, elegido con calma: titulares de afiche,
fotografía de oficio grande, estante de estilos y ficha clara por artista.
Hueso, tinta cálida y rojo sostienen una vidriera limpia y profesional.
Bebas Neue aporta la voz de afiche; Manrope permite leer y decidir sin esfuerzo.
El trabajo manda, con superficies planas y fotografías en marcos sencillos.

La dirección acordada excluye estética oscura recargada, máquinas decorativas,
recortes flotantes, reseñas inventadas y video de fondo. La fotografía muestra
el oficio sin atribuir un portfolio real a la marca ni a los artistas ficticios.

**Key Characteristics:**

- Titulares de afiche y cuerpo de lectura claro.
- Fotografía ilustrativa de oficio en marcos limpios.
- Superficies cálidas y planas, con rojo reservado a acción y selección.
- Galería manual, controles nativos y contenido visible por defecto.

## Colors

La paleta contrapone una base cálida de papel con tinta profunda y un único
acento rojo. Los valores normativos están en el frontmatter y corresponden
a las propiedades de la raíz del CSS.

### Primary

- **Rojo tinta** (red): botones primarios, filtro seleccionado, números del
  proceso, precios y foco visible. También colorea el punto de la marca.

### Neutral

- **Hueso** (bone): fondo general y texto claro sobre tinta o rojo.
- **Tinta cálida** (ink): texto corrido, cierre, footer y estados de interacción.
- **Piedra** (stone): texto secundario y créditos sobre el footer oscuro.
- **Papel claro** (paper): sección de artistas y FAQ, filtros inactivos,
  botones secundarios y paneles de precio.

**The Piedra Rule.** Piedra se usa como texto secundario sobre tinta; el texto corrido de las superficies claras va en tinta.

## Typography

**Display Font:** Bebas Neue (sans-serif), peso regular.
**Body Font:** Manrope (sans-serif), pesos 400, 500, 600 y 700.

La combinación conserva el carácter de afiche de la marca sin convertir el
cuerpo en una pieza ornamental. Los titulares no mezclan familias ni palabras
en itálica; el texto y los botones usan voseo.

### Hierarchy

- **Display:** titular del hero en dos líneas explícitas. Usa display sobre
  1050 px, display-mid entre 851 y 1050 px, display-tablet entre 601 y 850 px,
  y display-mobile hasta 600 px. La escala final es 96 / 88 / 76 / 80 px.
- **Headline:** títulos de sección; headline en escritorio y tablet,
  headline-mobile hasta 600 px. El cierre usa una escala propia de
  90 / 78 / 72 px, con interlínea de .94 y ancho de 7ch, ampliado a 9ch en móvil.
- **Title:** base de título de panel. Los nombres de artistas usan artist-title,
  las piezas work-title. El proceso usa 30 px, 27 px hasta 1050 y 31 px hasta
  600, con interlínea 1.05; el panel de precio pasa de 36 a 32 px en móvil.
- **Body:** cuerpo a 16 px con interlínea 1.6 y máximo global de 65ch.
  La bajada del hero usa hero-lead y un ancho de 37ch; hasta 850 px baja a 16 px.
  El override final fija en 16 px las bajadas de sección, descripciones de
  artistas, pasos del proceso, respuestas FAQ, párrafo de cierre y aclaración
  de precios, incluso en móvil.
- **Action / supporting copy:** botones a 14 px y 13 px hasta 600, con peso 700.
  Filtros a 14 / 13 px y peso 600; resumen FAQ a 16 / 15 px y peso 600.
  Tamaños orientativos, estado de filtro, epígrafes y aviso de ficción usan
  13 px; otros metadatos del footer y de precios se mantienen en 13–15 px.
  Estos metadatos no establecen un cuerpo de lectura menor.

**The One Display Voice Rule.** Bebas Neue conserva una sola voz regular en marca y titulares; Manrope lleva lectura, metadatos y acciones.

## Layout

Contenedor centrado con máximo de 1240 px. Los márgenes laterales son 40 px
sobre 850 px, 28 px entre 601 y 850 px, y 22 px hasta 600 px. La separación
principal de secciones es 96 px por lado, reducida a 68 px en móvil; el hero,
precios y cierre tienen sus propios ajustes de ritmo.

| Ancho | Hero y navegación | Grillas y ritmo |
|---|---|---|
| Más de 1050 px | Dos columnas .9fr / 1.1fr con 64 px de separación; foto de 650 px de alto. Header sticky de 80 px y navegación horizontal. | Artistas en tres columnas con 28 px de separación; proceso en cinco. Precios y FAQ en dos columnas. |
| 851–1050 px | Hero con 36 px de separación y foto de 580 px. | Fotos de artistas de 340 px; proceso con 20 px de separación. |
| 601–850 px | Hero aún en dos columnas, separación de 26 px y foto de 540 px. Acciones apiladas. Header de 72 px y menú desplegable. | Artistas aún en tres columnas con fotos de 300 px; proceso en tres. Precios y FAQ pasan a una columna; cierre apilado y footer en dos. |
| Hasta 600 px | Una columna; titular y CTA antes de la foto de 420 px. Acciones en fila con ajuste de línea entre botones. | Artistas en una columna, fotos de 350 px y separación de 42 px. Proceso vertical con 62 px reservados al número. Dos paneles de precio permanecen juntos; footer en una columna. |

Las anclas reservan 104 px superiores. El estante de trabajos y los filtros
tienen desplazamiento horizontal propio; la página no se desplaza lateralmente.
Las tarjetas de galería miden 316 px en escritorio; en móvil dejan ver el
inicio de la siguiente mediante un ancho calc(100% - 34px). Su separación
pasa de 24 a 20 px. El estante usa snap de proximidad, sin forzar cada gesto.

La verificación final local en 1440, 768, 430 y 390 px registró cero overflow,
nueve imágenes resueltas, seis enlaces de WhatsApp y CTA del hero sin salto
de línea. Las capturas completas y los recortes de sección coinciden con
estos estados; el informe de QA local quedó en PASS.

## Elevation & Depth

El sistema no usa sombras. La profundidad proviene de la alternancia entre
hueso, papel y tinta, del tamaño de las fotografías y del espacio. No hay
gradientes, transparencias de vidrio ni bordes usados como decoración.
El header conserva un fondo hueso sólido y el botón flotante se separa con
un borde hueso de 3 px.

**The Flat Surface Rule.** Las superficies permanecen planas; el estado se expresa con color, foco y desplazamientos breves, sin añadir sombras.

## Shapes

Fotografías con esquinas discretas (photo), paneles de precio más suaves
(panel), acciones y filtros en cápsula (capsule), y acceso flotante circular
(circle). La implementación conserva radios distintos por función; no se
uniforman todas las piezas. Los marcos recortan su foto con overflow oculto.
Los íconos son SVG de línea, sin glifos decorativos ni dependencias de fuentes.
WhatsApp usa el símbolo de marca de Bootstrap Icons, relleno en currentColor
y sin trazo agregado; en el flotante su caja es de 27 × 27 px sin encogimiento.
Fuente y licencia MIT: THIRD-PARTY-LICENSES.txt.

## Components

### Buttons

Cápsulas claras y directas. Los primarios usan fondo rojo y texto hueso; los
secundarios papel con tinta; mantienen texto en una línea, ícono de 20 px
y separación de 10 px. El alto del token representa el mínimo del CSS.
En móvil disminuyen el padding horizontal y el alto mínimo según button-mobile.

Hover primario: fondo tinta y elevación de 2 px; active vuelve a su posición.
El secundario pasa a tinta con texto hueso. En el cierre oscuro, el primario
pasa a hueso/tinta y el secundario a rojo/hueso. Transición de fondo y
transformación de .2 s. El foco global es un contorno rojo de 3 px separado
5 px del elemento.

### Filters

Píldoras sin borde: Todos, Tradicional, Blackwork, Línea fina, Color y Realismo.
El filtro seleccionado declara aria-pressed=true y usa rojo/hueso; el inactivo,
papel/tinta. Hover del inactivo usa tinta/hueso; el seleccionado conserva rojo.
Área mínima de 44 px y separación de 8 px.

El clic oculta únicamente las piezas que no coinciden, reinicia el estante
al comienzo y anuncia la cantidad mediante un estado aria-live polite.
Los controles operan con teclado. Sin JavaScript se ocultan los filtros y
permanecen las cinco piezas visibles.

### Galería y artistas

El estante de galería se desplaza de manera nativa y manual, sin reproducción
automática ni flechas falsas. Cada pieza tiene foto 4:5, título y tamaño
orientativo. Hover amplía la foto a 1.035 durante .45 s dentro de su marco.
Las medidas son ficticias y orientativas, no deducidas de la imagen.

Las fichas de artistas son abiertas, sin caja ni sombra: foto, nombre,
especialidad, descripción y consulta individual. Rocco: Tradicional y color;
Vera: Línea fina y blackwork; Santi: Realismo en sombras. Los recortes CSS
conservan posiciones propias: Rocco 50% 28%, Vera 50% 35%, Santi 65% 42%.

### Navigation

Header sticky con marca Bebas y punto rojo. La navegación ofrece Trabajos,
Artistas, El proceso y Preguntas; hover cambia a rojo y el foco sigue el
contorno global. Hasta 850 px, un botón de 44 × 44 px controla el menú con
aria-controls, aria-expanded y etiquetas Abrir menú / Cerrar menú.

Los enlaces cierran el menú. Escape lo cierra y devuelve el foco al botón
si estaba dentro de la navegación. Sin JavaScript, el menú permanece visible,
se integra al flujo y el botón se oculta. No hay una navegación que dependa
de la animación para existir.

### Proceso y precios

Lista ordenada de cinco pasos con numeración automática 01–05 en rojo:
Contás tu idea; Diseño y presupuesto; Seña y turno; La sesión; Cuidados
posteriores. Los números miden 56 px, reducidos a 45 px en móvil; pasan
del bloque superior a una columna lateral.

Los paneles de precio usan papel, radio panel y padding de 28 px
(23 px verticales / 20 px horizontales en móvil). Los precios destacan en
Bebas y rojo, a 48 px y 43 px en móvil. El contenido ficticio es exacto:
Chico, Hasta 5 cm, desde $40.000; Mediano, Hasta 12 cm, desde $90.000;
Grande o manga, Se cotiza por sesiones. La aclaración permanece visible:
"El precio final depende del diseño, el tamaño y la zona; se confirma antes de señar."
No hay CTA de cobro ni importe de seña inventado.

### FAQ

Seis details/summary nativos, sin cajas ni bordes decorativos. El SVG de más
gira 45 grados al abrir; el resumen conserva el foco visible y el contenido
se opera y lee sin JavaScript. La separación vertical es 22 px (20 en móvil),
con la respuesta a 18 px del resumen.

Se preserva el contenido exacto implementado:

| Pregunta | Respuesta |
|---|---|
| ¿Cómo funcionan la seña y la reprogramación? | La seña confirma tu turno. Te explicamos las condiciones antes de señar. Si necesitás mover la fecha, avisá cuanto antes para coordinar una nueva disponibilidad. |
| ¿Cuál es la edad mínima? | Atendemos únicamente a mayores de 18 años, sin excepciones. Traé tu documento a la sesión. |
| ¿Hacen cover up? | Sí. Revisamos el tatuaje que querés cubrir y evaluamos las opciones según su tamaño, la tinta y la zona. La propuesta y el presupuesto se conversan antes de confirmar. |
| ¿Me explican los cuidados posteriores? | Sí. Al terminar te damos instrucciones por escrito, pensadas para tu pieza. Si después tenés dudas, consultanos antes de cambiar los cuidados indicados. |
| ¿Qué piercings colocan y qué material usan? | Colocamos piercings de lóbulo, hélix y septum con joyería de titanio grado implante. Primero evaluamos la zona y conversamos la colocación y sus cuidados. |
| ¿Puedo ir con alguien? | Podés venir con una persona. Durante la sesión, tu acompañante espera en el área de recepción para que el espacio de trabajo quede despejado. |

### Cierre, footer y WhatsApp

Cierre y footer forman un campo tinta con frase grande, WhatsApp y enlace
a trabajos. El footer conserva nombre, Palermo Soho/CABA, martes a sábado
de 11 a 20 h, Instagram ficticio y aviso completo:
"Vidriera de demostración de Nexvia IA · Marca, personas y datos ficticios."
Tiene padding inferior de 6rem para liberar el botón fijo.

El flotante usa círculo rojo con borde hueso y un SVG de WhatsApp de 27 px:
58 px, a 20 px de los bordes; en móvil 56 px, a 18 px. Hover pasa a tinta.
Los seis enlaces usan el número ficticio 5491100000000, abren una nueva
pestaña con noopener y conservan estos mensajes precargados:

| Origen | Mensaje |
|---|---|
| Hero | Hola Casa Tinta! Quiero reservar un turno y contarles mi idea. |
| Rocco | Hola Casa Tinta! Quiero consultar con Rocco por un tatuaje tradicional o a color. |
| Vera | Hola Casa Tinta! Quiero consultar con Vera por un tatuaje de línea fina o blackwork. |
| Santi | Hola Casa Tinta! Quiero consultar con Santi por un tatuaje de realismo en sombras. |
| Cierre | Hola Casa Tinta! Quiero contarles mi idea y consultar por un turno. |
| Flotante | Hola Casa Tinta! Quiero consultar por un tatuaje o piercing. |

El favicon es un monograma CT vectorial propio sobre rojo tinta.
No existen inputs, formularios, checkout, estados de pago ni cobros reales.

### Movimiento y alternativa estática

GSAP 3.12.5, ScrollTrigger y Lenis 1.1.14 se cargan por CDN. La única
coreografía de entrada pertenece al hero y ocurre una vez: foto desde escala
1.045 durante 1.1 s; titular desde 14 px y opacidad .65 durante .65 s;
acciones desde 8 px y opacidad .8 durante .5 s, con ease power2.out.

El resto del contenido de lectura permanece visible. Los antiguos atributos
data-reveal no tienen animación asociada; no se reintroducen revelados generales.
La selección de filtro responde al visitante sin transición de entrada o salida.
Lenis usa duración .9 y sincroniza ScrollTrigger; las anclas conservan el
despeje superior. No hay autoplay ni pin largo.

Con prefers-reduced-motion se evita Lenis y GSAP, se desactivan animaciones
y transiciones CSS, y el scroll es directo. El contenido es visible por defecto;
enlaces, galería manual y FAQ no dependen de GSAP. La grabación recorre la
web real a 430 × 932 mediante el script existente, sin IA y con primer cuadro
verificado; no es video de fondo ni una fotografía generada.

### Fotografías

Todas son fotografías ilustrativas de Pexels, optimizadas a WebP en assets/.
Se revisan marcas, texto ajeno y caras de frente; se usan recortes de trabajo
y perfiles. Los tamaños de las piezas son orientativos ficticios, no medidas
deducidas de la fotografía. La marca y los artistas no son autores reales
de estas fotos. Licencia: https://www.pexels.com/license/

| Archivo | Uso | Autor | Fuente |
|---|---|---|---|
| hero-proceso.webp | Hero, detalle de tatuaje en proceso | Antoni Shkraba | https://www.pexels.com/photo/close-up-photo-of-a-tattoo-artist-tattooing-a-client-7005667/ |
| trabajo-tradicional.webp | Rosa clásica, galería Tradicional | Jan Kopřiva | https://www.pexels.com/photo/close-up-shot-of-tattoo-on-a-person-s-arm-3295586/ |
| trabajo-blackwork.webp | Pieza geométrica, galería Blackwork | Kaboompics | https://www.pexels.com/photo/tattoo-on-an-arm-4750247/ |
| trabajo-linea-fina.webp | Pieza botánica, galería Línea fina | Alex Shimray | https://www.pexels.com/photo/elegant-minimalist-arm-tattoo-design-40444258/ |
| trabajo-color.webp | Mariposa con trazos rojos, galería Color | Alex Shimray | https://www.pexels.com/photo/butterfly-tattoo-on-skin-with-red-accents-40444058/ |
| trabajo-realismo.webp | León en sombras, galería Realismo | jovan curayag | https://www.pexels.com/photo/a-person-with-arm-tattoos-7203283/ |
| artista-rocco.webp | Artista trabajando, mirada baja | Antoni Shkraba | https://www.pexels.com/photo/a-tattoo-artist-tattooing-the-client-arm-7005735/ |
| artista-vera.webp | Tatuadora de perfil | Michael Burrows | https://www.pexels.com/photo/tattooist-making-tattoo-on-body-in-salon-7148025/ |
| artista-santi.webp | Artista inclinado durante la sesión | cottonbro studio | https://www.pexels.com/photo/a-male-tattoo-artist-working-on-a-female-client-5088480/ |

La foto de Rocco se reencuadra para excluir el lateral de una caja con marca;
se mantienen el artista, sus manos y su tarea. No se generan píxeles nuevos.
Las nueve fotos elegidas se descargaron correctamente; no hubo sustituciones
por fallos de descarga. Se descartaron candidatas con letras inglesas visibles
o marcas en la ropa. La candidata 8182253 se sustituyó por 40444058 al detectar
las palabras inglesas TRUTH / FAITH en las cintas del tatuaje durante la
revisión independiente. La foto final de Color pertenece a Alex Shimray.
Créditos accesibles desde el footer mediante el ancla Fotografías.

Cada uno de los nueve WebP conserva su sidecar .webp.json con el campo prompt
de procedencia exacta: autor, URL de origen, licencia y tratamiento realizado.
Ese campo registra origen y transformación; no es un prompt de generación.
El scan de procedencia registra nueve rasters y cero sidecars faltantes.
No se utilizó fotografía generada.

## Do's and Don'ts

### Do:

- **Do** conservar la paleta cálida, los radios por función y la voz regular de Bebas Neue.
- **Do** mantener el cuerpo importante a 16 px y verificar el CTA del hero en una línea.
- **Do** conservar galería manual, foco visible, FAQ nativa y alternativa sin JavaScript.
- **Do** mantener los nueve créditos y la declaración explícita de ficción junto a la vidriera.
- **Do** usar movimiento solo en el hero y respetar prefers-reduced-motion.

### Don't:

- **Don't** añadir sombras, gradientes, vidrio o estética oscura recargada a esta identidad.
- **Don't** atribuir las fotos de stock a Rocco, Vera, Santi o Casa Tinta como portfolio real.
- **Don't** reintroducir letras ajenas, marcas visibles, reseñas inventadas o fotografía generada.
- **Don't** ocultar el cuerpo de lectura detrás de revelados de scroll ni automatizar el estante.
- **Don't** convertir los precios ficticios o la conversación sobre seña en un cobro real.
