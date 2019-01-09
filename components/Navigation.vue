<template>
  <nav class="navbar" v-bind:class="{ 'is-open': isOpen }">

    <div class="navbar-language">
      <a href="">Română</a>
    </div>

    <div class="navbar-menu">

      <ul v-show="isOpen">
        <li><nuxt-link to="/services">Services</nuxt-link></li>
        <li><nuxt-link to="/workflow">Workflow</nuxt-link></li>
        <li><nuxt-link to="/projects">Projects</nuxt-link></li>
        <li><nuxt-link to="/about">About</nuxt-link></li>
        <li><nuxt-link to="/careers">Careers<!-- <span class="count">4</span> --></nuxt-link></li>
      </ul>

      <button type="button" class="navbar-menu-toggle" v-on:click="toggle()">
        <svg v-show="!isOpen"  width="32" height="32" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M24.67 20.67v2H7.33v-2h17.34zm0-5.34v2H7.33v-2h17.34zm0-5.33v2H7.33v-2h17.34z" fill="currentColor"/></svg> 
        <svg v-show="isOpen" width="33" height="32" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M17.42 16l5.42 5.42-1.42 1.41-5.41-5.41-5.42 5.42-1.42-1.42L14.6 16l-5.42-5.42 1.41-1.42 5.43 5.43 5.42-5.42 1.41 1.41L17.42 16z" fill="currentColor"/></svg>
        <span class="sr">{{ isOpen ? 'Close menu' : 'Open menu'}}</span>
      </button>

    </div>

    <div class="navbar-action">
      <a href="#contact">Contact</a>
    </div>

  </nav>
</template>

<script>
import EventBus from '~/components/Events.js';

export default {
  data() {
    return {
      isOpen: false
    }
  },
  watch: {
    isOpen(newValue) {
      EventBus.$emit('navbar-toggle', { isOpen: newValue });
    }
  },
  methods: {
    toggle() {
      this.isOpen = !this.isOpen;
      
    }
  },
  mounted() {
    var mq = window.matchMedia('(min-width: 900px)');
    var vueInstance = this;

    function checkMedia(e) {
      if (e.matches) {
        vueInstance.isOpen = true;
      } else {
        vueInstance.isOpen = false;
      }
    }

    checkMedia({ matches: mq.matches });

    mq.addListener(checkMedia);
  }
}
</script>


<style lang="scss">
  @import '@/assets/scss/navbar.scss';
</style>

