<template>
  <section class="">
    <div>
      <h1 class="text-3xl bg-yellow text-black">
        Identity Test
      </h1>
      <div data-netlify-identity-menu></div>
      <div data-netlify-identity-button>Login with Netlify Identity</div>
    </div>
  </section>
</template>

<script>
import netlifyIdentity from "netlify-identity-widget";

export default {
  mounted() {
    window.netlifyIdentity = netlifyIdentity;
    // You must run this once before trying to interact with the widget
    netlifyIdentity.init();
  }
};
</script>

<style lang="postcss">
@tailwind preflight;
@tailwind utilities;
</style>
