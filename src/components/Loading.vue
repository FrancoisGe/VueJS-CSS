<template>
  <div class="loading-container">
      <h2 class="loading-item" data="Loading...">Loading...</h2>
  </div>
</template>

<script>

export default {
  name: 'Loading',

}
</script>

<style scoped>
.loading-container {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 80vh;
    background: #252839;
}
.loading-item {
    position: relative;
    font-size: 14vh;
    color: #252839;
    -webkit-text-stroke: 0.3vw #383d52;
    text-transform: uppercase;
}
.loading-item::before {
    content: attr(data);
    position: absolute;
    top:0;
    left: 0;
    width: 0;
    height: 100%;
    color: #01fe87;
    -webkit-text-stroke: 0vw  #383d52;
    border-right: 2px solid #01fe87;
    overflow: hidden;
    animation: loading 6s linear infinite;
}
@keyframes loading {
    0%, 10%, 100% {
        width: 0;
    }
    70%, 90% {
        width: 100%;
    }
    
}
</style>
