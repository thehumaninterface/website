<template>
  <div>
    <nav class="navmenu">
      engleză

      servicii, workflow, despre, proiecte, cariere

      contact
    </nav>

    <main>
      <section class="section section-intro">

        <div class="media">
          <img src="" alt="main image">          
        </div>
        <p class="large">interfața umană este preocupată de un singur lucru: experiența utilizatorului</p>
        <p class="large">ideea este să uiți că există un ecran între tine și aplicație</p>
      </section>

      <section class="section section-services">
          <h2>Servicii</h2>
          
          <ul>
            <li>User Research.</li>
            <li>User Experience.</li>
            <li>Graphical User Interface.</li>
            <li>Interaction Design.</li>
            <li>Data visualization.</li>
          </ul>
          <p>Aplicat pe web apps, web sites intranets, etc.</p>

        <div class="section-media">
          <img src="" alt="media">
        </div>

      </section>

      <section>
        <h2>Workflow</h2>

        <section>
          <h3>Analiză</h3>
          <p>Transformăm user personas în user flows, specificațiile de conținut în concept map, obiectivele de business în KPI-uri.</p>
        </section>
        <section>
          <h3>Interacțiune</h3>
          <p>Cu focus pe usability, explorăm mai multe variante de wireframe-uri, prototipăm.</p>
        </section>
        <section>
          <h3>Grafică</h3>
          <p>Mockup-uri, ilustrații, animații, style guide, inclusiv identitatea vizuală a produsului.</p>
        </section>
        <section>
          <h3>Livrare</h3>
          <p>Mockup-uri, ilustrații, animații, style guide, inclusiv identitatea vizuală a produsului.</p>
        </section>

      </section>

      <section>
        <h2>Proiecte</h2>
        
        <nav>
          <span class="sr">Categorii de proiecte:</span>
          <ul>
            <li><a href="">game design</a></li>
            <li><a href="">AR/VR</a></li>
            <li><a href="">web app</a></li>
            <li><a href="">b2b</a></li>
            <li><a href="">data visualisation</a></li>
            <li><a href="">intranet</a></li>
          </ul>
          <!-- highlight tags based on scroll. nice! Desktop only -->
          <!-- description on wait or click -->
        </nav>

        <!-- maybe a component? -->
        <div onclick="window.location = '#project'" tabindex="0">
          <h3>
            <a href="#project">Stagii pe Bune</a>
          </h3>
          <img src="" alt="">
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ratione, quaerat. Minus minima sequi maxime expedita libero consequatur dolor nemo sit explicabo, velit voluptatum saepe magnam, adipisci, quasi autem suscipit aspernatur.</p>
          <div class="project-tags">
            <span class="sr">Categorii:</span>
            <a href="#tag" rel="tag">b2b</a>
            <a href="#tag" rel="tag">b2c</a>
            <a href="#tag" rel="tag">web app</a>
          </div>
        </div>
      </section>

      <section class="section section-whyus" id="de-ce-noi">
        <h2>De ce noi?</h2>

        <div class="because because-benefit">
          <p>Toate proiectele încep de la 20%.</p>
          <!-- click to show more -->
        </div>

        <div class="because because-benefit">
          <p>Livrăm de 2 ori pe săptămână.</p>
        </div>

        <div class="because because-benefit">
          <p>Poți verifica oricând la ce lucrăm și cât lucrăm, vezi ciorne, documente de lucru, fișierele sursă, tot.</p>
        </div>

        <div class="because because-benefit">
          <p>Stocare și backup pentru minim 2 ani.</p>
        </div>

        <div class="because because-testimonial">

          <blockquote>
            <div class="quote-body">
              <p>Valentin (the face in interface) has been handling all our UX challenges for more than 5 years. Somehow, I still find myself surprised with his designs.</p>
            </div>
            <footer class="quote-source">
              Andrei Meliș, CEO @ Eau de Web
            </footer>
          </blockquote>
        </div>
      </section>
    </main>

    <nav class="navcontrols">
      next
    </nav>

    <footer>

      <h2>Contact</h2>

      intefața umană
      <a href="mailto:salut@interfataumana.ro">salut@interfataumana.ro</a>

      <strong>Valentin Popescu</strong>
      human interface designer
      <a href="tel:+40728154126">+40 (728) 154 126</a>

      <p>
        Nod Makerspace, Splaiul Unirii nr. 160, Corp C3, Aripa 1 <br>
        040041 Sector 4 – București
      </p>

    </footer>

  </div>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  }
}
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css?family=Montserrat:400,400i,600&subset=latin-ext');

  :root {
    font-size: 8px;

    --gutter: 3rem;
  }
  @media (min-width: 900px) {
    :root {
      font-size: 10px;

      --gutter: 4rem;
    }
  }
  body {
    font-size: 2rem;
    font-family: 'Montserrat', sans-serif;
    line-height: 1.5;

    padding-left: var(--gutter);
    padding-right: var(--gutter);
  }


  .large {
    font-size: 125%;
  }
  

  .container {
    box-sizing: border-box;
    margin-left: auto;
    margin-right: auto;
    padding-left: 3rem;
    padding-right: 3rem;
  }


  @media (max-width: 899px) {
    .navmenu {
    }
    main section {
      min-height: calc(100vh - 12rem);
    }
    .navcontrols {
      position: sticky;
      bottom: 0;
      background: #fff;
    }
  }


  .media {
    position: relative;

    border: 1px solid lightgray;

    img {
      display: block;
    }

    @media (max-width: 899px) {
      margin-bottom: 1em; 
      padding-bottom: 56.25%;
      img {
        position: absolute;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
      }
    }
  }



  body {
    max-width: 1280px;
    margin-left: auto;
    margin-right: auto;
  }



  // you need
  // 1. div before media
  // 2. div for media
  // 3. div after media
  // container takes a 4 row template: 1fr auto auto 1fr;
  // before media row: 2
  // after media row: 3
  // media row-start; 1 / -1

  // .section {
  //   display: grid;
  //   grid-template-columns: 1fr 1fr;
  //   grid-template-rows: 1fr auto auto 1fr;

  //   .section-media {
  //     grid-column: 2;
  //     grid-row: 1 / -1;
  //     height: 40rem;
  //   }
  // }


</style>

