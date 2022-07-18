<template>
    <footer>
        <div class="footer-content">
            <div class="footer-content-items d-flex ">
                <div class="col-1">
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

                <div class="col-1">
                    <h4>Dc</h4>
                    <ul>
                        <li v-for="(link, index) in dcLinks" :key="index">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>
                </div>
                <div class="col-1">
                    <h4>Sites</h4>
                    <ul>
                        <li v-for="(link, index) in sitesLinks" :key="index">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>

                    
                </div>

                <div class="footer-bg">
           
                </div>

                
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
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Tv',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                }
            ],
            shopLinks: [
                {
                    text: 'Shop DC',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#',
                    current: false,
                }
            ],
            dcLinks: [
                {
                    text: 'Term of Use',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Privacy policy (New)',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Ad Choices',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Advertising',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Jobs',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Subscriptions',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Talent Workshop',
                    url: '#',
                    current: false,
                },
                {
                    text: 'CPSC Certificates',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Ratings',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop Help',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Contact Us',
                    url: '#',
                    current: false,
                }
            ],
            sitesLinks: [
                {
                    text: 'DC',
                    url: '#',
                    current: false,
                },{
                    text: 'MAD Magazine',
                    url: '#',
                    current: false,
                },
                {
                    text: 'DC Kids',
                    url: '#',
                    current: false,
                },
                {
                    text: 'DC Universe',
                    url: '#',
                    current: false,
                },
                {
                    text: 'DC Power Visa',
                    url: '#',
                    current: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../styles/style.scss";

footer{

    height: 25rem;
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size:cover;

    
        .footer-bg{
            width: 40%;
            object-fit: cover;
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
        }
}

.footer-content{
    width: 80%;
    margin: 0 auto;

    
    h4{
        text-transform: uppercase;
    }
    ul{
        padding: 1rem 0;
        li{
            font-size: .6rem;
            a{
                color: #b4b4b4;
            }
        }
    }
    
}

</style>