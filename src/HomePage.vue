<template>
  <div>
    <!-- Barra superior fija -->
    <div class="navbar-container">
      <div class="navbar">
        <div class="brand">Portfolio</div>
        <div class="nav-buttons">
          <!-- botones para el desplazamiento suave -->
          <a href="#home">Home</a>
          <a href="#about">About</a>
          <a href="#gallery">Gallery</a>
          <a href="#contact">Contact</a>
        </div>
      </div>
    </div>

    <!-- Secciones -->
    <div id="home" class="main-content">
      <h1>Bienvenido a mi Portfolio</h1>
      <p>Estudiante de la carrera TICs, área en entornos virtuales y negocios digitales.</p>
    </div>

    <div id="about" class="about-section">
      <div class="about-container">
        <div class="image">
          <img src="@/assets/ceci.jpg" alt="Mi Foto" />
        </div>
        <div class="text">
          <h2>Sobre mí</h2>
          <p class="justified">Soy una estudiante de la carrera de Tecnologías de la Información y la Comunicación, especializada en Entornos Virtuales y Negocios Digitales, me gusta aprender y dejar buen papel sobre mi, siempre busco la manera de trabajar bien y tener exito en lo que me propongo, actualmente me encuentro trabajando y estudiando.</p>
        </div>
      </div>
    </div>

    <div id="gallery" class="gallery-section">
      <h2>Galería de Proyectos</h2>
      <p>Mis proyectos realizados.</p>
      
      <!-- Mis Imágenes de la galería -->
      <div class="gallery-images">
        <div class="gallery-item">
          <img src="@/assets/Modelado en blender.jpg" alt="Proyecto 1" />
          <p>Proyecto 1 - Mi trabajo en Diseño en 3D.</p>
        </div>
        <div class="gallery-item">
          <img src="@/assets/Desarrollo de una app.jpg" alt="Proyecto 2" />
          <p>Proyecto 2 - Desarrollando una aplicacion web y app movil sobre musica.</p>
        </div>
        <div class="gallery-item">
          <img src="@/assets/MI perfil uni.jpg" alt="Proyecto 3" />
          <p>Proyecto 3 - Hice mi perfil universitario.</p>
        </div>
        <!-- aqui agrego mas imagenes -->
      </div>
    </div>

    <div id="contact" class="contact-section">
      <h2>Contacto</h2>
      <form>
        <div class="mb-3">
          <label class="form-label">Nombre</label>
          <input type="text" class="form-control" />
        </div>
        <div class="mb-3">
          <label class="form-label">Email</label>
          <input type="email" class="form-control" />
        </div>
        <div class="mb-3">
          <label class="form-label">Mensaje</label>
          <textarea class="form-control"></textarea>
        </div>
        <button type="submit" class="btn btn-primary">Enviar Mensaje</button>
      </form>
    </div>

    <!-- Footer -->
    <footer class="footer">
      <div class="footer-container">
        <div class="footer-column">
          <h3>About us</h3>
          <p>Somos un equipo apasionado de estudiantes en el campo de las Tecnologías de la Información y la Comunicación (TICs), especializados en entornos virtuales y negocios digitales. Nos dedicamos a crear soluciones innovadoras que transforman la manera en que las personas interactúan con la tecnología.</p>
        </div>
        <div class="footer-column">
          <h3>Quick Links</h3>
          <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About me</a></li>
            <li><a href="#gallery">Gallery</a></li>
            <li><a href="#contact">Contact</a></li>
          </ul>
        </div>
        <div class="footer-column">
          <h3>Contact</h3>
          <p>Email: orzcocecilia@gmail.com</p>
          <p>Phone: 984 313 45 55</p>
          <p>Address: Cancun,quintana Roo, playa del carmen</p>
        </div>
      </div>
      <div class="footer-bottom">
        <p>© 2025. By Cecilia orozco. All rights reserved.</p>
      </div>
    </footer>
  </div>
</template>


esta es la parte de mi CSS
<script>
export default {
  name: "HomePage",
};
</script>

<style scoped>
/* Barra de navegación fija */
.navbar-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #6a4c9c;  /* Color morado */
  z-index: 1000;
  padding: 10px 0;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 20px;
}

