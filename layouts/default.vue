<template>
  <v-app dark>
    <div class="d-flex mb-6">
      <NuxtLink class="subtitle-2 primary--text mr-4" to="/">Home</NuxtLink>
      <NuxtLink class="subtitle-2 primary--text" to="/about">About</NuxtLink>
    </div>
    <v-main>
      <Nuxt />
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: "mdi-apps",
          title: "Welcome",
          to: "/"
        },
        {
          icon: "mdi-chart-bubble",
          title: "Inspire",
          to: "/inspire"
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "Vuetify.js"
    };
  }
};
</script>
