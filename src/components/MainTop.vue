<template>
    <section class="main-top">
         <div class="box-title">
            <div class="title"> --> Content goes here &lt;-- </div>
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
        height:100px;
        @include my-container;

        .title{
        color:$fontColorInvert;
        padding-top: 20px;
        font-size: 2rem;
    }

    .box-title{
        @include box;
    }

    }

    
    

</style>