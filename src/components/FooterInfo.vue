<template>
  <div class="ms_container">
    <div class="container">
      <div class="row row-cols-2">
            <div class="col">
              <button>SIGN-UP NOW!</button>
            </div>

            <div class="col social-link align-items-center">
              <div class="ps-4">
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-twitter.png" alt="">
                <img src="../assets/img/footer-youtube.png" alt="">
                <img src="../assets/img/footer-pinterest.png" alt="">
                <img src="../assets/img/footer-periscope.png" alt="">
              </div>

              <h5 class="fw-bold m-0">Follow Us</h5>

            </div>
      </div>
    </div>
   
      
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../styles/variabiles.scss";

div .ms_container{
    background-color: $footerColor;

    .container{
        padding: 2.5rem 0rem;
    }

    button{
      background-color: $footerColor;
      padding: 1rem;
      color: $textColor;
      border: 1.5px solid $colorPrimary;
    }
}

.social-link{
  display: flex;
  flex-direction: row-reverse;
  align-items: center;

  h5{
    text-transform: uppercase;
    color: $colorPrimary;
  }

  img{
    margin: 0px 5px;
  }
}


</style>