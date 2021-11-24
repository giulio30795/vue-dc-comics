<template>
<div>
    <section class="bg">
        <div class="container flex">
            <div class="left-container flex">
                <div>
                    <ul>
                        <li><h3>DC Comics</h3></li>
                        <li v-for="(element, index) in footer1" :key="`list-${index}`">
                            <a href="">{{element.text}}</a>
                        </li>
                    </ul>
                    <ul>
                        <li><h3>Shop</h3></li>
                        <li v-for="(element, index) in footer2" :key="`list2-${index}`">
                            <a href="">{{element.text}}</a>
                        </li>
                        
                    </ul>
                </div>
                <div>
                    <ul>
                        <li><h3>DC</h3></li>
                        <li v-for="(element, index) in footer3" :key="`list2-${index}`">
                            <a href="">{{element.text}}</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <ul>
                        <li><h3>Sites</h3></li>
                        <li v-for="(element, index) in footer4" :key="`list-${index}`">
                            <a href="">{{element.text}}</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="right-container">
                <img src="../assets/dc-logo-bg.png" alt="">
            </div>
        </div>
    </section>
        <section class="social">
            <div class="container middle flex">
                <div>
                <div class="sign-up">Sign-Up Now!</div>
            </div>
            <div class="follow flex">
                <div>
                follow us
                </div>
                <div>
                    <img src="../assets/footer-facebook.png" alt="">
                    <img src="../assets/footer-twitter.png" alt="">
                    <img src="../assets/footer-youtube.png" alt="">
                    <img src="../assets/footer-pinterest.png" alt="">
                    <img src="../assets/footer-periscope.png" alt="">
                </div>
            </div>
            </div>
        </section>
</div>
    
</template>

<script>

import Footer1 from '@/data/Footer1.js';
import Footer2 from '@/data/Footer2.js';
import Footer3 from '@/data/Footer3.js';
import Footer4 from '@/data/Footer4.js';

export default {
    name: 'Footer',
    data() {
        return {
            footer1: Footer1,
            footer2: Footer2,
            footer3: Footer3,
            footer4: Footer4,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/styles/general';

section.bg{
    background-image: url('../assets/footer-bg.jpg');
    background-size:cover ;
}

.middle{
    justify-content: space-between;
}
.left-container{
    div {
        padding: 20px 20px 20px 0;
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
.right-container{
    position: relative;
        img{
            position: absolute;
            top: 10px;
            left:300px;
            max-width: 400px;
            height: 400px;
        }
}

.social{
    background-color: #303030;
    justify-content: space-between;
    padding: 20px 0;
    position: relative;
    
}
.sign-up{
    border: 1px solid #0D7CEC;
    padding: 10px;
    color: #fff;
    box-sizing: border-box;
}
.follow{
    color: #1373BB;
    text-transform: uppercase;
    img{
        max-width: 30px;
        max-height: 30px;
        margin: 0.2rem;
    }
    div {
        align-self: center;
        margin-right: 10px;
        font-weight: bold;
    }
}
</style>