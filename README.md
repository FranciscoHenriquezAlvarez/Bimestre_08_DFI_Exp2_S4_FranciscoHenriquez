# Mortal Store 🎮

Proyecto desarrollado progresivamente para la asignatura **Desarrollo Frontend I**.

**Mortal Store** corresponde a una tienda ficticia de videojuegos utilizada como proyecto base para aplicar, semana a semana, los contenidos revisados durante la asignatura.

---

## 📚 Evolución del proyecto

### Semana 01 — Estructura HTML

Durante la primera semana se desarrolló la estructura inicial del sitio utilizando HTML.

Se incorporaron:

- Encabezado principal.
- Menú de navegación.
- Sección de productos.
- Información de contacto.
- Imágenes representativas de los videojuegos.
- Estructura básica del documento HTML.

### Semana 02 — CSS y diseño visual

Durante la segunda semana se incorporó una hoja de estilos CSS externa para mejorar la presentación visual del sitio.

Se trabajó con:

- Hoja CSS externa.
- Modelo de cajas.
- Márgenes y rellenos.
- Bordes.
- Colores.
- Tipografía.
- Selectores CSS.
- Pseudoclases.
- Organización visual del contenido.

### Semana 03 — Flexbox, Grid y diseño responsivo

Durante la tercera semana se mejoró la estructura y adaptabilidad del sitio.

Se incorporaron:

- HTML semántico.
- Flexbox.
- CSS Grid.
- Media Queries.
- Diseño adaptable para escritorio, tablet y móvil.
- Variables CSS mediante `:root`.
- Mejoras de accesibilidad.
- Organización y documentación del código.
- Publicación del proyecto mediante GitHub Pages.

### Semana 04 — Bootstrap 5

Durante la cuarta semana el proyecto fue actualizado mediante **Bootstrap 5**, manteniendo y mejorando los estilos personalizados desarrollados anteriormente.

El objetivo fue incorporar componentes y utilidades del framework para mejorar la estructura responsive, la organización del contenido y la experiencia de navegación.

Se implementaron:

- Bootstrap 5 mediante CDN.
- Navbar responsive.
- Menú colapsable mediante botón hamburguesa.
- Carousel de imágenes.
- Cambio automático del Carousel cada 3 segundos.
- Indicadores y controles de navegación del Carousel.
- Sistema Grid de Bootstrap.
- Cards para representar los productos.
- Distribución responsive mediante breakpoints de Bootstrap.
- Integración de Bootstrap con CSS personalizado.
- Mejoras de accesibilidad y semántica HTML.
- Uso de unidades relativas `rem`.
- Mejora de los estados de foco mediante `focus-visible`.
- Incorporación de `figure` y `figcaption`.

---

## 📱 Diseño responsivo

El sistema Grid de Bootstrap permite adaptar automáticamente los productos según el ancho disponible en pantalla.

Para las columnas de productos se utilizó:

```html
<article class="col-12 col-md-6 col-lg-4">
```

Esto genera la siguiente distribución:

| Dispositivo | Distribución |
|---|---|
| Móvil | 1 producto por fila |
| Tablet | 2 productos por fila |
| Escritorio | 3 productos por fila |

El comportamiento fue comprobado mediante las herramientas responsive de **Google Chrome DevTools** en las siguientes resoluciones:

- Móvil: **390 × 844 px**
- Tablet: **768 × 1024 px**
- Escritorio: **1440 × 900 px**

Las pruebas permitieron verificar que el contenido mantiene su legibilidad, las imágenes conservan sus proporciones y no se producen desbordamientos horizontales.

---

## 🧭 Navbar responsive

La barra de navegación fue implementada utilizando el componente **Navbar de Bootstrap 5**.

En dispositivos de escritorio se muestran directamente los enlaces:

- Inicio
- Productos
- Contacto

En dispositivos con menor ancho, la navegación se transforma automáticamente en un menú colapsable mediante un botón hamburguesa.

