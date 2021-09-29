<template>
    <footer>
        <div class="row" id="row_bg">
            <div class="container" >
                <div class="col-6 colonna" id="left_column">
                    <div class="col-3 piccola_colonna" v-for="(link, index) in links" :key='index'>
                        <h2>{{link.name}}</h2>
                        <li v-for="(element, indice) in links[index].linkList" :key="indice" ><a href="#" >{{element}}</a></li>
                    </div>
                </div>
                <div class="col-6 colonna" id="dc_bg"></div>
            </div>
        </div>
        <div class="row" id="scnd_row">
            <div class="container">
                <div class="col-6">
                    <button>sing-up now!</button>
                </div>
                <div class="col-6">
                    
                    <ul>
                        <li><h2>follow us</h2></li>
                        <li><a href=""><img src="../assets/img/footer-facebook.png" alt=""></a></li>
                        <li><a href=""><img src="../assets/img/footer-twitter.png" alt=""></a></li>
                        <li><a href=""><img src="../assets/img/footer-youtube.png" alt=""></a></li>
                        <li><a href=""><img src="../assets/img/footer-pinterest.png" alt=""></a></li>
                        <li><a href=""><img src="../assets/img/footer-periscope.png" alt=""></a></li>
                    </ul>
                </div>
            </div>
        </div>
        
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    components: {

    },
    data: function(){
        return{

            links: [
                {
                    name: 'dc comics',
                    linkList: [
                        "Characters", 
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News'
                        
                    ]
                },
                {
                    name: 'shop',
                    linkList: [
                        'Shop DC',
                        'Shop DC Collectibles'
                    ]
                },
                {
                    name: 'dc',
                    linkList: [
                        'Terms Of Use',
                        'Privacy policy (New)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contac Us'
                    ]
                },
                {
                    name: 'sites',
                    linkList: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        '   DC Power Visa'
                    ]                    
                }
            ]
        }
    }
}

</script>

<style lang="scss" scoped>
@import './style/variables.scss';
#row_bg{
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-position:center ;
    background-size: cover;
    height: 400px;
}
.row{
    .container{
        display: flex;

        .piccola_colonna{
            padding-top: 50px
        }
        li{
            list-style-type: none;
        }
        a{
            color: grey;
            font-size: 12px
        }
        h2{
            color: white;
            text-transform: uppercase;
            font-weight: 700;
            font-size: 17px;
        }
        #left_column{
            display: flex;

        }
        .colonna{
            height: 100%;
 
        }
        #dc_bg{
            background-image: url('../assets/img/dc-logo-bg.png');
            background-position: center ;
        }
    }
}

#scnd_row{
    height: 100px;
    background-color: rgb(56, 56, 56);
    .container{
        display: flex;
        justify-content: center;
        align-items: center;
        button{
            text-transform: uppercase;
            color: white;
            height: 50px;
            width: 150px;
            border: 2px solid $bluCeleste;
            background-color:rgb(56, 56, 56);
        }
        h2{
            font-size: 1.3em;
            color: $bluCeleste;
            margin: 0;
            height: 100%;
        }
        ul{
            display: flex;
            justify-content: space-evenly;
        }
    }
}


</style>