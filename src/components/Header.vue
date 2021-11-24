<template>
  <div class="container flex">
      <img src="@/assets/dc-logo.png" alt="">
      <ul class="flex">
          <li v-for="(element, index) in menuElements" :key="`element-${index}`">
              <a href="#">{{element.text}}</a>
          </li>
        </ul>
  </div>
</template>

<script>

import menulist from '@/data/MenuList.js';

export default {
    name: 'Header',

    data(){
        return {
            menuElements: menulist,
        };
    },
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
        margin: 0 10px;
        height: 100%;
        border-bottom: 4px solid transparent;
        text-transform: uppercase;
        font-size: .8rem;
        a {
            color: #464646;
            font-weight: 600;
        }
        }
    }
li:hover{
color: blue;
border-bottom: 4px solid #1373BB;
}

img {
    padding-top: 1rem;
    padding-bottom: 1rem;
}
</style>