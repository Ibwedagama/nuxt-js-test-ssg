<template>
 <v-container>
    <h1>CSR</h1>
    <div v-for="(v, i) in data" :key="i">
      <p>{{v}}</p>
    </div>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      data: []
    }
  },
  async mounted() {
    const response = await fetch('https://jsonplaceholder.typicode.com/users')
    const data = await response.json()

    this.data = data
  }
}
</script>
