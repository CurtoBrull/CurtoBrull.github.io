`2020-07-12 14:17:33 Sunday`

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

# Curso de Desarrollo Web Online

Curso Básico de 6 horas de contenido.

> En este curso, Leonidas Esteban te da una introducción al mundo del desarrollo web que te será de mucha utilidad, tanto si quieres convertirte en un programador Backend, como si tu objetivo es ser un programador Frontend. Aprenderás a codificar los documentos necesarios para que tu sitio web se vea y se pueda acceder a través de internet.

* [Curso de Desarrollo Web Online]( https://platzi.com/clases/html5-css3/ "Curso de Desarrollo Web Online")


## Atributos HTML
Los atributos son valores agregados a las etiquetas (tags) html que extienden su habilidad o funcionalidad con información específica.

A continuación, un ejemplo de los atributos más comunes y usados en algunas etiquetas:

Para **img:**

**src:** específica la ruta de la imagen que será mostrada a través de esta etiqueta. La ruta puede ser absoluta (cunado especifica una dirección exacta, incluyendo el prefijo http(s) ) o relativa (cuando la referencia a la ubicación de la imagen parte de la ubicación del archivo actual).

**alt:** indica un texto alternativo que será mostrado en lugar de la imagen cuando ésta no pueda ser mostrada.

**width:** ancho de la imagen en pixeles.

**height:** alto de la imagen en pixeles.

Para **link**, en la cabecera head del documento:

**rel:** indica la relación del recurso con el contenido.

**type:** indica el tipo de recurso / formato.

**href:** indica la ubicación (url) del recurso enlazado.

Para **meta**, también en la cabecera head del documento:

**charset:** indica la tabla de caracteres (utf-8 para caracteres latinos) usada en el documento.

Para **a:**
**href:** la ubicación o ruta a la que enlaza esta etiqueta de ancla. En el caso de querer enlazar a elementos que se encuentran dentro del mismo documento, este atributo debe indicar el valor del atributo ““id”” de ese elemento destino del enlace.

## Formularios HTML

Los Formularios en html son unidades de información que nos permiten recolectar información para enviarlos al propietario del website o a un servicio externo. Esta formado por dos partes o contextos: una parte donde se hace el ingreso y modelación de esos datos (en el frontend), y otra parte que se encarga de enviar, procesar y almacenar esos datos (en el backend).

Los formularios se crean con la etiqueta **form**. El atributo principal de un formulario es **action**, ya que contiene la ruta a la que serán enviados los datos recolectados.

Hay diversos elementos html que permiten la captura o recolección de datos, aunque generalmente se usan los elementos creados con la etiqueta **input**. Los inputs también sirven para crear botones, aunque existe una etiqueta especial para ésto llamada **button**… El atributo principal de los inputs es **type**, que indica el tipo de comportamiento o dato que se espera recibir.

Los elementos creados con la etiqueta **label** muestran un texto que se puede asociar con un input para darle mayor significado al campo, principalmente cuando no se usa el atributo **placeholder**.

## Formas de agregar estilos a HTML

Hay tres opciones para incluir estilos que definan la apariencia de tu html:

Estilos **en línea**: se definen directamente en el elemento html que quieres estilizar, se agregan con el atributo **style**.

Estilos con el **tag Style**: regularmente este tag se incluye dentro de la etiqueta head del html.

Estilos enlazados desde un archivo **css externo**: utilizando la etiqueta **link** que nos permite enlazar recursos externos.

A CSS, se le llama hojas de estilos en cascada porque los estilos que se definen para una página, se van aplicando de arriba hacia abajo, y de lo más general a lo más particular, teniendo prioridad lo más particular. Esto es, los estilos que prevalecen son los que han sido definidos en línea, luego los que fueron definidos mediante la etiqueta style en la cabeza o cuerpo del html, y por último los estilos definidos en archivos externos enlazados con la etiqueta link. Esta prioridad se puede alterar al usar el modificador **!important** en la definición de algún estilo en particular, aunque esto no es recomendado.

## Bordes

Todos los elementos html admiten la propiedad de css border, que define la apariencia que tendrá el contorno del componente.
El borde puede ser de muchos estilos, y al igual que las propiedades margin y padding que aprenderás más adelante, a los bordes se les puede colocar estilos tanto de forma general con la propiedad border, como de acuerdo al lado del elemento que se indique: **border-top, border-right, border-bottom y border-left**.

Con la propiedad **boder-radius** se define el redondeado de las esquinas de los bordes.

## Márgenes

Los márgenes en CSS son el espacio que separa a los elementos html entre sí. Hay elementos de html que traen márgenes predefinidos (por defecto) en los estilos propios del navegador como el caso de: body, h1, h2, h3, h4, h5, h6, ol, ul, li, p, y muchos otros.

Cuando hay dos márgenes de elementos diferentes que colindan entre sí, se presenta una situación llamada **“margin collapsing”** en la que el mayor margen de los dos se superpone al otro.

Se puede asignar una medida de margin para los cuatro lados del elemento, o márgenes individuales para cada uno de los lados con: **margin-top, margin-right, margin-bottom y margin-left.**

Se puede centrar un elemento html colocándole el valor de **margin: 0 auto**, cuando dicho elemento tiene **display block**.

## Tipos de display

Display es la propiedad de css que indica cómo debe ser mostrado un elemento html. Todos los elementos tienen algún tipo de display. Si un elemento no se ve en pantalla es porque seguramente su display es **none**.

Los valores más comunes que puede recibir la propiedad display son:

**block**: el elemento intenta abarcar todo el ancho posible.
**inline**: reduce su tamaño exclusivamente hasta lo que abarca su contenido, descartando las propiedades width y height.
**inline-block**: combina lo mejor de block e inline, ya que respeta las dimensiones indicadas en las propiedades width y height, pero coloca el elemento en línea (al costado) de elementos hermanos que también tengan display: inline o inline-block.
**flex**: asume algunas propiedades por defecto que favorecen la alineación de los elementos internos.
**grid**: similar a flex, asume algunas propiedades por defecto organizando los contenidos en filas y columnas.
**none**: oculta el elemento.

## Propiedades de flexbox

Flexbox se refiere al tipo de display en css que permite un manejo flexible de la alineación, dimensionamiento y distribución de elementos html.

Esta propiedad se aplica a un elemento padre, pero va a afectar principalmente a sus elementos hijos directos. Por defecto, los elementos internos quedan alineados unos seguidos de los otros. El comportamiento del modelo de caja de estos elementos hijos también se ha modificado, ya que pierden el efecto de su propiedad margin.

Los elementos hijos de un padre con propiedad display: flex tienen a su disposición algunas nuevas propiedades que aportan mayor flexibilidad a su comportamiento. Una de estas propiedades es **flex-shrink** que, junto a la propiedad **flex-wrap** del padre, permite adaptar y distribuir los elementos de manera dinámica en el espacio horizontal disponible hasta ocupar todo el espacio, y luego pasar a ocupar dinámicamente las siguiente filas hacia abajo.

## Alineando elementos de forma horizontal

La propiedad de css que nos permite definir la forma en que se alinearán o distribuirán los hijos de un elemento al que se le ha asignado un display flex es: **justify-content**. Y puede tomar entre otros valores, los siguientes:

**flex-start**: para alinear todos los elementos hacia el inicio del espacio disponible.
**flex-end**: para alinear todos los elementos hacia el final, a la derecha.
**center**: para alinear todos los elementos al centro del espacio disponible.
**space-between**: para distribuir los elementos con un espacio proporcional e igual entre ellos.
**space-evenly**: para distribuir los elementos con un espacio proporcional e igual entre ellos (incluyendo el primer y último elementos con respecto a los extremos del espacio disponible).
**space-around**: similar a space-evenly pero tanto en el primero como en el último elemento, el espacio hacia los extremos es la mitad del espacio usado entre los elementos.

## Alineando elementos de forma vertical

Similar a como sucede con justify-content, es posible alinear y distribuir los elementos internos en el espacio vertical disponible usando la propiedad **align-items**, que puede tomar también los valores de: **flex-start, flex-end y center**.

Algo que es muy importante y se debe tener en cuenta a la hora de usar align-items y justify-content es que **dependiendo de la propiedad flex-direction que se haya definido, el efecto de ambos se invierte**, no en cuanto a sus elementos internos, sino en cuanto a si se debe usar uno u otro de manera vertical u horizontal.

**IMPORTANTE**: Cuando la propiedad flex-direction se ha definido como column, la propiedad justify-content ya no va a aplicar sobre la alineación horizontal, sino sobre la vertical. Y align-items ya no aplicaría sobre la alineación vertical sino la horizontal. Se intercambian sus efectos.

Para centrar completamente los elementos internos de manera vertical y horizontal en su elemento padre, debemos usar el valor center en ambas propiedades.

# Conceptos elementales de Responsive Design

Para abordar el campo del Responsive Design es necesario que tengas claridad sobre algunos conceptos básicos.

Por este motivo, durante esta clase aprenderás qué es el Responsive Design, cuáles son los lenguajes de programación que lo hacen posible, qué medidas son necesarias aplicar para lograr que tus proyectos se adapten a pantallas de diversas medidas y condiciones, cuáles son los principios del Responsive Design (mostly fluid, colocación de columnas, layout shifter, tiny tweaks, off canvas).

Finalmente, aprenderás el objetivo principal del Responsive Design: la óptima visualización de las web sites en cualquier dispositivo y podrás tener referentes en www.mediaqueri.es .

# Patrones en Responsive Desing:

## Mostly Fluid:

El patrón Mostly fluid consiste, principalmente, en una cuadrícula fluida. Por lo general, en las pantallas grandes o medianas se mantiene el mismo tamaño y simplemente se ajustan los márgenes en las más anchas.
En las pantallas más pequeñas, la cuadrícula fluida genera el reprocesamiento del contenido principal, mientras que las columnas se apilan verticalmente. Una de las mayores ventajas de este patrón es que, en general, solo se necesita un punto de interrupción entre las pantallas grandes y las pequeñas.

## Colocación de columnas:

En el caso de los diseños con varias columnas de ancho completo, durante el proceso de colocación de columnas éstas únicamente se colocan de forma vertical debido a que el ancho de la ventana es demasiado reducido para el contenido.
En un momento dado, todas las columnas se apilan verticalmente. La selección de puntos de interrupción para este patrón de diseño depende del contenido y cambia para cada diseño.

## Layout shifter:

El patrón Layout shifter es el más adaptable, ya que posee varios puntos de interrupción en diferentes anchos de pantalla.
La clave para este diseño es el desplazamiento del contenido, en lugar de su reprocesamiento y colocación debajo de otras columnas. Debido a las diferencias significativas entre cada punto de interrupción principal, es más complejo de mantener, y es posible que se deban realizar cambios dentro de los elementos, no solo en el diseño de contenido general.

## Tiny tweaks:

El patrón Tiny tweaks permite realizar pequeños cambios en el diseño, como ajustar el tamaño de la fuente, cambiar el tamaño de las imágenes o desplazar el contenido de maneras muy poco significativas.
Funciona correctamente en diseños con una sola columna, como los sitios web lineales de una sola página y los artículos con mucho texto.

## Off canvas:

En lugar de apilar contenido verticalmente, el patrón Off canvas coloca contenido menos usado (tal vez menús de navegación o de apps) fuera de la pantalla y solo lo muestra cuando el tamaño de la pantalla es suficientemente grande. En las pantallas más pequeñas, el acceso al contenido es posible con solo a un clic.

# Media queries

Para que logres los resultados que deseas en tus proyectos, es necesario cambiar ciertas propiedades para modificar el tamaño de los textos, contenidos y hojas de estilo; la manera de hacer esto es el media queries.

El media queries es un módulo de css que hace posible al responsive design, éste existe desde el 2010 y se encarga de adaptar la representación del contenido a características del dispositivo.

En esta clase conocerás cómo funciona su estructura, cómo se construye y adquirirás los conocimientos necesarios para trabajar con él, desde tu editor de código.

**@media media type and (condición) {} // @media screen and (max-width:800px) and (min-width:400px) {}**

## Movile First: 

@media screen and (min-width:320px) {}
@media screen and (min-width:480px) {}
@media screen and (min-width:768px) {}
@media screen and (min-width:1024px) {}

## Desktop First:

@media screen and (max-width:1024px) {}
@media screen and (min-width:768px) {}
@media screen and (min-width:480px) {}
@media screen and (min-width:320px) {}

Link en HTML:

    <link rel="stylesheet" href="./css/media.css" media="screen and (max-width:786px)"/>
    
# CSS Positions

**static**: es la propiedad por defecto.

Con las otras opciones, se activan las propiedades de top, bottom, left, right y z-index.

**relative**: El objeto se mueve en base al lugar donde se encuentra originalmente.

**absolute**: El objeto se ubica de manera absoluta con el elemento más cercano que tenga posición relativa o con el body.

**fixed**: El elemento se muestra de manera fija en el viewport.

**sticky**: El elemento se queda de manera fija una vez que aparece en pantalla.

