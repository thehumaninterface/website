<template>
  <div>

    <nav>
      engleză

      servicii, workflow, despre, proiecte, cariere

      contact
    </nav>

    <main>


      <section class="section section-intro">
        <p>interfața umană este preocupată de un singur lucru: experiența utilizatorului</p>
        <p>ideea este să uiți că există un ecran între tine și aplicație</p>
      </section>

      <section class="section section-services">

        <h2>Servicii</h2>
          
        <div class="media">
          <img src="" alt="">
        </div>

        <ul>
          <li>User Research.</li>
          <li>User Experience.</li>
          <li>Graphical User Interface.</li>
          <li>Interaction Design.</li>
          <li>Data visualization.</li>
        </ul>
        <p>Aplicat pe web apps, web sites intranets, etc.</p>

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

<style>
</style>

