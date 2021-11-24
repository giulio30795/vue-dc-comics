<template>  
    <section>
        <div class="container">
            <ul class="flex">
                <li class="flex">
                    <img src="../assets/buy-comics-digital-comics.png" alt="">
                    <span>Digital Comics</span>
                </li>
                <li class="flex">
                    <img src="../assets/buy-comics-merchandise.png" alt="">
                    <span>Dc Merchandise</span>
                </li>
                <li class="flex">
                    <img src="../assets/buy-comics-subscriptions.png" alt="">
                    <span>Subscriptions</span>
                </li>
                <li class="flex">
                    <img src="../assets/buy-comics-shop-locator.png" alt="">
                    <span>Comic Shop Locator</span>
                </li>
                <li class="flex">
                    <img src="../assets/buy-dc-power-visa.svg" alt="">
                    <span>DC Power Visa</span>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Shop'
}
</script>

<style scoped lang="scss">

section{
    background-color:#1883F9 ;
    width: 100%;
    ul {
        justify-content: center;
        width: 100%;
        padding: 1rem 0;
        li {
            justify-content: center;
            width: 100%;
            align-items: center;
            color: #fff;
            font-size: 0.8rem;
            text-transform: uppercase;
        }
        img{
            width: 16%;
            margin-right: .5rem;
            
        }
    }
}




</style>