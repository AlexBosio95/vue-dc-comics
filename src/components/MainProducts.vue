<template>

  <div class="ms_container">
      <div class="container py-5 d-flex align-items-center">
          <div class="products d-flex m-2 align-items-center" v-for="(product, index) in productsList" :key="index">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="">
              <span class="fw-bold">{{product.text}}</span>
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
            ]

        }
    }

}
</script>

<style lang="scss" scoped>
@import "../styles/variabiles.scss";

img{
    height: 4rem;
    margin-right: 0.5rem;
}

.products{
    width: calc(100% / 5);
}


div .ms_container{
    background-color: $colorPrimary;
    

    span{
        color: $textColor;
    }
}

</style>