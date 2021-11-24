<template>
  <div class="hero">
       <span class="current">
           Current Series
       </span>
  </div>
</template>

<script>
export default {
    name: 'Hero',
}
</script>

<style scoped lang="scss">
.hero{
    height: 400px;
    background-image: url('../assets/jumbotron.jpg');
    background-position: top;
    position: relative;
    .current{
        background-color:#0D7CEC;
        color: #fff;
        padding: .8rem;
        text-transform: uppercase;
        font-weight: 600;
        position: absolute;
        top: 95%;
        left: 19%;
    }
}
</style>