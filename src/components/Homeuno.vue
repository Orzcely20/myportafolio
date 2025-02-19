<template>
  <div class="home-page">
    <!-- Sección Home -->
    <section id="home" class="home">
      <h1>Bienvenido a mi Portfolio</h1>
      <p>Desarrollador Web & Diseñador UI/UX</p>
    </section>

    <!-- Sección About -->
    <section id="about" class="about">
      <h2>Sobre mí</h2>
      <p>Información sobre el desarrollador.</p>
    </section>

    <!-- Sección Gallery -->
    <section id="gallery" class="gallery">
      <h2>Galería de Proyectos</h2>
      <p>Aquí van imágenes y descripciones de proyectos.</p>
    </section>

    <!-- Sección Contact -->
    <section id="contact" class="contact">
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
        <button type="submit" class="btn btn-primary">Enviar</button>
      </form>
    </section>
  </div>
</template>

<script>
export default {
  name: "HomePage",
};
</script>

<style scoped>
/* Estilos para las secciones */
.home {
  text-align: center;
  margin-bottom: 50px;
  padding: 20px;
}

.about, .gallery, .contact {
  margin: 50px 0;
  padding: 20px;
  background-color: #f4f4f4;
}

.about {
  background-color: #e0d4f1; /* Lila suave */
}

.gallery {
  background-color: #d0c7f1; /* Lila más oscuro */
}

.contact {
  background-color: #c1b0f1; /* Lila claro */
}

h1, h2 {
  color: #3a3a3a;
}

button {
  margin-top: 10px;
}
</style>
