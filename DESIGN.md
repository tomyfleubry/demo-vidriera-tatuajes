---
name: Casa Tinta
description: Galería oscura total, con pedidos por estilo y reserva por artista.
colors: {"ink":"#16130E","bone":"#F4F1EC","red":"#B3352B","panel":"rgba(244,241,236,.045)","muted":"rgba(244,241,236,.78)","whatsapp":"#25D366","white":"#FFFFFF"}
typography: {"display":{"fontFamily":"Bebas Neue, sans-serif","fontSize":"156px","fontWeight":400,"lineHeight":0.87,"letterSpacing":"-.015em"},"headline":{"fontFamily":"Bebas Neue, sans-serif","fontSize":"76px","fontWeight":400,"lineHeight":1,"letterSpacing":"-.015em"},"body":{"fontFamily":"Manrope, sans-serif","fontSize":"16px","fontWeight":400,"lineHeight":1.65},"action":{"fontFamily":"Manrope, sans-serif","fontSize":"14px","fontWeight":700,"lineHeight":1.4},"caption":{"fontFamily":"Manrope, sans-serif","fontSize":"13px","fontWeight":400,"lineHeight":1.6}}
rounded: {"photo":"0px","artist":"6px","pill":"999px","circle":"50%"}
spacing: {"gutter":"40px","gutter-tablet":"28px","gutter-mobile":"22px","section":"88px","section-mobile":"64px"}
components: {"button-primary":{"backgroundColor":"{colors.red}","textColor":"{colors.bone}","typography":"{typography.action}","rounded":"{rounded.pill}","padding":"14px 24px","height":"50px"},"button-secondary":{"backgroundColor":"transparent","textColor":"{colors.bone}","typography":"{typography.action}","rounded":"{rounded.pill}","padding":"14px 24px","height":"50px"},"filter":{"backgroundColor":"{colors.panel}","textColor":"{colors.bone}","padding":"10px 20px","height":"44px","rounded":"{rounded.pill}"},"filter-selected":{"backgroundColor":"{colors.red}","textColor":"{colors.bone}"},"artist":{"backgroundColor":"{colors.panel}","textColor":"{colors.bone}","rounded":"{rounded.artist}"},"whatsapp-floating":{"backgroundColor":"{colors.whatsapp}","textColor":"{colors.white}","width":"58px","height":"58px","rounded":"{rounded.circle}"},"button-secondary-hover":{"backgroundColor":"{colors.panel}","textColor":"{colors.bone}"}}
---

# Design System: Casa Tinta — Galería oscura total

## Overview

**Creative North Star: "Galería oscura total"**

Decisión fijada por Tomas antes de escribir el HTML: tinta de principio a fin,
fotografía de oficio a pantalla completa y una galería densa como protagonista.
El visitante mira un trabajo y abre una consulta que ya nombra su estilo. La
cabecera fija permite llegar a elegir artista con un toque durante el recorrido.
No se traslada este molde a otras vidrieras. Se conserva el contenido del HTML
publicado, sin inventar artistas, estilos, importes ni condiciones.

**Key Characteristics:**
- Hero full-bleed con velo tinta, texto hueso y acción roja.
- Galería a sangre, filtros vigentes y cinco consultas por estilo.
- Tres fichas horizontales de artista con sus mensajes actuales.
- Proceso numerado, carta de precios y FAQ sobre la misma base oscura.

## Colors

Tinta #16130E es el suelo global. Hueso #F4F1EC es el texto, con secundarios
derivados al78% para conservar contraste. Rojo #B3352B es el único acento de
interfaz: acciones, selección, números y foco. Las fichas usan hueso al4.5%
sobre tinta, un tono apenas más claro; no hay tarjetas o secciones claras.
La única excepción expresa es el flotante de WhatsApp: verde #25D366 con ícono
blanco #FFFFFF, como exige el brief. No se usa verde en los otros botones.

**The Dark Ground Rule.** Ninguna sección vuelve a hueso o papel como fondo.

## Typography

Bebas Neue regular para palabra de marca, titulares, nombres y cifras; Manrope
para lectura, datos, filtros y acciones. Se conserva la hoja de Google Fonts.
Portada156px en escritorio;128px hasta1050;112px hasta850; escala móvil de
84–104px según ancho. H2 de76/64/52px. Cuerpo16px/1.65; metadatos13px/1.6.
Acciones14px y objetivos mínimos44px, con texto e ícono sin compresión.
Las frases, titulares, nombres de piezas, estilos, descripciones y respuestas
son los originales. No se usa el acento para colorear palabras sueltas del H1.

## Layout

Orden exacto: hero, galería, artistas, proceso, precios, antes de reservar,
cierre y footer. Contenedor de1240px y márgenes40/28/22px. Anclas104px.

- Hero: foto actual de proceso como fondo absoluto, cover y encuadre65%50%.
  Alto de primera pantalla descontando header80/72px. Velo desde tinta abajo
  hacia transparencia arriba; contenido abajo, sin tarjeta ni foto enmarcada.
  Los dos textos que acompañaban la foto pasan a una línea discreta del hero.
