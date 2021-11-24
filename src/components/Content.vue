<template>
    <section>
        <div class="container">
            <ul class="thumb-list flex">
                <li v-for="(element, index) in comics" :key="`list-${index}`">
                    <Card 
                    :immagine="element.thumb"
                    :testo="element.series"
                    />
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
import comicsList from '@/data/dc-comics.js'
import Card from '@/components/Card.vue'
export default {
    name: 'Content',
    components: {
        Card,
    },
    data(){
        return {
            comics: comicsList,
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
        // .img-container{
        //     height: 150px;
            
        //     img{
        //         object-fit: cover;
        //         height: 100%;
        //         width: 100%;
        //         object-position: top;
        //     }
        // }
    }
}
section {
    background: #000;
}
</style>