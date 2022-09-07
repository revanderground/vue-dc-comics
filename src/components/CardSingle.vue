<template>
    <div>
            <div class="wrapper-cards">

                <div class="card-image">
                    <img :src="oneCard.thumb">
                </div>
                <div class="card-title">
                    {{oneCard.series}}
                </div>


            </div>
                

    </div>
  
  
</template>

<script>
export default {
   
    props: {
        oneCard: Object
    }
}
</script>

<style lang="scss" scoped>

   .wrapper-cards{

         
             .card-image{
                
                width:100%;
                overflow:hidden;
                height: 9rem;
                border:-1px;
                transition: 0.5s ease;
            }

            .card-image:hover{
                filter: saturate(0.6) opacity(0.5);
                cursor: pointer;
                scale: 1.05;

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