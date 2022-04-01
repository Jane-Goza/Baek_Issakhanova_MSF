<template>
<Header />
  <div class="Contact">
    <h1>This is an contact page</h1>
  </div>
<Footer />
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'Contact',
  components: {
    Header,
    Footer,
  },
};
</script>

<style lang="scss">
 @import "src/assets/sass/main.scss";
</style>
