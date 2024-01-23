Actividades
1. Creación de la Estructura de la Card de Producto
Para cada producto que deseamos mostrar, encapsularemos la información en una estructura HTML que definirá claramente los elementos de la card. Seguiremos una metodología clara para asegurarnos de que cada parte de la card esté correctamente posicionada y sea fácil de estilizar.

Contenedor Principal de los Productos (product-container): Comenzaremos definiendo un div con la clase product-container dentro del div con clase .container, en reemplazo del texto de ejemplo, que actuará como el envoltorio de nuestras card de producto. Este contenedor nos ayudará posteriormente a organizar múltiples cards en un diseño de cuadrícula o en filas y columnas para una presentación atractiva.

Card del Producto (product-card): Dentro de nuestro contenedor principal, añadiremos una etiqua <article> con la clase product-card. Esta será la entidad principal que albergará todos los detalles específicos del producto.

Imagen del producto (product-img): Colocaremos una etiqueta <img> con los atributos src y alt y la clase product-img, asegurándonos de que cada imagen sea accesible y tenga una descripción alternativa para los lectores de pantalla.

Bloque de información: Colocaremos una etiqueta div con la clase product-info donde agruparemos toda la información textual de nuestro producto. Esto nos permitirá dar un margen a todos los textos por igual.

Título y Descripción del Producto: Seguirá el título del producto, envuelto en un <span> con la clase product-title, seguido de una descripción corta del producto en otro <span> con la clase product-description.

Bloque de Precio (product-price-block): Para la información de precios, crearemos un div con la clase product-price-block, donde incluiremos otro <span> para el precio y, si es necesario, un <span> adicional para mostrar un descuento aplicado.

Información de Impuestos: Finalmente, incluiremos un div con la clase product-tax-policy para informar al cliente sobre los impuestos o cargos adicionales incluidos en el precio.

Nuestro código para la card de producto debería verse así:

<main>
  <div class="container">
    <div class="product-container">
      <article class="product-card">
        <img class="product-img" src="ruta_a_la_imagen.jpg" alt="Macbook Pro" />
        <div class="product-info">
          <span class="product-title">Macbook Pro 15'4</span>
          <span class="product-description">Space Gray</span>
          <div class="product-price-block">
            <span class="price">$750.000</span>
            <span class="discount">50% Off</span>
          </div>
          <div class="product-tax-policy">Incluye impuesto País y percepción AFIP</div>
        </div>
      </article>
    </div>
  </div>
</main>
Con esta estructura en su lugar, habremos creado una base sólida para cada card de producto. En las siguientes actividades, nos centraremos en dar estilo a estos elementos con CSS para que sean visualmente coherentes con el diseño global de la tienda virtual y garantizar una navegación intuitiva y atractiva para los usuarios.

2. Insertando imágenes en nuestra card
Selección de Imágenes: Antes de insertar imágenes en nuestras tarjetas de producto, es importante seleccionar imágenes de alta calidad que representen de manera fiel y atractiva los productos. Asegúrate de que las imágenes estén en un formato compatible con la web (como JPG o PNG) y que su tamaño sea adecuado para una carga rápida sin sacrificar la calidad.

Inserción de Imágenes: En la estructura de la tarjeta de producto product-card, inserta la imagen del producto usando la etiqueta <img>. Asegúrate de reemplazar "ruta-a-la-imagen.jpg" con la ruta correcta, que será algo como ./assets/nombre-de-la-imagen.jpg. Por ejemplo: <img class="product-img" src="imagenes/macbook-pro.jpg" alt="Macbook Pro">

Estilización de Imágenes: Los estilos definidos para .product-img son fundamentales para asegurar que las imágenes se ajusten adecuadamente en las tarjetas. Agreguemos la clase y los estilos a nuestra etiqueta style:

width: 100%; : Asegura que la imagen cubra todo el ancho de la tarjeta.

height: 250px; : Define una altura fija para mantener la consistencia visual.

object-fit: cover; y object-position: center center; : Estos estilos garantizan que la imagen se recorte de manera uniforme, manteniendo el enfoque en el centro del producto, lo que es especialmente útil para imágenes que no son del mismo tamaño o proporción.

3. Aplicando estilos a nuestra información
Inclusión de Fuentes Externas: Antes de aplicar estilos específicos, hemos incluido una fuente externa utilizando la etiqueta <link>. Esto nos permite usar tipografías que no están disponibles por defecto en los navegadores. En este caso, estamos utilizando la fuente 'Inter', una tipografía versátil y moderna. Inserta las etiquetas <link> correspondientes en la sección <head> de tu documento HTML. Estas etiquetas se conectan con Google Fonts y descargan la tipografía seleccionada. Por ejemplo:

<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
  href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap"
  rel="stylesheet"
/>
Dentro de tus estilos, define la tipografía Inter para todo el sitio de la siguiente forma:

body,
html {
  font-family: "Inter", sans-serif;
}
2. Implementando Flexbox para Layouts Flexibles: En nuestro diseño, utilizamos Flexbox para estructurar la disposición de los elementos dentro de la tarjeta de producto, especialmente en el bloque de precios.

Flexbox es un método de diseño que permite colocar elementos en un contenedor de manera flexible y responsiva. En tu CSS, para el bloque de precio, usa display: flex; para definir un contenedor flexible.

Luego, con justify-content: space-between; y align-items: center;, alineas los elementos dentro del contenedor de forma horizontal y vertical respectivamente. Por ejemplo:

