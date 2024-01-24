Actividades
1. Estilizando la Navegación y la Búsqueda
Ahora nos enfocaremos en aplicar los estilos CSS que definirán la estética y la estructura de los bloques de búsqueda y navegación en nuestro Header.

Estilos para el Bloque de Búsqueda (search): Abre tu archivo styles.css y aplica estilos Flexbox para organizar el logo, el formulario de búsqueda y los iconos sociales dentro del div de la clase search.

.search {
  flex: 1;
  display: flex;
  justify-content: space-between;
  align-items: center;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
Estilizando el Formulario de Búsqueda: Personaliza el formulario y el campo de búsqueda para que sean intuitivos y estilísticamente coherentes con el diseño general del sitio.

.search .form {
  box-sizing: border-box;
  display: flex;
  justify-content: center;
}
.search .form input {
  height: 62px;
  border-radius: 14px;
  border: none;
  width: 505px;
  padding: 20px;
  box-sizing: border-box;
}
Estilos para los Iconos Sociales: Establece una disposición atractiva y accesible para los íconos sociales.

.search .social ul {
  display: flex;
  justify-content: flex-end;
  list-style-type: none;
  margin: 0;
  padding: 0;
}
.search .social ul li {
  padding: 0 10px;
}
Estilos para la Navegación (nav): Utiliza Flexbox para asegurar que los elementos de la lista de navegación estén bien alineados y distribuidos.

.nav {
  padding: 10px 0;
}
.nav ul {
  display: flex;
  justify-content: space-between;
  list-style-type: none;
  margin: 0;
  padding: 0;
}
.nav ul li a {
  color: white;
  font-weight: 700;
  text-align: left;
  text-decoration: none;
}
.nav ul li a:hover {
  text-decoration: underline;
}
2. Pruebas y Ajustes
Asegúrate de que el Header se visualiza correctamente en diversos tamaños de pantalla, y realiza los ajustes necesarios para garantizar una experiencia de usuario óptima en todos los dispositivos.

✅ Actividades finalizadas
Estilizando la Navegación y la Búsqueda

Pruebas y Ajustes