.brand {
  font-size: 1.8em;
  color: white;
  font-weight: bold;
}

.nav-buttons {
  display: flex;
  gap: 15px;
}

.nav-buttons a {
  color: white;
  text-decoration: none;
  padding: 8px 16px;
  border: 2px solid white;
  cursor: pointer;
}

.nav-buttons a:hover {
  background-color: white;
  color: #6a4c9c;
}

/* Secciones */
.main-content, .about-section, .gallery-section, .contact-section {
  padding-top: 60px; /* Para no tapar el contenido por la barra fija */
  margin-top: 30px;
  text-align: center;
  padding-bottom: 60px; /* Para un poco de espacio en la parte inferior */
}

h1, h2 {
  color: #6a4c9c;
  font-size: 2em;
}

p {
  font-size: 1.2em;
}

form .mb-3 {
  margin-bottom: 20px;
}

form button {
  background-color: #6a4c9c;
  color: white;
  border: none;
  padding: 10px 20px;
  cursor: pointer;
}

form button:hover {
  background-color: white;
  color: #6a4c9c;
}

/* Estilos para la sección "Sobre mí" */
.about-container {
  display: flex;
  justify-content: center; /* Centra los elementos horizontalmente */
  align-items: center; /* Centra los elementos verticalmente */
  flex-direction: column; /* Acomoda la imagen y el texto en una columna */
  text-align: center; /* Centra el texto */
  margin-top: 20px; /* Ajusta el margen superior si es necesario */
  padding: 0 20px; /* Da un poco de espacio a los lados para que no se pegue al borde */
}
.about-container .text p {
  text-align: justify; /* Justifica el texto */
  text-justify: inter-word; /* Esto es opcional, ya que controla la distribución de los espacios entre palabras */
}

.about-container .about-content {
  max-width: 1200px; /* ajusta el valor de anche deseadoo */
  width: 100%;
  padding: 20px;
  box-sizing: border-box; /* Para que el padding no afecte el ancho */
  display: flex;
  justify-content: center; /* Centra los elementos dentro de esta sección */
  flex-direction: column; /* Coloca la imagen y el texto en una columna */
}

.about-container .image {
  margin-bottom: 20px; /* Espacio entre la imagen y el texto */
}

.about-container img {
  max-width: 100%;
  height: auto;
  border-radius: 20%; /* para poner forma circular */
  max-height: 2000px; /* Tamaño máximo de la imagen */
}

/* Para pantallas grandes, vuelve a disposición en fila */
@media (min-width: 768px) {
  .about-container {
    flex-direction: row; /* Los elementos estarán uno al lado del otro en pantallas grandes */
    padding: 0 100px; /* Aumenta el espacio de los lados en pantallas grandes */
  }

  .about-container .about-content {
    flex-direction: row; /* Para que la imagen y el texto estén lado a lado */
  }

  .about-container .image {
    margin-right: 20px; /* Espacio entre la imagen y el texto */
  }
}


/* Estilos para la galería */
.gallery-images {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  gap: 20px;
}

.gallery-item {
  width: 30%;
  text-align: center;
}

.gallery-item img {
  width: 100%;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.gallery-item p {
  font-size: 1.1em;
  color: #6a4c9c;
  margin-top: 10px;
}

/* Footer */
.footer {
  background-color: #f8f9fa;
  padding: 20px 0;
  text-align: left;
}

.footer-container {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  gap: 20px;
}

.footer-column {
  width: 30%;
}

.footer-column h3 {
  font-size: 1.2em;
  color: #6a4c9c;
}

.footer-column p, .footer-column ul, .footer-column li, .footer-column a {
  font-size: 1em;
  color: #6a4c9c;
  text-decoration: none;
}

.footer-bottom {
  background-color: #6a4c9c;
  color: white;
  text-align: center;
  padding: 10px 0;
}

.footer-bottom p {
  margin: 0;
}

/* Agregar un espacio entre secciones */
section {
  margin-bottom: 40px;
}

/* Scroll suave */
html {
  scroll-behavior: smooth;
}
</style>
