<template>

  <div class="ms_container">
      <div class="container d-flex">
          <div class="products" v-for="(product, index) in productsList" :key="index">
              <img :src="'../assets/img/' + product.imageUrl" alt="">
              <h4 class="fw-bold">{{product.text}}</h4>
          </div>

      </div>
  </div>

</template>

<script>
export default {
   data: function(){
        return{
            productsList: [
                {
                    imageUrl: "buy-comics-digital-comics.png",
                    url: '#',
                    text: 'DIGITAL COMICS'
                },
                {
                    imageUrl: "buy-comics-merchandise.png",
                    url: '#',
                    text: 'DC MERCHANDISE'
                },
                {
                    imageUrl: "img/buy-comics-shop-locator.png",
                    url: '#',
                    text: 'SUBSCRIPTION'
                },
                {
                    imageUrl: "img/buy-comics-subscriptions.png",
                    url: '#',
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    imageUrl: "img/buy-comics-subscriptions.png",
                    url: '#',
                    text: 'DC POWER VISA'
                },

            ],
            indexActive: 0,

        }
    },
    methods: {
        log: function(index){
            console.log(index)
        }

    }
    

}
</script>

<style lang="scss" scoped>
@import "../styles/variabiles.scss";

img{
    height: 3rem;
}

div .ms_container{
    background-color: $colorPrimary;
    

    .container{
        height: 10rem;
    }

    h4{
        color: $textColor;
    }
}

</style>