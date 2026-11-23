# Bitácora Examen | Paula Inostroza

## Información del proyecto

**Link de Figma:** (https://www.figma.com/design/22OMYk2AjVtOsIJuyRmK0B/Portafolio-Int.-Web?node-id=2-3&t=9m9nFSSsm3kyQrse-1)
**Link Portafolio:** (https://pau-io.github.io/paula-inostroza-portafolio/) 
---

# Avance 1 | 9 de noviembre

## 1. Descripción del proyecto

Diseñaré mi portafolio personal, recopilando distintos proyectos desarrollados durante mi formación universitaria en Diseño Industrial.

Adicionalmente, desarrollaré una versión simplificada de tipo *one-page*, pensada para presentarla como portafolio en una postulación de intercambio semestral. Esta segunda versión tendrá una estética más limpia, una estructura sencilla y una navegación intuitiva, priorizando la presentación de los proyectos y la información personal.

## 2. Estructura y contenido del sitio web

La propuesta inicial contempla cuatro secciones principales:

### 2.1. Home

Pantalla de inicio que presenta los siete proyectos mediante miniaturas interactivas.

**Características e interacciones:**
- **Navbar:** Barra de navegación estática durante todo el recorrido de la página, con un fondo semitransparente que permite visualizar el contenido que se encuentra detrás.
- **Título central (PIO):** Al pasar el cursor sobre cada letra, aparece el nombre correspondiente y las letras realizan un pequeño movimiento.
- **Miniaturas:** Se desplazan ligeramente de manera automática, generando movimiento en la composición.
- **Interacción con miniaturas:** Al pasar el cursor sobre cada una, aumenta ligeramente su tamaño y el cursor muestra el mensaje «¡Mírame!».

### 2.2. Página principal | Proyectos

Sección que reúne cuatro proyectos individuales y tres proyectos grupales.

**Características e interacciones:**
- Cada proyecto cuenta con una composición visual y descriptiva propia.
- A la derecha de cada proyecto se incorpora un carrusel o slideshow de imágenes.
- Los carruseles se desplazan automáticamente y cumplen una función exclusivamente visual, sin actuar como botones de navegación.

### 2.3. Sobre mí

Sección integrada dentro de la página principal, destinada a presentar información personal.

**Características:**
- Contiene una breve presentación personal.
- Incorpora un carrusel o slideshow de imágenes en la parte inferior.
- Incluye la información de contacto.

### 2.4. Galería de proyectos

Página adicional que reúne fotografías correspondientes a los distintos proyectos y a la que se accede mediante la opción «Galería» del navbar.

**Características e interacciones:**
- Las fotografías se presentan en una composición visual continua.
- La galería permite desplazarse libremente mediante el cursor.
- El movimiento es infinito, sin un punto de inicio ni de término definido.
- Las fotografías cumplen una función visual y no actúan como botones de navegación.

---

## 3. Referentes web

Para desarrollar la propuesta visual y funcional del portafolio, seleccioné distintos sitios web como referentes. Estos se agrupan según las características que me interesa rescatar de cada uno.

### 3.1. Navbar y navegación

**[Collletttivo](https://www.collletttivo.it/)**

Me interesa la forma en que el navbar utiliza un fondo semitransparente, permitiendo visualizar el contenido que se encuentra detrás. Aunque en el sitio de referencia la barra no permanece estática, me gustaría incorporar esta característica en mi propuesta para mantener el acceso a la navegación durante todo el recorrido, sin necesidad de volver al inicio de la página.

### 3.2. Diagramación y disposición de elementos

**[Portafolio GV | Behance](https://www.behance.net/gallery/240508821/Portafolio-GV)**

Aunque este portafolio no corresponde a una página web tradicional, ya que

# Desarrollo del Examen

## 1. Desarrollo y decisiones de diseño

Debido a problemas personales, falta de tiempo y la carga académica de los demás ramos, no fue posible diseñar la versión mobile del sitio. Por esta razón, para esta instancia desarrollé únicamente la versión desktop, procurando que fuera responsive.

Para comenzar el desarrollo del examen, primero me aseguré de que el diseño en Figma estuviera correctamente construido desde un inicio, utilizando Auto Layout y verificando que no faltara ningún contenido ni imagen.

Durante el proceso, me di cuenta de que la diagramación funcionaba mejor al presentar los proyectos mediante tarjetas desplegables. Esto permitía abrirlas y cerrarlas, evitando que la página quedara demasiado extensa y facilitando la navegación.

Para implementar esta decisión, fue necesario simplificar algunas características del diseño original. Por ejemplo, los slideshows dejaron de ser automáticos y se reemplazaron por cuadrículas de imágenes estáticas.

Por otro lado, diferencié la diagramación y jerarquización de las imágenes dentro de cada tarjeta de proyecto, buscando que el contenido fuera legible y cómodo de visualizar.

Finalmente, simplifiqué la sección **«Sobre mí»**, manteniendo únicamente la información que consideré necesaria.

---

## 2. Desarrollo HTML

Para desarrollar ambos archivos HTML, me basé en los contenidos vistos en clases y en el material de apoyo de HTML y CSS que las profesoras habían compartido.

Durante el proceso tuve dificultades al organizar los párrafos. Inicialmente, al separar cada uno utilizando etiquetas `<p></p>`, la distribución del contenido se alteraba. Por este motivo, opté por mantener un solo párrafo y separarlo mediante dos saltos de línea utilizando `<br><br>`.

Me gustaría profundizar en cómo solucionar este problema a futuro, ya que tengo entendido que utilizar saltos de línea para separar párrafos no es una buena práctica.

---

## 3. Desarrollo CSS

Para desarrollar el CSS, conecté Figma con Claude Code y le solicité que generara el archivo `style.css` desde cero, utilizando mis propios archivos HTML como referencia.

Preferí esta alternativa porque quería obtener un código ordenado y que respetara todas las indicaciones y características de mi diseño.

A continuación, dejo el prompt que utilicé:

### Prompt utilizado en Claude Code

Hola, para mi portafolio web tengo los archivos `index.html` (desktop de Figma) y `galeria.html` (galería desktop de Figma), te los enlazo para que lo revises bien y los uses para escribir el `style.css`. Si cometí algún error, házmelo saber y yo lo edito.

Te voy a explicar paso a paso lo que necesitas saber para escribir el `style.css`:

**Consideraciones:**

- Utiliza tanto el frame Desktop como el Galería Desktop para escribir el CSS. Debe ser completamente fiel.
- Quiero que la interactividad y animaciones que yo te describa puedan lograrse en CSS y solo lo estrictamente necesario sea en JavaScript. Si es así, haz un archivo `script.js` aparte.
- Toma en cuenta el material de apoyo que ya te había subido.
- Todas las medidas deben estar en `rem`.
- Utiliza flex para que pueda ser responsive.
- No utilices `position: absolute`.
- Pon desplazamiento smooth.

**Fonts:**

- En Figma, PIO es Gadugi, cámbiala por Atkinson Hyperlegible en Bold (en Figma utilicé 200pt). Usa el embed code de Google Fonts:

```css
.atkinson-hyperlegible-bold {
    font-family: "Atkinson Hyperlegible", sans-serif;
    font-weight: 700;
    font-style: normal;
}
```

- Para Inter, usa el embed code de Google Fonts y ajusta el font weight según el Figma:

```css
.inter-<uniquifier> {
    font-family: "Inter", sans-serif;
    font-optical-sizing: auto;
    font-weight: <weight>;
    font-style: normal;
}
```

- Para Alte Haas Grotesk, solo conseguí la fuente descargada en formato TTF. Escribe el código usando `@font-face` con la ruta de mi carpeta, que es `assets`.

  Nombres de los archivos en mi carpeta:
  - `AlteHaasGroteskRegular.ttf`
  - `AlteHaasGroteskBold.ttf`

**Desktop:**

Utiliza las variantes de componentes descritas en el UI KIT de Figma.

Nota: El ícono triangular que está al lado de «Examen» ya no lo utilizaré.

- **Encabezado + Navbar:** El encabezado PIO debe redirigir al inicio de la página al hacer clic. Al hacer clic en las secciones del Navbar, estas deben redirigir a su correspondiente sección dentro de la misma página, identificada por el primer elemento descrito en esa parte del HTML. Excepto por la sección de galería, que debe redirigir a `galeria.html` como una página aparte.

- **PIO + Nombres:** PIO no se mueve. Al iniciar la página, luego de 3 segundos, los nombres (Paula, Inostroza y Olmedo) aparecen con una animación de izquierda a derecha y en orden de arriba hacia abajo.

- **Miniaturas:** Cada número debe quedar por detrás de su imagen y posicionarse como aparece en Figma. Cada miniatura debe moverse suavemente en un loop, primero un poco hacia arriba y luego volver hacia abajo. Al pasar el cursor sobre cada miniatura, estas deben hacerse ligeramente más grandes y, al hacer clic, deben redirigir a su correspondiente sección de proyecto.

- **Proyectos:** Al iniciar la página, todas las tarjetas de los proyectos deben estar cerradas. Al hacer clic sobre el número en grande, se debe desplegar la tarjeta con todo el contenido en su interior.

- **Contacto:** El `h2` «¡Hablemos!» debe tener la siguiente animación: al pasar el cursor sobre cada carácter, este se achica a la mitad de su tamaño y luego vuelve a su tamaño original, como si rebotara.

- **Galería:** Las fotografías deben estar ordenadas según la disposición de Figma y desplazarse hacia arriba en un loop infinito, lento y smooth.

Con toda esta información debes escribir el `style.css`, por favor.

Además de escribir el CSS, también generó el archivo `script.js`.

---

## 4. Modificaciones realizadas posteriormente

Durante la revisión del resultado, realicé algunos ajustes directamente en el CSS:

- **Velocidad de la galería:** Me pareció que la animación en loop de la galería estaba demasiado lenta, por lo que busqué en el CSS el código que controlaba su duración y reduje el tiempo de `90s` a `70s`.

- **Ajuste de medidas:** Algunas medidas en `rem` tenían demasiados decimales, por lo que las fui modificando para utilizar valores más estandarizados.

---

## 5. Problemas encontrados durante el desarrollo

Uno de los principales problemas apareció al trabajar con las cuadrículas de imágenes de los proyectos.

En Figma había adaptado las fotografías a las dimensiones de cada rectángulo, pero los archivos originales de mi carpeta `assets` mantenían sus tamaños y proporciones originales. Esto provocó que las cuadrículas de los proyectos 02 y 03 no se visualizaran correctamente al implementar el diseño en HTML y CSS.

Para solucionarlo:

- **Proyecto 02:** Mantuve la cuadrícula como quedó originalmente, pero adapté la alineación para que todas las imágenes quedaran a la misma altura que la imagen principal.
- **Proyecto 03:** Recorté una a una las fotografías desde mi carpeta `assets` hasta conseguir que la cuadrícula se visualizara correctamente.

---

## 6. Aprendizajes y conclusiones

A partir de este proceso, identifiqué algunas prácticas que considero importantes para futuros desarrollos web:

- **Adaptación de imágenes:** Considero que es una buena práctica preparar las fotografías según las dimensiones y proporciones en las que se utilizarán dentro de la página web. Esto permite evitar problemas de ancho, alto y composición de las imágenes.

- **Organización de párrafos:** Aprendí que es preferible separar los párrafos utilizando etiquetas `<p>` independientes y controlar su espaciado mediante CSS, en lugar de recurrir a múltiples etiquetas `<br>`.

- **Organización del código:** Comprendí la importancia de mantener una estructura HTML ordenada, con contenedores y clases que permitan controlar los elementos del css.

