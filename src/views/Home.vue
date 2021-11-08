<template>
  <div class="homa">
    <nav class="navbar">
      <div class="container">
        <div class="navbar__logo">
          <p class="navbar__title">
            <a href="#">LS2D</a>
          </p>
        </div>
        <div class="navbar__menu">
          <i class="fas fa-bars"></i>
        </div>
        <ul class="navbar__links">
          <li class="navbar__link active" data-ref="home">
            <a href="#home">Inicio</a>
          </li>
          <li class="navbar__link" data-ref="about">
            <a href="#about">¿Quienes somos?</a>
          </li>
          <li class="navbar__link" data-ref="services">
            <a href="#services">Servicios</a>
          </li>
          <li class="navbar__link" data-ref="team">
            <a href="#equipo">Equipo</a>
          </li>
          <li class="navbar__link" data-ref="contact">
            <a href="#contact">Contacto</a>
          </li>
        </ul>
      </div>
    </nav>
    <section id="home" class="home">
      <div class="home__background"></div>
      <picture>
        <source type="image/jpeg" srcset="@/assets/img/crew.jpeg" />
        <img class="home__profile" alt="picture profile" />
      </picture>
      <div class="home__description">
        <h1 class="home__title">LS2D</h1>
        <span class="home__title--secondary"
          >Desarrollo de soluciones analizando necesidades y promoviendo
          innovación</span
        >
      </div>
    </section>
    <section id="about">
      <div class="container">
        <h2 class="section__title">¿Quienes somos?</h2>
        <div class="about__grid">
          <div class="about__description">
            <h2>LS2D</h2>
            <h2>Desarrollo de soluciones</h2>
            <p class="midiom">
              Buscamos generar un impacto positivo a través de la ejecución de
              nuevos proyectos que permitan maximizar las oportunidades de
              desarrollo tecnológico. Ofreciendo a nuestros clientes
              servicios de excelencia, de acuerdo con las necesidades del
              usuario, esto a través de una búsqueda constante de la alta
              calidad de la mano de la innovación, asimismo realizando el
              pertinente estudio y gestión de los proyectos de desarrollo, diseñando ofertas que cumplan con los requerimientos
              de calidad, y la relación costo/beneficio de nuestros clientes
            </p>
          </div>
          <div class="about__skills">
            <picture>
              <source type="image/jpeg" srcset="@/assets/img/coder.png" />
              <img class="coder-img" alt="picture profile" />
            </picture>
          </div>
        </div>
      </div>
    </section>

    <section id="services">
      <div class="container">
        <h2 class="section__title">Servicios</h2>
        <h3 class="section__subtitle">¿Qué ofrecemos a nuestros clientes?</h3>
        <div class="services__grid">
          <div class="services__item">
            <i class="fas fa-mobile-alt"></i>
            <h3>Totalmente Responsivo</h3>
            <p>
              Su sitio se mostrará correctamente en cualquier dispositivo, incluidas computadoras de escritorio, tabletas y teléfonos móviles.
            </p>
          </div>
          <div class="services__item">
            <i class="fas fa-pencil-ruler"></i>
            <h3>Diseños Creativos</h3>
            <p>
              Un buen y atractivo diseño web le ayuda a mantener sus clientes potenciales en su sitio, que es la cara digital de su negocio.
            </p>
          </div>
          <div class="services__item">
            <i class="fas fa-code"></i>
            <h3>Desarrollo</h3>
            <p>
              Desarrollamos aplicaciones de todo tipo utiles y funcionales, mas halla de lo que desea obtendrá lo que necesita
            </p>
          </div>
          <div class="services__item">
            <i class="fas fa-thumbs-up"></i>
            <h3>Integracion De Redes Sociales</h3>
            <p>
              Existen muchas plataformas sociales y debes promover tu presencia en ellas en tu sitio web.
            </p>
          </div>
          <div class="services__item">
            <i class="fas fa-tachometer-alt"></i>
            <h3>Performance</h3>
            <p>
              Retener a los usuarios es fundamental para mejorar las conversiones. Los sitios de alto rendimiento atraen y retienen a los usuarios
            </p>
          </div>
          <div class="services__item">
            <i class="fas fa-crosshairs"></i>
            <h3>SEO</h3>
            <p>
              Optimizarémos su sitio con una estrategia inteligente de optimización de motores de búsqueda para generar clientes potenciales..
            </p>
          </div>
        </div>
      </div>
    </section>
    <section id="equipo">
      <div class="container">
        <h2 class="section__title">Equipo</h2>
        <h3 class="section__subtitle">
          ¿Quienes conforman LS2D?
        </h3>
        <div class="team__grid">
          <div class="team__item">
            <picture>
              <source type="image/jpeg" srcset="@/assets/img/diego.jpeg" />
              <img class="team__img" alt="team item" />
            </picture>
            <div class="team__description">
              <h3 class="team__description--title">Diego Ramos</h3>
              <p class="team__description--text">
                Gerente de proyectos
              </p>
              <div class="buttons__container">
                <!-- <a
                  class="button"
                  href="https://platzi-video-react-app.netlify.app/"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  <i class="fas fa-globe-americas"></i> Website
                </a> -->
                <a
                  class="button"
                  href="https://github.com/Blodige-D"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  <i class="fab fa-github"></i> Repositorio
                </a>
              </div>
            </div>
          </div>
          <div class="team__item">
            <picture>
              <source type="image/jpeg" srcset="@/assets/img/sair.jpg" />
              <img class="team__img" alt="team item" />
            </picture>
            <div class="team__description">
              <h3 class="team__description--title">
                Wilmer Ramos
              </h3>
              <p class="team__description--text">
                CEO
              </p>
              <div class="buttons__container">
                <a
                  class="button"
                  href="http://sramos.ls2d.com"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  <i class="fas fa-globe-americas"></i> Web
                </a>
                <a
                  class="button"
                  href="https://github.com/s-ramosm"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  <i class="fab fa-github"></i> Repositorio
                </a>
              </div>
            </div>
          </div>
          <div class="team__item">
            <picture>
              <source type="image/jpeg" srcset="@/assets/img/leey.jpeg" />
              <img class="team__img" alt="team item" />
            </picture>
            <div class="team__description">
              <h3 class="team__description--title">Leeynyker Montaño</h3>
              <p class="team__description--text">
                CTO
              </p>
              <div class="buttons__container">
                <!-- <a
                  class="button"
                  href="https://jgestradam.github.io/Simon-says-game/"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  <i class="fas fa-globe-americas"></i> Website
                </a> -->
                <a
                  class="button"
                  href="https://github.com/Leeynyker"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  <i class="fab fa-github"></i> Repositorio
                </a>
              </div>
            </div>
          </div>
          <div class="team__item">
            <picture>
              <source type="image/jpeg" srcset="@/assets/img/david.jpeg" />
              <img class="team__img" alt="team item" />
            </picture>
            <div class="team__description">
              <h3 class="team__description--title">David Arias</h3>
              <p class="team__description--text">
                Gerente comercial, Lider de tecnología
              </p>
              <div class="buttons__container">
                <a
                  class="button"
                  href="https://github.com/Davarias"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  <i class="fab fa-github"></i> Repositorio
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section id="contact">
      <div class="container">
        <h2 class="section__title">Contacto</h2>
        <h3 class="section__subtitle">
          Contactese con nosotros
        </h3>
        <div class="contact__grid">
          <a
            href="mailto:coders.l2sd@gmail.com"
            target="_blank"
            rel="noopener noreferrer"
          >
            <div class="contact__item">
              <i class="far fa-envelope"></i>
              <p>Enviar mail</p>
            </div>
          </a>

          <a
            href="https://github.com/LS2D-coders"
            target="_blank"
            rel="noopener noreferrer"
          >
            <div class="contact__item">
              <i class="fab fa-github"></i>
              <p>Siguenos</p>
            </div>
          </a>
          <a
            href="https://twitter.com/"
            target="_blank"
            rel="noopener noreferrer"
          >
            <div class="contact__item">
              <i class="fab fa-twitter"></i>
              <p>Siguenos</p>
            </div>
          </a>
          <a
            href="#"
            target="_blank"
            rel="noopener noreferrer"
          >
            <div class="contact__item">
              <i class="fab fa-linkedin-in"></i>
              <p>Contactanos</p>
            </div>
          </a>
        </div>
      </div>
    </section>
    <footer class="footer">
      <div class="container">
        <p>
          Copyright © 2021. <a href="#">LS2D</a> <br />
        </p>
      </div>
    </footer>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
  },
};
</script>
