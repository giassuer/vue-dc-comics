<template>
    <div class="foter-top-container">
        <div class="foter-top-menu">
            <div v-for="(element, index) in footerTopContent" :key="index" class="footer-top-contant">
                <div class="footer-top-img"><img :src="element.url" alt=""><span class="footer-top-text">{{element.text}}</span></div>
            </div>
            
        </div>
    </div>
</template>

<script>
export default {
  name: "FooterTop",

  data: function() {
        return {
            footerTopContent: [
                {
                    text: 'DIGITAL COMICS',
                    url: '../assets/img/buy-comics-digital-comics.png',
                },
                {
                    text: 'DC MERCHANDISE',
                    url: '../assets/img/buy-buy-comics-merchandise.png',
                },
                {
                    text: 'SUBSCRIPTION',
                    url: '../assets/img/buy-comics-subscriptions.png',
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    url: '../assets/img/buy-comics-shop-locator.png',
                },
                {
                    text: 'DC POWER VISA',
                    url: '../assets/img/buy-comics-shop-locator.png',
                },
                {
                    text: 'COLLECTIBLES',
                    url: '../assets/img/buy-comics-shop-locator.png',
                },
               
            ],
        };
    }

};
</script>

<style scoped leng="scss">

.foter-top-container{
    background-color: #0282f9;
}

.foter-top-menu{
    display: flex;
    justify-content: center;
    height: 150px;
}

.footer-top-contant{
    display: flex;
    align-items: center;
}

.footer-top-img{
    display: flex;
    align-items: center;
}

.footer-top-contant img{
    width: 30%;
}

.footer-top-text{
    font-size: 12px;
    text-align: left;
}

</style>