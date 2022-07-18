<template>
    <footer>
        <div class="footer-content">
            <div class="footer-content-items d-flex ">
                <div class="col pt-4">
                    <h4>Dc Comics</h4>
                    <ul>
                        <li v-for="(link, index) in dcComicsLinks" :key="index">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>
                    <h4>Shop</h4>
                    <ul>
                        <li v-for="(link, index) in shopLinks" :key="index">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>
                </div>

                <div class="col pt-4">
                    <h4>Dc</h4>
                    <ul>
                        <li v-for="(link, index) in dcLinks" :key="index">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>
                </div>
                <div class="col pt-4">
                    <h4>Sites</h4>
                    <ul>
                        <li v-for="(link, index) in sitesLinks" :key="index">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>

                    
                </div>


                <div class="footer-bg mx-auto">  </div>
                     

            </div>
            
        </div>
    </footer>
</template>

<script>
export default {
    data: function(){
        return {
            dcComicsLinks: [
                {
                    text: 'Characters',
                    url: '#',
                },
                {
                    text: 'Comics',
                    url: '#',
                },
                {
                    text: 'Movies',
                    url: '#',
                },
                {
                    text: 'Tv',
                    url: '#',
                },
                {
                    text: 'Games',
                    url: '#',
                },
                {
                    text: 'Collectibles',
                    url: '#',
                },
                {
                    text: 'Videos',
                    url: '#',
                },
                {
                    text: 'Fans',
                    url: '#',
                },
                {
                    text: 'News',
                    url: '#',
                },
                {
                    text: 'Shop',
                    url: '#',
                }
            ],
            shopLinks: [
                {
                    text: 'Shop DC',
                    url: '#',
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#',
                }
            ],
            dcLinks: [
                {
                    text: 'Term of Use',
                    url: '#',
                },
                {
                    text: 'Privacy policy (New)',
                    url: '#',
                },
                {
                    text: 'Ad Choices',
                    url: '#',
                },
                {
                    text: 'Advertising',
                    url: '#',
                },
                {
                    text: 'Jobs',
                    url: '#',
                },
                {
                    text: 'Subscriptions',
                    url: '#',
                },
                {
                    text: 'Talent Workshop',
                    url: '#',
                },
                {
                    text: 'CPSC Certificates',
                    url: '#',
                },
                {
                    text: 'Ratings',
                    url: '#',
                },
                {
                    text: 'Shop Help',
                    url: '#',
                },
                {
                    text: 'Contact Us',
                    url: '#',

                }
            ],
            sitesLinks: [
                {
                    text: 'DC',
                    url: '#',
                },{
                    text: 'MAD Magazine',
                    url: '#',
                },
                {
                    text: 'DC Kids',
                    url: '#',
                },
                {
                    text: 'DC Universe',
                    url: '#',
                },
                {
                    text: 'DC Power Visa',
                    url: '#',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../styles/style.scss";

footer{

    height: 17rem;
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size:cover;

    
        
}

.footer-content{
    width: 80%;
    margin: 0 auto;

    
    h4{
        text-transform: uppercase;
        color:white;
        font-size: 1rem;
        font-weight: 600;
    }
    ul{
        padding: 0.6rem 0;
        li{
            font-size: .6rem;
            a{
                color: #b4b4b4;
            }
        }
    }

    .footer-bg{
            width: 40%;
            object-fit: cover;
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
        }


}

</style>