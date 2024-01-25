1. Preparando nuestro sitio para la nueva página de producto
En este paso, vamos a crear una página de detalles de producto. Comenzaremos duplicando nuestro archivo index.html y lo renombraremos como product.html. Después, realizaremos ajustes en el contenido para enfocarnos específicamente en los detalles del producto.

Duplicando nuestro archivo:

Localiza el archivo index.html: Este archivo es tu página principal actual y servirá como base para tu nueva página de producto.

Duplica el archivo: Haz una copia de index.html y renómbralo como product.html. Puedes hacer esto usando el explorador de archivos de tu sistema operativo o mediante una línea de comando. Si usas un sistema basado en Windows, simplemente copia y pega el archivo. En un sistema basado en Unix, como Linux o macOS, puedes usar el comando cp index.html product.html en tu terminal.

Verifica la duplicación: Asegúrate de que el nuevo archivo product.html esté en la misma ubicación que tu index.html y no te olvides de ejecutarlo en tu navegador para poder ir viendo los cambios.

Limpiando el contenido de product.html:

Abre product.html en tu editor de texto: Ahora que tienes tu archivo duplicado, es hora de hacer ajustes específicos para la página de producto.

Elimina la sección hero: La sección hero generalmente es específica de la página de inicio. Encuentra esta sección en tu product.html y elimínala. Esto puede ser tan simple como borrar el bloque de HTML correspondiente.

Limpia el contenido principal (main): Tu objetivo es centrarte en los detalles del producto, así que elimina el contenido innecesario que pertenece a la página principal. Mantén la etiqueta <main> y los contenedores principales a main pero quita todo el contenido interno que no esté relacionado con los detalles del producto.

Guarda tus cambios: Después de realizar estos ajustes, guarda el archivo product.html.

2. Creando la nueva estructura dentro de nuestro <main>
En este paso crearemos la estructura necesaria dentro de main para alojar nuestros bloques de detalle de producto. Un bloque para imagenes, un bloque para descripción y el bloque final para detalles como precio y los botones o call to action para agregar nuestro producto al carrito.

Revisión de estilos existentes:

Revisa los estilos ya aplicados a las clases container y columns-container. Estos estilos serán la base para tu nueva estructura, ayudando a mantener la coherencia y evitar duplicación de código.

Modificación de estilos:

En tu archivo styles.css, encuentra la clase .columns-container.

Agrega gap: 20px; a .columns-container. Esto asegurará que las nuevas columnas dentro de la página de producto tengan un espacio de 20 píxeles entre ellas.

Estructura básica:

Dentro de <main>, utiliza la clase container para envolver tu contenido principal.

Dentro de container, usa .columns-container para crear un contenedor flexible para tus columnas. Recuerda que las clases .container y .columns-container ya están definidas en nuestro archivo de estilos y en el caso de .columns-container, organizan los divs "hijos" de .container de forma horizontal. Justo lo que necesitamos para nuestro layout de 3 columnas.

División en columna:

Crea 3 <div> dentro de columns-container. Cada una representará un aspecto diferente del producto: imágenes, descripción y detalles adicionales como precio y botones de acción.

Asigna una clase o identificador a cada <div> para poder estilizarlos y referenciarlos específicamente más adelante.

Bloque de ventas:

Agrega un <div> con la clase sales-block después del columns-container. Este bloque puede usarse para mostrar productos en oferta u otras promociones relacionadas.

Contenido de ejemplo:

Por ahora, puedes usar texto de relleno como "Lorem ipsum" para simular el contenido. Esto te ayudará a visualizar la estructura y realizar ajustes antes de agregar el contenido real.

Nuestro <main> debería verse así:

<main>
  <div class="container">
    <div class="columns-container">
      <div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam,
        unde! Obcaecati non cum illum, rem voluptatem commodi exercitationem
        accusantium, quod voluptatum aspernatur amet ab! Quo soluta aut
        reiciendis labore corporis?
      </div>
      <div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam,
        unde! Obcaecati non cum illum, rem voluptatem commodi exercitationem
        accusantium, quod voluptatum aspernatur amet ab! Quo soluta aut
        reiciendis labore corporis?
      </div>
      <div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam,
        unde! Obcaecati non cum illum, rem voluptatem commodi exercitationem
        accusantium, quod voluptatum aspernatur amet ab! Quo soluta aut
        reiciendis labore corporis?
      </div>
    </div>
    <div class="sales-block">
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Accusamus porro,
      eum minus nobis doloribus pariatur tempora officia a, facilis repellendus,
      aspernatur veniam. Similique nulla tenetur necessitatibus provident ipsam,
      incidunt ipsa.
    </div>
  </div>
</main>
✅ Actividades finalizadas
Preparando nuestro sitio para la nueva página de producto

Creando la nueva estructura dentro de nuestro <main>