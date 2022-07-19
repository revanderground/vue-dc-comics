<template>
    <section class="main-top">
         <div class="box-jumbotron">
            <div class="jumbotron"></div>
        </div>
    </section>
   
    
</template>

<script>
export default {

}
</script>

<style lang="scss">
    @import "../styles/style.scss";
    
    template{
        background-color: $darkColor;
    }

    .main-top{
        background-color: $darkColor;
        height:20rem;
        @include my-container;
       
    }

    .box-jumbotron{

        .jumbotron{
            height: 25rem;
            background-image:url("../assets/img/jumbotron.jpg");
            background-size: cover;
        }
    
    }



    
    

</style>