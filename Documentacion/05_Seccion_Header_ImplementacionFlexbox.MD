Actividades
1. Aplicando Color de Fondo al Header
Daremos vida al <header> con un color de fondo distintivo que se alinee con la identidad visual de la tienda.

En el archivo styles.css, aplica un color de fondo a la etiqueta header:

header {
  background-color: #ff3b3c; /* Ejemplo de color */
}
2. Creación de Bloques para Búsqueda y Navegación
La estructura del Header se divide en dos partes principales, el Bloque de Búsqueda y el Bloque de Navegación.

1. Estructura del Bloque de Búsqueda: Abre tu archivo index.html. Dentro del header, crea un div con la clase search. Este bloque contendrá el logo, la barra de búsqueda y los iconos de redes sociales.

<div class="search">
  <!-- Aquí irán el logo, el formulario de búsqueda y los iconos sociales -->
</div>
2. Añadiendo Elementos al Bloque de Búsqueda: Dentro del div de la clase search, añade tres contenedores:

Un div que contendrá el logo con la clase logo.

Otro div para el formulario de búsqueda con la clase form.

Un tercer div para los iconos de las redes sociales con la clase social.

<div class="search">
  <div class="logo">
    <img src="../assets/tiendamia-logo.svg" width="218" alt="Logo store" />
  </div>
  <div class="form">
    <form>
      <input type="text" placeholder="Search" />
    </form>
  </div>
  <div class="social">
    <!-- Aquí irán los íconos de redes sociales -->
  </div>
</div>
3. Estructura del Bloque de Navegación:

A continuación, crea otro div con la clase nav para la barra de navegación. Dentro de este div, añade una lista desordenada (ul) para los enlaces de navegación (li).

<div class="nav">
  <ul>
    <li><a href="#">Ofertas de la semana</a></li>
    <!-- Más elementos de lista aquí -->
  </ul>
</div>
✅ Actividades finalizadas
Aplicando Color de Fondo al Header

Creación de Bloques para Búsqueda y Navegación