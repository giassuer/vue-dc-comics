<template>
    <div class="header-container">
        <div class="header-logo"><img src="../assets/img/dc-logo.png" alt=""></div>
        <div class="header-menu">
            <ul class="menu-list">
                <li v-for="(element, index) in links" :key="index">
                    <a href="">{{element.text}}</a>
                </li>
                
            </ul>
        </div>
    </div>
</template>

<script>
export default {
  name: "Header",

      data: function() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    current: false
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: false
                },
            ],
        };
    }

};
</script>

<style scoped leng="scss">

.header-container{
    width: 80%;
    height: 100px;
    margin: auto;
}

.header-logo{
    float: left;
    height: 100%;
    line-height: 100px;
    vertical-align: middle;
}

.header-logo img{
    height: 60px;
    vertical-align: middle;
}

.header-menu{  
    height: 100%;
    float: right;
}

.menu-list{
    display: flex;
    
}

li{
    line-height: 100px;
    margin: 0px 10px;
    font-size: 12px;
}

</style>
