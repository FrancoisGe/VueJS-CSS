<template>
  <div class="m-2  bg-gray-200 p-2">
    <router-link :to="link">
        <h1>{{title}}</h1>
        <div>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptas, repudiandae? Nam laudantium repudiandae dolor libero aut quis dolore earum asperiores hic vero sunt accusantium, voluptate maiores quae ea laboriosam. Delectus.
        </div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
      title: String,
      link: String,
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
