<template>

    <section>
        <div class="box-main">
            <ul class="d-flex justify-content-center py-4">
                <li class="px-2 pt-3" v-for="(element, index) in mainBottomItems" :key="index" >
                    <a class="d-flex px-2" :href="element.url">
                        <img class="px-2" :src="require('../assets/img/' + element.image)" >
                        <p class="pt-2">{{element.text}}</p>
                    </a>
                </li>
            </ul>

        </div>

    </section>
  
</template>

<script>

export default {

    data: function() {
        return {
            mainBottomItems: [
                {
                    text: 'DIGITAL COMICS',
                    url: '#',
                    image: 'buy-comics-digital-comics.png'
                },
                {
                    text: 'DC MERCHADISE',
                    url: '#',
                    image: 'buy-comics-merchandise.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    url: '#',
                    image: 'buy-comics-shop-locator.png'
                },
                {
                    text: 'SUBSCRIPTIONS',
                    url: '#',
                    image: 'buy-comics-subscriptions.png'
                },
                {
                    text: 'POWER VISA',
                    url: '#',
                    image: 'buy-dc-power-visa.svg'
                }
            ]
        }
    }
}

</script>

<style lang="scss" scoped>
    @import "~bootstrap/scss/bootstrap.scss";
    @import "../styles/style.scss";

    section{
  
        background-color:$secondaryColor;
        .box-main{
           
            height:130px;
            

            ul{         
                @include box; 
                li{
                    color: $primary;
                
                   p{
                        color:$primary;
                        font-size: 0.81rem;
                        font-weight: 500;
                    }

                    img{
                        height:45px;

                    }


                }

                 
                
            }
        }


    }

</style>