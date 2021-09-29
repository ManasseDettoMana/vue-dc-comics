<template>
    <div class="row" id="root">
        <div class="container">
            <nav>
                <li v-for="(link, index) in infoLink" :key="index">
                    <a href="#">
                        <div>
                            <img :src="link.url" alt="">
                        </div>
                        <span>{{link.text}}</span>
                    </a>
                </li>
            </nav>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PageNav',
    components: {
        
    },
    data: function(){
        return{
            infoLink: [
                {
                    url: '../assets/img/buy-comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    url: '../assets/img/buy-comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    url: '../assets/img/buy-comics-subscriptions.png',
                    text: 'subscription'
                },
                {
                    url: '../assets/img/buy-comics-shop-locator.png',
                    text: 'comic shop locator'
                },
                {
                    url: '../assets/img/buy-dc-power-visa.svg',
                    text: 'dc power visa'
                },       
            ]
        }
    }   
}
 




</script>

<style scoped lang="scss">
@import './style/variables.scss';
.row{
    background-color: $bluCeleste;
    height: 170px;
}
.container{
    display: flex;
    justify-content: center;
    align-items: center;

    nav{
        width: 100%;
        display: flex;
        justify-content: space-between;

        li{
            list-style-type: none;
            a{
                display: flex;
                justify-content: center;
                align-items: center;
                color: white;
                font-size: 0.9rem;
                &:hover{
                    text-decoration: underline;
                }
                span{
                    text-transform: uppercase;
                    margin-left: 15px;

                }
                img{
                    width: 50px;
                }
                div{
                    width: 60px;
                    height: 60px;
                    img{
                        width: 100%;
                        height: 100%;
                    }
                }
            }
        }
    }
}


</style>