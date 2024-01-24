Actividades
1. Aplicando un color de fondo a nuestro footer
Identificar la etiqueta del footer: Primero, asegúrate de que el elemento footer está correctamente identificado en tu archivo HTML. Generalmente, se usa la etiqueta <footer>.

Color de fondo: Dentro de la etiqueta <footer>, agrega una propiedad css que defina el color de fondo al siguiente valor hexadecimal: #7525A7;

2. Estructura del footer
Agrega un <div> dentro del container con la clase "columns-container". Este div se usará para organizar las columnas del footer.

Crea múltiples <div> con la clase "col" dentro del "columns-container". Cada "col" representará una columna individual en el footer.

En cada columna (<div class="col">), añade un <ul> para listar los elementos e inserta elementos <li> dentro de cada <ul>. Cada <li> contendrá un enlace (<a href="#">) que representa diferentes secciones o servicios de la tienda online, como ofertas, información sobre compras, etc.

Además, al mismo nivel de columns-container, agrega un <div> con clase copyright, para alojar información legal sobre tu sitio y el año de creación o actualización de tu tienda.

3. Estilos del footer
Configuración del Contenedor InternoSelecciona en tu archivo de estilos el div container dentro del footer y aplica estilos para acomodar los elementos según el prototipo:display: flex: Esto permite organizar los elementos internos en un diseño flexible.flex-direction: column: Establece el div container como columna para apilar los elementos verticalmente. (Los items de las listas y nuestro espacio para copyright)

Columnas del footerPara el columns-container:flex: 1: Establece la propiedad flex para que ocupe el espacio vertical disponible.display: flex: Esto organizará las columnas con las listas de enlaces de manera horizontal.justify-content: Usa justify-content: space-between; para distribuir las columnas uniformemente.

Listas y enlacesAsegurate de seleccionar el elemento ul de la lista y ajustar el padding a 0 y eliminar el estilo de la lista para evitar que cada item tenga un bullet. Ajusta los espacios utilizando las propiedades margin y padding para simular los espacios entre elementos del prototipo.

Puedes ajustar el peso de la fuente y colorear los enlaces de color blanco y eliminar el subrayado.

La estructura actualizada de tu footer debería verse así:

<footer>
  <div class="container">
    <div class="columns-container">
      <div class="col">
        <ul>
          <li class="col-main-item"><a href="#">Ofertas de la semana</a></li>
          <li><a href="#">Laptops</a></li>
          <li><a href="#">Audio</a></li>
          <li><a href="#">Auticulares</a></li>
        </ul>
      </div>
      <div class="col">
        <ul>
          <li class="col-main-item"><a href="#">Cómo comprar</a></li>
          <li><a href="#">Formas de pago</a></li>
          <li><a href="#">Envios</a></li>
          <li><a href="#">Devoluciones</a></li>
        </ul>
      </div>
      <div class="col">
        <ul>
          <li class="col-main-item"><a href="#">Costos y tarifas</a></li>
          <li><a href="#">Impuestos</a></li>
          <li><a href="#">Facturación</a></li>
        </ul>
      </div>
      <div class="col">
        <ul>
          <li class="col-main-item"><a href="#">Mis pedidos</a></li>
          <li><a href="#">Pedir nuevamente</a></li>
          <li><a href="#">Lista de deseos</a></li>
        </ul>
      </div>
      <div class="col">
        <ul>
          <li class="col-main-item"><a href="#">Garantía de Entrega</a></li>
        </ul>
      </div>
    </div>
    <div class="copyright">Curso de HTML + CSS 2023</div>
  </div>
</footer>
Los estilos de tu footer deberían verse de la siguiente manera:

footer {
  border: 1px solid #009145;
  /* Hexadecimal color code*/
  min-height: 368px;
  background-color: #7525a7;
}
footer .container {
  display: flex;
  flex-direction: column;
}
.columns-container {
  flex: 1;
  display: flex;
  justify-content: space-between;
}
.columns-container .col ul {
  list-style-type: none;
  padding: 0;
}
.columns-container .col ul li {
  padding: 5px 0;
}
.columns-container .col ul li.col-main-item {
  font-weight: bold;
  padding-bottom: 20px;
}
.columns-container .col ul li a {
  color: white;
  text-decoration: none;
}
.copyright {
  border-top: 1px solid #ba53fb;
  text-align: center;
  color: white;
  font-weight: bold;
  padding: 30px 0;
  box-sizing: border-box;
}
✅ Actividades finalizadas
Aplicando un color de fondo a nuestro footer

Estructura del footer

Estilos del footer