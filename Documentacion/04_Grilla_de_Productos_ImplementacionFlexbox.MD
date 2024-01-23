Actividades
1. Añadiendo ID a la Sección Hero
Comenzaremos por identificar nuestra sección Hero con un ID único, lo que nos permitirá aplicar estilos específicos.

Aplicar ID hero a la Sección:

En tu archivo index.html, agrega el ID hero a la etiqueta <section> que actuará como tu Hero Section, para esto ten en cuenta el mockup final de la web y deduce cuál sería basándote en lo que hemos visto hasta el momento. Por ejemplo:

<section id="hero">
  <!-- Contenido de la Hero Section -->
</section>
2. Añadiendo Fondo a la Hero Section
El fondo es un componente clave que define el tono visual de tu Hero Section.

Establecimiento del Fondo:

En styles.css agrega a la clase que definimos previamente como section el selector ID #hero. De esta manera tendremos mayor especificidad, el navegador aplicará los estilos a una etiqueta section con un id hero.

Luego aplica la imagen de fondo usando background:url('../assets/hero_bg.png');.

Asegúrate de que la imagen cubra toda la sección utilizando background-size: cover; y que esté correctamente posicionada con background-position: top center;.

2. Explicación de Propiedades de Fondo:

background-size: cover; garantiza que la imagen de fondo cubra completamente el área de la sección, independientemente de sus dimensiones originales.

background-position: top center; coloca la imagen en el centro de la sección, alineándola en la parte superior.

3. Añadiendo y Estilizando el Título
El título de la Hero Section debe ser llamativo y estar claramente visible.

Estilización del contenedor del título: Agrega al contenedor del título (<div class="container"></div>) la propiedad display: flex para poder alinear el título. Para esto agrega las siguientes propiedades con los valores que logren dejar el título a la izquierda en el centro: align-items y justify-content.

Inserción y Estilización del Título: Agrega el título dentro de un div con la clase title-container en tu index.html. Por ejemplo: <div class="title-container">
  <span>tecnología</span>
  <span>renovada</span>
</div>

Explicación del Estilo del Título:

Utiliza display: block; en los elementos <span> para asegurar que cada uno se muestre en una línea separada.

Usa selectores pseudo-clases como :first-child y :last-child para aplicar estilos distintivos a cada parte del título.

Ajusta font-size para diferenciar visualmente las partes del título.

line-height es esencial para establecer la altura de la línea del texto, mejorando su legibilidad y estética.

4. Pruebas y Ajustes
Realiza una revisión de tu Hero Section en diferentes tamaños de pantalla para asegurarte de que los elementos se muestren correctamente y el diseño sea responsivo.

Tu código CSS para la Hero Section debería verse así:

/* Hero section */
section#hero {
  border: 1px solid purple;
  height: 340px;
  background: url("../assets/hero_bg.png");
  background-size: cover;
  background-position: top center;
}
section#hero .container {
  display: flex;
  align-items: center;
  justify-content: flex-start;
}
.title-container span {
  display: block;
  color: white;
  font-weight: 700;
}
.title-container span:first-child {
  font-size: 40px;
}
.title-container span:last-child {
  font-size: 100px;
  line-height: 80px;
}
Y tu html así

<section id="hero">
  <div class="container">
    <div class="title-container">
      <span>tecnología</span>
      <span>renovada</span>
    </div>
  </div>
</section>
Tu tienda, de momento debería lucir así

hero section flexbox.snapshot
✅ Checklist
Añadir ID hero a la sección Hero.

Implementar fondo y configurar sus propiedades.

Añadir y estilizar el título de la Hero Section.

Pruebas de visualización responsiva.