La implementación utiliza clases de Bootstrap como:

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
```

También se incorporó el componente `navbar-toggler` para controlar la apertura y cierre del menú.

Se verificó manualmente su correcto funcionamiento tanto al desplegar como al contraer la navegación en dispositivos móviles y tablet.

---

## 🖼️ Carousel

Se incorporó un **Carousel de Bootstrap** para presentar los videojuegos destacados.

El componente incluye:

- Tres imágenes.
- Indicadores de posición.
- Control anterior.
- Control siguiente.
- Cambio automático de imágenes.

El funcionamiento automático fue configurado mediante:

```html
data-bs-ride="carousel"
data-bs-interval="3000"
```

El valor `3000` corresponde a un intervalo de **3 segundos** entre cada imagen.

También se utilizaron controles e indicadores que permiten cambiar manualmente entre las diferentes imágenes del Carousel.

---

## 🃏 Cards de productos

Los videojuegos fueron organizados utilizando el componente **Card de Bootstrap**.

Cada tarjeta contiene:

- Imagen del videojuego.
- Nombre del producto.
- Descripción.
- Estilos personalizados.
- Adaptación automática al sistema Grid.

Entre las clases utilizadas se encuentran:

```html
card
card-img-top
card-body
card-title
card-text
h-100
```

Los productos incluidos en el sitio son:

1. Mortal Kombat 1
2. Minecraft
3. EA Sports FC 26

La clase `h-100` permite mantener una altura consistente entre las tarjetas dentro de una misma fila.

---

## ♿ Accesibilidad y buenas prácticas

Además de Bootstrap, se mantuvieron y mejoraron diferentes prácticas incorporadas durante las semanas anteriores.

Se implementaron:

- HTML semántico.
- Uso de `header`.
- Uso de `nav`.
- Uso de `main`.
- Uso de `section`.
- Uso de `article`.
- Uso de `figure`.
- Uso de `figcaption`.
- Uso de `footer`.
- Textos alternativos mediante `alt`.
- Atributos `aria-label`.
- Atributos `aria-labelledby`.
- Elementos `visually-hidden` de Bootstrap.
- Navegación mediante teclado.
- Estados de foco mediante `focus-visible`.
- Separación entre estructura HTML y presentación CSS.
- Comentarios para identificar las principales secciones del código.

Para reforzar la navegación mediante teclado se incorporó:

```css
a:focus-visible,
button:focus-visible {
    outline: 0.1875rem solid var(--color-enlace);
    outline-offset: 0.1875rem;
}
```

---

## 🎨 CSS personalizado

Bootstrap se utilizó como framework principal para los componentes responsive, pero se mantuvo una hoja de estilos externa para conservar la identidad visual de Mortal Store.

El archivo utilizado es:

```text
css/styles.css
```

En esta hoja se mantienen:

- Variables CSS.
- Colores personalizados.
- Tipografía.
- Estilos del encabezado.
- Personalización de Cards.
- Estilos del pie de página.
- Efectos `hover`.
- Estados `focus-visible`.
- Ajustes del Carousel.
- Media Queries complementarias.

También se priorizó el uso de unidades relativas `rem` en tipografía y espaciados para favorecer la escalabilidad del diseño.

---

## 🛠️ Tecnologías utilizadas

- HTML5
- CSS3
- Bootstrap 5.3.3
- Flexbox
- Bootstrap Grid
- Bootstrap Cards
- Bootstrap Navbar
- Bootstrap Carousel
- Media Queries
- Google Chrome DevTools
- Git
- GitHub
- GitHub Pages

---

## 📁 Estructura del proyecto

```text
Bimestre_08_DFI_Exp2_S4_FranciscoHenriquez/
│
├── index.html
├── README.md
│
├── css/
│   └── styles.css
│
└── img/
    ├── fc26.jpg
    ├── minecraft.jpg
    └── mortal-kombat.jpg
```

---

## 🌐 Publicación

### GitHub Pages

https://franciscohenriquezalvarez.github.io/Bimestre_08_DFI_Exp2_S4_FranciscoHenriquez/

---

