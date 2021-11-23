<template>
  <div class="container flex">
      <img src="@/assets/dc-logo.png" alt="">
      <ul class="flex">
          <li>
              <a href="#">TEST</a>
          </li>
          <li>
              <a href="#">TEST</a>
          </li>
          <li>
              <a href="#">TEST</a>
          </li>
          <li>
              <a href="#">TEST</a>
          </li>
          <li>
              <a href="#">TEST</a>
          </li>
          <li>
              <a href="#">TEST</a>
          </li>
          <li>
              <a href="#">TEST</a>
          </li>
          <li>
              <a href="#">TEST</a>
          </li>
          <li>
              <a href="#">TEST</a>
          </li>
          <li>
              <a href="#">TEST</a>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
    name: 'Header',
}
</script>

<style scoped lang="scss">
@import '@/styles/general';

div.container {
    justify-content: space-between;
    align-self: center;
    height: 130px;
}
.flex{
    display: flex;
}

ul {
    height: 100%;
    li {
        display: flex;
        align-items: center;
        margin: 0 20px;
        height: 100%;
        border-bottom: 4px solid transparent;
        }
    }
li:hover{
color: blue;
border-bottom: 4px solid blue;
}

img {
    padding-top: 1rem;
    padding-bottom: 1rem;
}
</style>