<template>
    <div>
        
        <div class="main-top">
            <div class="box-jumbotron">
                <div class="jumbotron"></div>
             </div>
        </div>
       
    </div>

  
    
</template>

<script>
export default {
    
  

}
</script>

<style lang="scss" scoped>
    @import "../styles/style.scss";
    
    template{
        background-color: $darkColor;
    }

    .main-top{
        background-color: $darkColor;
        height:25rem;
        @include my-container;

        
        .box-jumbotron{

            .jumbotron{
                height: 25rem;
                background-image:url("../assets/img/jumbotron.jpg");
                background-size: cover;
            }
        
        }
       
    }




    
    

</style>