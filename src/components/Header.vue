<template>
    <header>
        <div class="container">
            <div class="row">
                <div class="col-4">
                    <a href="#">
                        <img src="../assets/img/dc-logo.png" alt="">
                    </a>
                </div>
                <div class="col-8 ">
                    <nav>
                        <ul class="d-flex justify-content-between justify-content-center align-items-center">
                            <li v-for="(element, index) in navLInk" :key="index" :class="{active : element.active}"><a :href='element.link' :class="{active : element.active}" >{{element.name}}</a></li>
                        </ul>
                    </nav>
                </div>
            </div>
        </div>
    </header>
</template>



<script>
export default {
    name: 'Header',

    data: function(){
        return{
            navLInk: [
                {
                    name: 'characters',
                    link: '#',
                    active: false
                },
                {
                    name: 'comics',
                    link: '#',
                    active: true
                },
                {
                    name: 'movies',
                    link: '#',
                    active: false
                },
                {
                    name: 'tv',
                    link: '#',
                    active: false
                },
                {
                    name: 'games',
                    link: '#',
                    active: false
                },
                {
                    name: 'collectibles',
                    link: '#',
                    active: false
                },
                {
                    name: 'videos',
                    link: '#',
                    active: false
                },
                {
                    name: 'fans',
                    link: '#',
                    active: false
                },
                {
                    name: 'news',
                    link: '#',
                    active: false
                },
                {
                    name: 'shop',
                    link: '#',
                    active: false
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import './style/variables.scss';
    .row{
      padding-top:50px;

        img{
            width: 75px;
        }
        nav{
            line-height: 75px;

            ul{
                height: 100%;
                margin: 0;
                display: flex;
                justify-content: space-evenly;
                li{
                    list-style-type: none;
                    height: 100%;
                    &.active{
                        color: $bluCeleste;
                        border-bottom: 3px solid $bluCeleste;
                    }
                    &:hover{
                        border-bottom: 3px solid $bluCeleste;
                    }
                    a{
                        color: black;
                        text-transform: uppercase;
                        font-weight: 700;
                        font-size: 13px;
                        &:hover{
                            text-decoration: none;
                        }


                    }
                }
            }
        }
        
        
    }
</style>