<template>
    <div class="row">
        <div class="container">
            <nav>
                <li><a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt=""><span>digital comics</span></a></li>
                <li><a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt=""><span>dc merchandise</span></a></li>
                <li><a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt=""><span>subscription</span></a></li>
            </nav>
        </div>
    </div>
</template>

<script>
export default {

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
                color: white;
                &:hover{
                    text-decoration: underline;
                }
                span{
                    text-transform: uppercase;
                    margin-left: 20px;
                }
            }
        }
    }
}

img{
    width: 50px;
}

</style>