<template>
    <div class="wrapper-cards">
                <div class="card-image">
                    <img :src="oneCard.thumb">
                </div>
                <div class="card-title">
                    {{oneCard.series}}
                </div>

    </div>
  
  
</template>

<script>
export default {
   
    props: {
        oneCard: Objects
    }
}
</script>

<style lang="scss" scoped>

 .album-card{
            width:calc((100% / 6) - 1rem);

             .card-image{
                
                width:100%;
                overflow:hidden;
                height: 9rem;
                border:-1px;
            }

            .card-title{
                color:white;
                font-size: 0.8rem;
                font-weight: 500;
                text-align:center;
                text-transform: uppercase;
                padding-top: 3px;
            }
 }


</style>