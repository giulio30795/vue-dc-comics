<template>
    <section>
        <div class="container flex">
            <div class="left-container flex">
                <div>
                    <ul>
                        <li><h3>Titolo</h3></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                    </ul>
                    <ul>
                        <li><h3>Titolo</h3></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                    </ul>
                </div>
                <div>
                    <ul>
                        <li><h3>Titolo</h3></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                    </ul>
                    <ul>
                        <li><h3>Titolo</h3></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                    </ul>
                </div>
                <div>
                    <ul>
                        <li><h3>Titolo</h3></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                        <li><a href="">Contenuto</a></li>
                    </ul>
                </div>
            </div>
            <div class="right-container">
                <img src="../assets/dc-logo-bg.png" alt="">
                d
            </div>
        </div>
        <section class="social">
            social
        </section>
    </section>
    
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="scss" scoped>
@import '@/styles/general';

section{
    background-image: url('../assets/footer-bg.jpg');
    background-size:cover ;
}

.container{
    justify-content: space-between;
}
.left-container{
    div {
        padding: 20px 20px;
    }
    h3 {
        color: white;
        font-size: 1.3rem;
        margin: 10px 0;
    }
    a{
        color: lightgrey;
        font-size: 0.75rem;
        margin: 10px 0;
    }
}
.social{
    background-color: grey;
    
}
</style>