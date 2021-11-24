<template>
    <section>
        <div class="container">
            <ul class="thumb-list flex">
                <li v-for="(element, index) in comics" :key="`list-${index}`">
                    <div class="img-container">
                        <img :src="element.thumb" :alt="element.series">
                    </div>
                    <h4>{{element.series}}</h4>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
import comicsList from '@/data/dc-comics.js'
export default {
    name: 'Content',

    data(){
        return {
            comics: comicsList
        }
    }
}
</script>

<style scped lang="scss">
@import '@/styles/general';

section
.thumb-list{
    padding-top: 2.5rem;
    color:#fff;
    flex-wrap: wrap;
    li{
        width: calc(100% / 6);
        padding: .5rem;
        .img-container{
            height: 150px;
            
            img{
                object-fit: cover;
                height: 100%;
                width: 100%;
                object-position: top;
            }
        }
    }
}
section {
    background: #000;
}
</style>