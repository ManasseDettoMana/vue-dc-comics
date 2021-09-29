<template>
    <div class="row">
        <div class="container">
            <div class="col-6 colonna" id="left_column">
                <div class="col-4 " v-for="(link, index) in links" :key='index'>
                    <h2>{{link.name}}</h2>
                    <li v-for="(element, indice) in links[index].linkList" :key="indice" ><a href="#" >{{element}}</a></li>
                </div>
            </div>
            <div class="col-6 colonna" id="dc_bg"></div>
        </div>
    </div>
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

.row{
    height: 400px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-position:center ;
    background-size: cover;

    .container{
        display: flex;
        li{
            list-style-type: none;
        }
        a{
            color: grey;
            font-size: 13px
        }
        h2{
            color: white;
            text-transform: uppercase;
            font-weight: 700;
            font-size: 18px;
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


</style>