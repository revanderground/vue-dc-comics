<template>
    <div class="footer-bottom">
        <div class="box">
            <div class="sign-up">
                <a href="#">
                    Sign-up Now!
                </a>
            </div>
            <div class="social-icons">
                <h4>Follow us</h4>
                <a href="#" v-for="(element, index) in iconItems" :key="index" class="mx-2">
                    <img :src="require('../assets/img/' + element.image)" alt="Social Logo">
                </a>
            </div>
        </div>
        
    </div>
</template>

<script>
export default {
    data: function(){
        return {
            iconItems: [
                {
                    image: 'footer-facebook.png',
                    url: '#'
                },
                {
                    image: 'footer-twitter.png',
                    url: '#'
                },
                {
                    image: 'footer-youtube.png',
                    url: '#'
                },
                {
                    image: 'footer-pinterest.png',
                    url: '#'
                },
                {
                    image: 'footer-periscope.png',
                    url: '#'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../styles/style.scss";
.footer-bottom{
    height: 6rem;
    background-color: $darkgreycolor;
    padding: 0.8rem 0;
    vertical-align: middle;
    div.box{
        @include d-flex(space-between, center);
        @include box;
      
        height: 100%;
        .sign-up{
            
            a{
                display: inline-block;
                color: white;
                padding: .7rem;
                text-transform: uppercase;
                font-size: .8rem;
                font-weight: bold;
                border: 2px solid $secondaryColor;

            }
        }
        .social-icons{
            @include d-flex('', center);
           
           img{
                height: 25px;
           }
                
           
            a {
                margin-left: 0.9rem;
            }

             h4{
                text-transform: uppercase;
                font-weight: bold;
                color: $secondaryColor;
                font-size: 1.1rem;
                padding-right: 20px;
            }


        }
    }
    
}
</style>