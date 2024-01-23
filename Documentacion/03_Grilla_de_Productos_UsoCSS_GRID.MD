Actividades
1. Separación de Estilos en un Archivo Externo
Antes de sumergirnos en la configuración del grid, es esencial comprender la importancia de mantener nuestro código CSS en un archivo separado. Esta práctica no solo facilita la lectura y el mantenimiento del código, sino que también permite reutilizar estilos en múltiples páginas de nuestra tienda virtual.

Creación del Archivo styles.css: Crea un nuevo archivo llamado styles.css en la misma carpeta que tu archivo index.html.

Corta y pega todos los estilos CSS de la etiqueta <style> en tu index.html a este nuevo archivo.

Vinculando styles.css con index.html: En tu archivo index.html, dentro de la etiqueta <head>, agrega una referencia al archivo styles.css usando la etiqueta <link>. Por ejemplo:<link rel="stylesheet" href="styles.css" />

Verificación: Abre tu archivo index.html en un navegador para asegurarte de que los estilos se aplican correctamente desde el archivo externo.

2. Configuración del Grid de Productos
Ahora, enfocándonos en el uso de CSS Grid, ajustaremos el product-container para presentar nuestras cards de productos de manera eficiente y atractiva.

Definición del Grid:

En styles.css, aplica display: grid; a .product-container.

Utiliza grid-template-columns: repeat(4, 1fr);para crear un layout de cuatro columnas.

Espaciado Entre Cards: Aplica grid-gap: 20px; para un espaciado uniforme.

Ajustes Responsivos: Agrega media queries para cambiar la disposición del grid en dispositivos más pequeños, como se muestra en la sección anterior.

3. Estilización de las Cards de Producto
En el archivo styles.css, realiza los ajustes necesarios para que cada card de producto se adapte y se presente adecuadamente dentro del grid. Configura la propiedad width:auto para que nuestra card ocupe todo el ancho disponible de la columna.

4. Replica tu card de producto
Felicitaciones. Tu tienda virtual ya soporte múltiples productos dentro de la grilla. Prueba duplicando tu card de producto en index.html varias veces para visualizar el nuevo comportamiento.

5. Pruebas y Ajustes
Revisa tu página en diferentes tamaños de pantalla para asegurarte de que el layout del grid y el diseño de las cards sean responsivos y estéticamente agradables.

En esta instancia, las adiciones a tu código deberían verse de la siguiente manera:

/* Bloque de productos */
.product-container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 20px;
}
/* Card de producto */
.product-card {
  background-color: #f0f0f0;
  border-radius: 14px;
  width: auto;
}
Tu grilla de productos debería verse similar a esta imagen:

product grid css
✅ Actividades finalizadas
Separación de Estilos en un Archivo Externo

Configuración del Grid de Productos

Estilización de las Cards de Producto

Replica tu card de producto

Pruebas y Ajustes