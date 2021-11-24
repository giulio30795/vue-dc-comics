<template>
<div>
    <div class="img-container">
        <img :src="immagine" :alt="testo">
    </div>
    <h4>{{testo}}</h4>
</div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        immagine: String,
        testo: String,
    },
}
</script>

<style scoped  lang="scss">
.img-container{
            height: 150px;
            
            img{
                object-fit: cover;
                height: 100%;
                width: 100%;
                object-position: top;
            }
        }
</style>