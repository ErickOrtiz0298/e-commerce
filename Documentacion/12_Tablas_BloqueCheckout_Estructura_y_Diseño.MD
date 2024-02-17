Actividades
1. Estructuración del Contenedor de Checkout
El objetivo de esta actividad es crear y estructurar un contenedor para el checkout en la página de detalle del producto. Este contenedor incluirá elementos como el total del precio, descripción de impuestos, políticas de envío y opciones de compra.

Instrucciones:
Crear el Contenedor Principal de Checkout:

En tu archivo HTML, identifica o crea la sección donde el bloque de checkout será ubicado.

Crea un <div> que actuará como el contenedor principal para el checkout y asigna una clase para identificación, por ejemplo, checkout-container.

Ejemplo:

<div class="checkout-container">
  <!-- Los elementos del checkout irán aquí -->
</div>
Agregar Elementos del Checkout:

Dentro del checkout-container, añade los siguientes elementos:

Etiqueta Total:

Agrega una etiqueta <span> o <div> para el total, por ejemplo, "Total:". Asigna una clase para estilizarla más tarde.

Precio Total:

Incluye un elemento <h2> para mostrar el precio total del producto. Asígnale una clase como checkout-total-price.

Descripción de Impuestos y Políticas:

Utiliza un párrafo <p> para describir detalles sobre impuestos y recuperaciones. Esta información es vital para que el usuario entienda cualquier costo adicional.

<span class="checkout-total-label">Total:</span>
<h2 class="checkout-total-price">$152.400</h2>
<p class="checkout-description">
  Incluye impuesto PAIS y percepción AFIP. Podés recuperar AR$ 50711
  haciendo la solicitud en AFIP.
</p>
Listar Políticas de Envío:

Añade una lista <ul> con varios <li> para describir las políticas de envío y otras condiciones relevantes.

Incluye íconos o imágenes para representar visualmente cada política, si es posible.

<ul class="checkout-policy-list">
  <li>
    <span class="policy-icon"
      ><img src="../assets/truck.png" alt="Truck"
    /></span>
    <span class="policy-desc"
      >Agrega el producto al carrito para conocer los costos de envío</span
    >
  </li>
  <li>
    <span class="policy-icon"
      ><img src="../assets/plane.png" alt="Plane"
    /></span>
    <span class="policy-desc"
      >Recibí aproximadamente entre 10 y 15 días hábiles, seleccionando
      envío normal</span
    >
  </li>
</ul>
Opciones de Compra:

Agrega un div para las opciones de compra que incluya elementos como un input para la cantidad y botones para "Comprar" y "Añadir al Carrito".

Cada botón y campo de entrada debe tener su propia clase para poder aplicar estilos específicos.

<ul class="checkout-policy-list">
  <li>
    <span class="policy-icon"
      ><img src="../assets/truck.png" alt="Truck"
    /></span>
    <span class="policy-desc"
      >Agrega el producto al carrito para conocer los costos de envío</span
    >
  </li>
  <li>
    <span class="policy-icon"
      ><img src="../assets/plane.png" alt="Plane"
    /></span>
    <span class="policy-desc"
      >Recibí aproximadamente entre 10 y 15 días hábiles, seleccionando
      envío normal</span
    >
  </li>
</ul>
Al completar estos pasos, tendrás un contenedor de checkout bien estructurado y listo para ser estilizado. Este contenedor será esencial para proporcionar a los usuarios una experiencia clara y sencilla al realizar una compra.

2. Diseño y Estilización del Contenedor y sus Elementos
En esta actividad, nos enfocaremos en aplicar los estilos CSS proporcionados para hacer que el bloque de checkout sea intuitivo, atractivo y coherente con el diseño general del sitio.

Estilizar el Contenedor de Checkout:

Aplica estilos al checkout-container para establecer un fondo, padding y bordes redondeados. Esto ayudará a que el bloque de checkout se destaque del resto de la página.

Ejemplo:

.checkout-container {
  background-color: #ebebeb; /* Color de fondo claro */
  padding: 33px; /* Espaciado interno */
  border-radius: 2px; /* Bordes ligeramente redondeados */
}
Estilizar Etiqueta y Precio Total:

Aplica estilos al checkout-total-label y checkout-total-price para resaltar visualmente el total del precio.

Asegúrate de que el color, tamaño de fuente y peso de la fuente del precio sean claros y destacados.

Ejemplo:

.checkout-total-label {
  color: #ff3b3c; /* Color distintivo para el texto 'Total:' */
}
.checkout-total-price {
  font-size: 28px; /* Tamaño grande para el precio */
  font-weight: 700; /* Fuente en negrita */
  margin-top: 10px; /* Espacio por encima del precio */
}
Estilizar Descripción del Checkout:

Estiliza el párrafo checkout-description para garantizar que la información adicional sea legible y esté bien estructurada.

Ejemplo:

.checkout-description {
  line-height: 20.4px; /* Espaciado de línea para mejorar la legibilidad */
  word-wrap: break-word; /* Asegura que el texto no desborde el contenedor */
}
Estilizar Lista de Políticas de Envío:

Aplica estilos a la checkout-policy-list y sus elementos <li> para mostrar claramente las políticas de envío y otras condiciones.

Usa display: flex; en los <li> para alinear los íconos con el texto.

Ejemplo:

.checkout-policy-list {
  list-style-type: none; /* Elimina los marcadores de lista */
  margin-bottom: 30px; /* Espacio debajo de la lista */
}
.checkout-policy-list li {
  display: flex; /* Alineación horizontal de íconos y texto */
  margin: 15px 0; /* Espacio entre elementos de la lista */
}
.checkout-policy-list li .policy-icon {
  margin-right: 15px; /* Espacio entre el ícono y el texto */
}
Estilizar Opciones de Compra:

Estiliza la sección checkout-process y sus elementos para mejorar la interacción con las opciones de compra.

Asegúrate de que los botones y el campo de cantidad sean fáciles de usar y visualmente atractivos.

Ejemplo:

.checkout-process .top {
  display: flex; /* Alinea el input y el botón horizontalmente */
  margin-bottom: 10px; /* Espacio debajo del grupo superior */
}
.checkout-process .top input {
  height: 40px;
  border-radius: 10px;
  border: none;
  width: 62px;
  margin-right: 10px;
  padding: 0 10px 0 20px;
  box-sizing: border-box;
}
.btn-primary {
  width: 100%;
  background: #ff3b3c;
  color: white;
  font-weight: bold;
  border: none;
  height: 40px;
  border-radius: 10px;
}
.btn-outline {
  width: 100%;
  border: 1px solid #ff3b3c;
  color: #ff3b3c;
  font-weight: bold;
  height: 40px;
  border-radius: 10px;
}
Pruebas Finales:

Revisa tu página en un navegador para asegurarte de que los estilos se apliquen correctamente y el bloque de checkout sea coherente y atractivo.

Haz ajustes según sea necesario para mejorar la presentación y asegurarte de que sea responsiva.

Al completar estos pasos, tendrás un bloque de checkout bien diseñado, lo que facilitará a los usuarios comprender el costo total y las políticas relacionadas, así como realizar acciones de compra.

✅ Actividades finalizadas
Estructuración del Contenedor de Checkout

Diseño y Estilización del Contenedor y sus Elementos