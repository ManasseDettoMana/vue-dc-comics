<template>
    <div class="row">
        <div class="container">
            <div class="col-6 colonna"></div>
            <div class="col-6 colonna" id="dc_bg"></div>
        </div>
    </div>
</template>

<script>
export default {

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