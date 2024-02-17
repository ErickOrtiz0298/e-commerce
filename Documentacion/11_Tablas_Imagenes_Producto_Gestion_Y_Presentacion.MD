Actividades
1. Creación del Contenedor de Imágenes
El objetivo de esta actividad es crear un contenedor para las imágenes del producto, asegurando que se muestren de manera organizada y atractiva. Este contenedor ayudará a los usuarios a visualizar claramente el producto que están considerando comprar.

Preparar el Espacio para el Contenedor de Imágenes:

En tu archivo HTML, identifica o crea el área donde deseas mostrar las imágenes del producto. Este será el lugar donde integrarás el contenedor de imágenes.

Asegúrate de que este espacio esté ubicado de manera estratégica en la página para captar la atención del usuario.

Crear el Contenedor Principal de Imágenes:

Dentro del espacio seleccionado, crea un <div> que actuará como el contenedor principal para las imágenes del producto.

Asigna una clase al contenedor, por ejemplo, product-images-block.

Ejemplo de inicio del contenedor:

<div class="product-images-block">
  <!-- Las miniaturas de imágenes irán aquí -->
</div>
Agregar Miniaturas de Imágenes:

Dentro del product-images-block, crea varios <div> que funcionarán como contenedores para las miniaturas de las imágenes.

Cada uno de estos <div> debe tener su propia clase, como thumbnail-container.

Dentro de cada thumbnail-container, agrega una etiqueta <img> con la ruta al archivo de imagen correspondiente.

Ejemplo:

<div class="product-images-block">
  <div class="thumbnail-container">
    <img src="../assets/mock1.jpg" alt="Descripción de la imagen 1" />
  </div>
  <div class="thumbnail-container">
    <img src="../assets/mock2.jpg" alt="Descripción de la imagen 2" />
  </div>
  <!-- Agregar más miniaturas según sea necesario -->
</div>
Verificación y Ajustes:

Revisa tu estructura HTML para asegurarte de que todos los elementos estén correctamente anidados y que las imágenes se carguen correctamente.

Ajusta las rutas de las imágenes si es necesario y asegúrate de que cada imagen tenga un atributo alt descriptivo para la accesibilidad.

2. Estilización y Ajuste de las Imágenes
En esta actividad, nos centraremos en aplicar estilos CSS para que las imágenes del producto se muestren correctamente dentro de su contenedor, manteniendo un aspecto uniforme y profesional.

Estilizar el Contenedor Principal de Imágenes:

En tu archivo CSS, busca o crea la clase correspondiente al contenedor principal de las imágenes, por ejemplo, .product-images-block.

Aplica estilos para manejar el ancho, el desbordamiento y cualquier otra propiedad que consideres necesaria para mejorar la presentación del contenedor.

Ejemplo:

.product-images-block {
  max-width: 100%;
  overflow: hidden; /* Asegúrate de que las imágenes no desborden el contenedor */
}
Estilizar los Contenedores de las Miniaturas:

Estiliza cada thumbnail-container para controlar la forma en que se presentan las miniaturas de las imágenes.

Puedes aplicar márgenes, bordes, o cualquier otro estilo que mejore la visualización individual de cada imagen.

Ejemplo:

.product-images-block .thumbnail-container {
  max-width: 100%;
  overflow: hidden; /* Mantiene la imagen dentro del contenedor */
  margin: 5px; /* Ajusta el margen según sea necesario */
  border: 1px solid #ccc; /* Opcional, si deseas bordes */
}
Estilizar las Imágenes Dentro del Contenedor:

Estiliza las etiquetas <img> dentro de cada thumbnail-container para asegurar que se ajusten adecuadamente.

Usa propiedades como object-fit y object-position para controlar cómo se muestran las imágenes dentro de sus contenedores.

Ejemplo:

.product-images-block .thumbnail-container img {
  max-width: 100%;
  height: auto; /* Mantiene la relación de aspecto de la imagen */
  object-fit: contain; /* Asegura que la imagen se ajuste completamente dentro del contenedor */
  object-position: center center; /* Centra la imagen en el contenedor */
}
✅ Actividades finalizadas
Creación del Contenedor de Imágenes

Estilización y Ajuste de las Imágenes