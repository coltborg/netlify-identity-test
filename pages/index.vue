<template>
  <div class="min-h-screen bg-yellow-lightest">
    <header class="mb-4 px-4 flex justify-between items-center bg-yellow text-black shadow-md">
      <h1 class="my-4 text-3xl">Netlify Identity Test</h1>
      <div data-netlify-identity-menu></div>
    </header>

    <section
      v-if="user"
      class="mx-4 px-6 py-8 bg-white shadow rounded">
      <AppContent />
    </section>

    <section
      v-else
      class="mx-4 px-6 py-8 bg-white shadow rounded">
      Please login to see content.
    </section>
  </div>
</template>

<script>
import netlifyIdentity from "netlify-identity-widget";
import AppContent from "~/components/Content.vue";

export default {
  components: {
    AppContent
  },
  data() {
    return {
      user: null
    };
  },
  mounted() {
    window.netlifyIdentity = netlifyIdentity;
    // You must run this once before trying to interact with the widget
    netlifyIdentity.init();

    // If page is refreshed and user is already logged in
    if (netlifyIdentity.currentUser()) {
      this.user = netlifyIdentity.currentUser();
    }

    netlifyIdentity.on("init", user => console.log(user));
    netlifyIdentity.on("login", user => {
      console.log(user);
      this.user = user;
    });
    netlifyIdentity.on("logout", () => {
      console.log("Logged out");
      this.user = null;
    });
    netlifyIdentity.on("error", err => console.error("Logged out"));
    netlifyIdentity.on("open", () => console.log("Widget opened"));
    netlifyIdentity.on("close", () => console.log("Widget closed"));
  }
};
</script>

<style lang="postcss">
@tailwind preflight;
@tailwind utilities;

.netlify-identity-menu {
  @apply flex list-reset;
}

.netlify-identity-item {
  @apply mx-2;
}

.netlify-identity-login,
.netlify-identity-logout,
.netlify-identity-signup {
  @apply no-underline text-black;
}

.netlify-identity-login:hover,
.netlify-identity-logout:hover,
.netlify-identity-signup:hover {
  @apply text-grey-darker;
}
</style>
