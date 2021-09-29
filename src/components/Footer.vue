<template>
    <div class="row">
        <div class="container">
            <div class="col-6 colonna" id="left_column">
                <div class="col-3 colonna"></div>
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
                    link: [
                        'Characters',
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
                    link: [
                        'Shop DC',
                        'Shop DC Collectibles'
                    ]
                },
                {
                    name: 'dc',
                    link: [
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
                    nmae: 'sites',
                    link: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        ' DC Power Visa'
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