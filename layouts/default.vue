<template>
  <div v-bind:class="{ 'navbar-is-open': navbarIsOpen }">

    <Navigation/>

    <nuxt/>
  </div>
</template>

<script>
import EventBus from '~/components/Events.js';
import Navigation from '~/components/Navigation.vue';

export default {
  components: {
    Navigation
  },
  data() {
    return {
      navbarIsOpen: false
    }
  },
  mounted() {
    var vueInstance = this;
    EventBus.$on('navbar-toggle', payload => {
      this.navbarIsOpen = payload.isOpen;
    });
  }
}
</script>

