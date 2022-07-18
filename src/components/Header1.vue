<template>
  <header>
     <nav class="navbar">
        <img src="../assets/img/dc-logo.png" class="logo-header">

        <ul>
            <li class="text-center" v-for="(item, index) in headerItems" :key="index" :class="{ active: item.current}">
                <a :href="item.url">{{item.text}}</a>
            </li>

        </ul>

    </nav>

    
  </header>
 
</template>

<script>

export default {
    data: function(){
        return {
            headerItems: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
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
                },
            ]
        }
    }    

}

</script>

<style lang="scss" scoped>

@import "../styles/style.scss";



header{
    @include my-container;
    @include d-flex(space-between, center);
    height: 88px;

  

    .navbar{

        @include box;

        .logo-header{
            width:60px;
           
        }
        
        height: 100%;
        ul{
            height: 100%;
            @include d-flex(center, '');
            li{
                padding-left: 1rem;
                padding-right: 1rem;
                height: 80px;
                display:inline-block;
           
                @include d-flex('', center);
                border-bottom: 4px solid transparent;
                &.active,
                &:hover{
                    border-bottom: 4px solid $secondaryColor;
                }
                a{
                    color: $fontColor;
                    text-transform: uppercase;
                    font-size: .8rem;
                    font-weight: 600;
                    text-align: center;
                }
            }
        }
    }
}


</style>