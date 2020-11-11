<template>
  <div class="home">
    <WebClient/>
  </div>
</template>

<script>
// @ is an alias to /src
import WebClient from '@/components/WebClient.vue'

export default {
  name: 'Home',
  components: {
    WebClient
  }
}
</script>
