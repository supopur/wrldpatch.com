

<template>
  Helloooo
<h1>Response: {{ response }}</h1>
</template>

<script>
import axios from 'axios'

export default {
  name: "Index",
  data() {
    return {
      response: null
    };
  },
  methods: {
    getResponse() {
      axios.get('https://mpe31fbb95bcd70113f8.free.beeceptor.com/').then((response) => {
        this.response = response.data;
      })
    }
  },
  mounted() {
    this.getResponse();
  }

}



</script>

<style scoped>

</style>