- Galería: fuera del marco estrecho, grilla de seis columnas sin separación
  entre fotos; las dos primeras piezas abarcan tres columnas, las otras dos.
  Fotos grandes en retrato. En móvil una columna, sin scroll lateral de página.
  Pieza, estilo/tamaño y «Quiero algo así» debajo de cada imagen, nunca encima.
  Filtros con su propia fila desplazable y estado accesible como ya existen.
- Artistas: tres tarjetas horizontales oscuras apiladas; fotografía lateral,
  nombre, estilo, descripción y botón actual. Sin cambiar las tres URLs/mensajes.
- Proceso: los cinco pasos existentes en línea, números rojos. En móvil una
  lista vertical simple; se preservan las cinco explicaciones.
- Precios: filas con concepto, tamaño e importe, separadas por filete fino.
  Chico: desde$40.000/hasta5cm; Mediano: desde$90.000/hasta12cm; Grande o manga:
  «Se cotiza por sesiones.». Se mantiene la nota de confirmación antes de señar.
- FAQ: los seis details/summary originales, sin panel claro ni nuevas preguntas.
- Cierre y footer integrados en tinta. Se conserva toda la información, el
  enlace a créditos y el aviso literal de marca/personas/datos ficticios.

## Elevation & Depth

El único velo es fotográfico y funcional en el hero; no hay vidrio ni ruido
decorativo. El flotante usa sombra suave. Las superficies editoriales son planas.
GSAP/ScrollTrigger/Lenis mantienen sus versiones actuales. Entrada coordinada de
hero y revelados leves en galería/artistas desde contenido ya visible. Nada de
autoplay, videos de fondo ni librerías nuevas. Reduced-motion apaga movimiento;
sinJS se ven los cinco trabajos, contenidos y enlaces, con filtros ocultos.

## Shapes

Fotos de galería sin radios ni marcos. Fichas oscuras con6px discretos; controles
de filtro y acciones en pastilla. Flotante circular58px. Separaciones y filetes
organizan texto, sin crear tarjetas de precio.

## Components

### Conversación por trabajo y artista

Cinco enlaces nuevos, uno por trabajo, al teléfono ficticio5491100000000:
`Hola! Vi un trabajo de [ESTILO] en la galería y quiero consultar por un diseño así.`
El estilo es la etiqueta exacta del filtro correspondiente: Tradicional,
Blackwork, Línea fina, Color o Realismo. Se preservan byte a byte los seis
href de WhatsApp actuales (hero, tres artistas, cierre y flotante) y sus textos.
Un acceso de cabecera a Artistas usa ancla interna, sin abrir una consulta nueva.

### WhatsApp: símbolo exacto del brief

El path entregado por Tomas se conserva literalmente en un único symbol
`i-wa` con viewBox0 0 24 24. Cada uso tiene viewBox24×24 explícito, fillcurrentColor,
sin stroke y sin encogerse. No se sustituye por Bootstrap ni se redibuja.
Botones rojos/oscuros: ícono blanco de20px. Flotante: fondo#25D366, ícono blanco
de28px, diámetro58px y sombra suave. Se revisan ampliados sobre página renderizada.

### Selección fotográfica

Todas las fotos se eligen del repo antes de tocar el HTML. Hero: hero-proceso.webp,
1100×1650, detalle de tatuaje en proceso. Se evalúa el fondo renderizado antes de
descargar otra versión; el velo no simula detalle ni crea contenido.
Galería: trabajo-tradicional, trabajo-blackwork, trabajo-linea-fina, trabajo-color,
trabajo-realismo. Artistas: artista-rocco, artista-vera, artista-santi. Se mantienen
las nueve imágenes, sus metadatos de origen y la atribución honesta de stock:
no son artistas ni portfolio de un estudio real. Sin nuevas fotos previstas.

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
- **Do** conservar contenido, seis mensajes existentes y precios exactos.
- **Do** mantener base tinta y contraste hueso legible también en metadatos.
- **Do** probar filtros, cinco pedidos, menú, anclas y FAQ en430px.
- **Do** verificar ampliados los íconos oficiales del flotante y de un botón.

### Don't:
- **Don't** recuperar superficies claras, tarjetas de precios o carruseles.
- **Don't** inventar artistas, estilos, datos, cobros o condiciones de reserva.
- **Don't** atribuir las imágenes de stock a la marca como trabajos reales.
- **Don't** sustituir o simplificar el path de WhatsApp provisto por Tomas.

### Ajustes de la primera inspección

Blackwork usa encuadre CSS 50%100% para priorizar el tatuaje sobre el tramo de piel vacío. No se edita ni sustituye la fotografía. Sin JavaScript, la navegación móvil queda en flujo para no tapar el hero. La foto del hero conserva detalle suficiente como fondo con velo en la captura de1440px: no se descargan imágenes nuevas.

Ajustes de revisión independiente: la línea literal de ubicación se integra a los metadatos debajo de las acciones. En móvil el epígrafe reserva68px a derecha para quedar libre del flotante. El ícono, textos y mensajes no cambian.
