<template>
    <div class="footer-container">
        <div class="footer-top">
            <div class="top-col-left">
                <div class="footer-menu-container">
                    <div class="col-left">
                        <div>
                            <h3>DC COMICS</h3>
                            <ul>
                                <li v-for="(element, index) in dcComics" :key="index">{{element.text}}</li>
                            </ul>
                        </div>
                        <div>
                            <h3>SHOP</h3>
                            <ul>
                                <li v-for="(element, index) in shop" :key="index">{{element.text}}</li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-center">
                        <div>
                            <h3>DC</h3>
                            <ul>
                                <li v-for="(element, index) in dc" :key="index">{{element.text}}</li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-right">
                        <div>
                            <h3>SITES</h3>
                            <ul>
                                <li v-for="(element, index) in sites" :key="index">{{element.text}}</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <div class="top-col-right"><img src="../assets/img/dc-logo-bg.png" alt=""></div>
        </div>
        <div class="footer-bottom-container">
            <div class="footer-bottom">
                <div class="bottom-col-left">
                    <div class="btn">SING-UP NOW!</div>
                </div>
                <div class="bottom-col-right">
                    <div>FOLLOW US</div>
                    <ul>
                        <li><a href=""><img src="../assets/img/footer-facebook.png" alt=""></a></li>
                        <li><a href=""><img src="../assets/img/footer-twitter.png" alt=""></a></li>
                        <li><a href=""><img src="../assets/img/footer-youtube.png" alt=""></a></li>
                        <li><a href=""><img src="../assets/img/footer-pinterest.png" alt=""></a></li>
                        <li><a href=""><img src="../assets/img/footer-periscope.png" alt=""></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: "Footer",

  data: function() {
        return {
            dcComics: [
                {
                    text: 'CHARACTERS',
                },
                {
                    text: 'COMICS',
                },
                {
                    text: 'MOVIES',
                },
                {
                    text: 'TV',
                },
                {
                    text: 'GAMES',
                },
                {
                    text: 'COLLECTIBLES',
                },
                {
                    text: 'VIDEOS',
                },
            ],

            dc: [
                {
                    text: 'CHARACTERS',
                },
                {
                    text: 'COMICS',
                },
                {
                    text: 'MOVIES',
                },
                {
                    text: 'TV',
                },
                {
                    text: 'GAMES',
                },
                {
                    text: 'COLLECTIBLES',
                },
                {
                    text: 'VIDEOS',
                },
                {
                    text: 'VIDEOS',
                },
                {
                    text: 'VIDEOS',
                },
                {
                    text: 'VIDEOS',
                },
                {
                    text: 'VIDEOS',
                },
            ],

            sites: [
                {
                    text: 'CHARACTERS',
                },
                {
                    text: 'COMICS',
                },
                {
                    text: 'MOVIES',
                },
                {
                    text: 'TV',
                },
                {
                    text: 'GAMES',
                },
            ],

            shop: [
                {
                    text: 'CHARACTERS',
                },
                {
                    text: 'COMICS',
                },
                
            ],
        };
    }

};
</script>

<style scoped leng="scss">

.footer-container{
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
}

.footer-top{
    width: 80%;
    margin: auto;
    display: flex;
    overflow: hidden;
}

.footer-top h3{
    color: white;
    padding: 10px 10px;
}

.footer-top img{
    width: 60%;
}

.footer-menu-container{
    display: flex;
}

.footer-menu-container li{
    color: #5d7b85;
    font-size: 10px;
    padding: 3px 5px;
}

.top-col-right{
    text-align: right;
}

.footer-bottom-container{
    background-color: #303030;
}

.footer-bottom{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 80%;
    margin: auto;
    padding: 20px 0px;
}

.btn{
    padding: 10px;
    border: 2px solid #0282f9;
    color: white;
}

.bottom-col-right{
    display: flex;
    align-items: center;
}

.bottom-col-right ul{
    display: flex;
}

.bottom-col-right li{
    margin: 0px 7px;
}

.bottom-col-right div{
    color: #0282f9;
    padding: 0px 7px;
}

</style>