# curriculumvitae
<!DOCTYPE html>
<html lang="es">
<head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Mi CV</title>
   <style>
      /* Estilos generales ... (tus estilos aquí) */
   </style>
</head>
<body>
   <!-- Barra de navegación -->
   <nav>
      <a href="#perfil">Perfil</a>
      <a href="#habilidades">Habilidades</a>
      <a href="#experiencia">Experiencia</a>
   </nav>
   <!-- Contenedor principal -->
   <div class="container">
      <!-- Sección de información personal ... (tu información personal aquí) -->
      <section id="habilidades" class="habilidades">
         <!-- Sección de habilidades ... (tus habilidades aquí) -->
      </section>
      <!-- Sección de experiencia laboral -->
      <section id="experiencia">
         <h2>Experiencia Laboral</h2>
         <div class="experiencia">
            <h3>Desarrolladora Web - ABC Tech</h3>
            <p>Trabajé en el desarrollo de aplicaciones web utilizando tecnologías como HTML, CSS y JavaScript. Colaboré en proyectos de equipo para entregar soluciones creativas y eficientes.</p>
            <button class="mostrar-info" data-target="info-desarrolladora">Mostrar Detalles</button>
            <p class="info-experiencia" id="info-desarrolladora" style="display: none;">Detalles sobre mi rol como Desarrolladora Web en ABC Tech.</p>
         </div>
         <div class="experiencia">
            <h3>Freelance Web Developer</h3>
            <p>Diseñé y desarrollé sitios web personalizados para clientes, asegurándome de que fueran receptivos y fáciles de usar en diferentes dispositivos.</p>
            <button class="mostrar-info" data-target="info-freelance">Mostrar Detalles</button>
            <p class="info-experiencia" id="info-freelance" style="display: none;">Detalles sobre mi trabajo como Freelance Web Developer.</p>
         </div>
      </section>
   </div>
   <script>
      // Función para mostrar información adicional
      function mostrarInfo(targetId) {
         const infoElement = document.getElementById(targetId);
         if (infoElement) {
            infoElement.style.display = 'block';
         }
      }

      // Agregar eventos de clic a los botones
      const mostrarInfoButtons = document.querySelectorAll('.mostrar-info');

      mostrarInfoButtons.forEach(button => {
         button.addEventListener('click', () => {
            const targetId = button.getAttribute('data-target');
            mostrarInfo(targetId);
         });
      });
   </script>
</body>
</html>
