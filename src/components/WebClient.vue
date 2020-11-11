<template>
  <div class="hello">
    <h1>Application with multi CSS exemple</h1>
    <div class="flex flex-wrap">
      <Card v-for="card in cards" :key="card.title" class="flex-1 " :title="card.title" :link="card.link"></Card>
    </div>
  </div>
</template>

<script>
import Card from './Card.vue'

export default {
  name: 'WebClient',
  components: {
    Card,
  },
  data: function () {
    return {
      cards: [
        {title: "Loading", link: "/loading"},
        {title: "Card 2", link: "/c2"},
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
