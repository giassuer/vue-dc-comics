<template>
    <div class="foter-top-container">
        <div class="foter-top-menu">
            <div v-for="(element, index) in footerTopContent" :key="index" class="footer-top-contant">
                <div class="footer-top-img"><img :src="'../assets/img/buy-comics-' + element.url + '.png'" alt=""><span class="footer-top-text">{{element.text}}</span></div>
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
                    url: 'digital-comics',
                },
                {
                    text: 'DC MERCHANDISE',
                    url: 'merchandise',
                },
                {
                    text: 'SUBSCRIPTION',
                    url: 'subscriptions',
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    url: 'shop-locator',
                },
                {
                    text: 'DC POWER VISA',
                    url: 'shop-locator',
                },
                {
                    text: 'COLLECTIBLES',
                    url: 'shop-locator',
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