.product-price-block {
  display: flex;
  margin: 5px 0;
  justify-content: space-between;
  align-items: center;
}
3. Aplicando Estilos a la Información del Producto:

A continuación, aplicaremos estilos a cada elemento de la tarjeta de producto para mejorar su visualización. Puedes basarte en el prototipo realizado en figma para obtener los tamaños y los detalles particulares de cada elemento.

Card de producto .product-card

Agrega un fondo de color #F0F0F0, redondea los bordes para que tengan un radio de 14px, define el ancho máximo de la card a 25% (max-width) y agrega un overflow: hidden para que la imagen no sobrepase los bordes redondeados.

Bloque de información .product-info

Establece un padding de 20px y la propiedad box-sizing: border-box;

Titulo del Producto .product-title:

Aplica un tamaño de fuente más grande y un peso de fuente en negrita para destacar el título.

Usa word-wrap: break-word; para evitar que el texto se desborde de su contenedor.

Utiliza la propiedad display:block para que el elemento siguiente se acomode a continuación de forma vertical.

Agrega un line-height: 22px para que en el caso de que el titulo tenga 2 lineas, la tipografía se separe correctamente entre lineas.

Descripción del Producto .product-description:

Utiliza un tamaño de fuente más pequeño y un peso de fuente regular para diferenciarlo del título.

Ajusta el color para una mejor legibilidad y un diseño más sutil.

Agrega un margen de 6px en el borde inferior.

Precio y Descuento .product-price-block:

Identifica en los estilos la clase .product-price-block

Establece tamaños de fuente distintos para el precio y el descuento, destacando el precio con un tamaño más grande.

Utiliza los conceptos aprendidos sobre especificidad para agregar los siguientes estilos:

.product-price-block .price {
  font-size: 22px;
  font-weight: 700;
  flex: 1;
}
.product-price-block .discount {
  font-size: 12px;
  font-weight: 700;
  color: #428f13;
}
Utiliza Flexbox para una disposición adecuada de estos elementos.

Política de Impuestos .product-tax-policy:

Usa un tamaño de fuente pequeño y un peso de fuente ligero para que esta información sea accesible pero no dominante.

De momento tu tarjeta tendrá el ancho total del contenedor, pero a continuación, en el paso siguiente, definiremos un ancho fijo para cada tarjeta en relación con el espacio disponible.

4. Pruebas y Ajustes
Una vez aplicados los estilos, abre tu archivo HTML en un navegador y revisa cómo se ven las tarjetas de producto. Asegúrate de que todos los elementos estén bien alineados y que los estilos se apliquen como se esperaba. Realiza ajustes si es necesario.

Al final de estas actividades nuestro código debería verse de la siguiente forma:

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap"
      rel="stylesheet"
    />
    <title>Tienda Virtual</title>
    <style>
      body,
      html {
        font-family: "Inter", sans-serif;
      }
      /* Estructura del sitio */
      header {
        border: 1px solid red;
        height: 152px;
      }
      section {
        border: 1px solid purple;
        height: 340px;
      }
      main {
        border: 1px solid blue;
        height: auto;
      }
      footer {
        border: 1px solid #009145; /* Hexadecimal color code*/
        min-height: 368px;
      }
      .container {
        width: 1220px;
        margin: 0 auto;
        border: 1px solid springgreen;
        height: inherit;
        min-height: inherit;
      }
      /* Card de producto */
      .product-card {
        background-color: #f0f0f0;
        border-radius: 14px;
        max-width: 25%;
        overflow:hidden;
      }
      .product-img {
        width: 100%;
        height: 250px;
        object-fit: cover;
        object-position: center center;
      }
      .product-info {
        padding: 20px;
        box-sizing: border-box;
      }
      .product-title {
        font-size: 20px;
        font-weight: 700;
        line-height: 22.27px;
        word-wrap: break-word;
        display: block;
      }
      .product-description {
        font-size: 12px;
        font-weight: 400;
        color: #383838;
        margin-bottom: 6px;
      }
      .product-price-block {
        display: flex;
        margin: 5px 0;
        justify-content: space-between;
        align-items: center;
      }
      .product-price-block .price {
        font-size: 22px;
        font-weight: 700;
        flex: 1;
      }
      .product-price-block .discount {
        font-size: 12px;
        font-weight: 700;
        color: #428f13;
      }
      .product-tax-policy {
        font-size: 11px;
        font-weight: 300;
      }
    </style>
  </head>
  <body>
    <header>
      <div class="container"></div>
    </header>
    <section>
      <div class="container"></div>
    </section>
    <main>
      <div class="container">
        <div class="product-container">
          <article class="product-card">
            <img
              class="product-img"
              src="../assets/mock1.jpg"
              alt="Macbook Pro"
            />
            <div class="product-info">
              <span class="product-title">Macbook Pro 15'4</span>
              <span class="product-description">Space Gray</span>
              <div class="product-price-block">
                <span class="price">$750.000</span>
                <span class="discount">50% Off</span>
              </div>
              <div class="product-tax-policy">
                Incluye impuesto País y percepción AFIP
              </div>
            </div>
          </article>
        </div>
      </div>
    </main>
    <footer>
      <div class="container"></div>
    </footer>
  </body>
</html>
✅ Actividades finalizadas
Creación de la Estructura de la Card de Producto

Insertando imagenes en nuestra card

Aplicando estilos a nuestra información

Pruebas y Ajustes