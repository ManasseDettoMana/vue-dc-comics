<template>
    <div class="row" id="root">
        <div class="container">
            <nav>
                <li v-for=""><a href="#"><div id="info_image_container"></div><span></span></a></li>
            </nav>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PageNav',
    data: function(){
        return{
            infoLink: [
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
        justify-content: space-around;

        li{
            list-style-type: none;
            a{
                display: flex;
                justify-content: center;
                align-items: center;
                color: white;
                &:hover{
                    text-decoration: underline;
                }
                span{
                    text-transform: uppercase;
                    margin-left: 20px;

                }
                img{
                    width: 50px;
                }
                #info_image_container{
                    width: 60px;
                    height: 60px;
                    background-image: url('../assets/img/buy-comics-digital-comics.png');
                    background-position: center;
                    background-size: contain;
                    background-repeat: no-repeat;
                }
            }
        }
    }
}


</style>