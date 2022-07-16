<template>
  <div class="ms_container">
      <div class="container">
          <div class="row row-cols-3">
              <div class="col-5 my-5">
                  <!-- Link -->
                  <div class="row row-cols-3">
                      <div class="col">
                            <h4 class="fw-bold">Dc Comics</h4>
                            <ul class="p-0 mt-4">
                                <li v-for="(link, index) in dcComicList" :key="index">{{link.text}}</li>
                            </ul>

                            <h4 class="fw-bold mt-4">Shop</h4>
                            <ul class="p-0 mt-4">
                                <li v-for="(link, index) in shopList" :key="index">{{link.text}}</li>
                            </ul>
                      </div>

                      <div class="col">
                            <h4 class="fw-bold">Dc</h4>
                            <ul class="p-0 mt-4">
                                <li v-for="(link, index) in utilityList" :key="index">{{link.text}}</li>
                            </ul>
                      </div>

                      <div class="col">
                            <h4 class="fw-bold">Sites</h4>
                            <ul class="p-0 mt-4">
                                <li v-for="(link, index) in siteLink" :key="index">{{link.text}}</li>
                            </ul>
                      </div>
                  </div>
              </div>

              <div class="col-2"></div>

              <div class="col-5 image">

              </div>
          </div>
      </div>

  </div>
</template>

<script>

export default {
    data: function(){
        return{
            dcComicList: [
                {
                    text: 'Characters',
                    url: '#'
                },
                {
                    text: 'Comics',
                    url: '#'
                },
                {
                    text: 'Movies',
                    url: '#'
                },
                {
                    text: 'Tv',
                    url: '#'
                },
                {
                    text: 'Games',
                    url: '#'
                },
                {
                    text: 'Videos',
                    url: '#'
                },
                {
                    text: 'News',
                    url: '#'
                }
            ],

            shopList: [
                {
                    text: 'Shop DC',
                    url: '#'
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#'
                }
            ],

            utilityList: [
                {
                    text: 'Terms Of Use',
                    url: '#'
                },
                {
                    text: 'Privacy policy (New)',
                    url: '#'
                },
                {
                    text: 'Ad Chalene',
                    url: '#'
                },
                {
                    text: 'Advertising',
                    url: '#'
                },
                {
                    text: 'Jobs',
                    url: '#'
                },
                {
                    text: 'Subscriptions',
                    url: '#'
                },
                {
                    text: 'Talent Workshone',
                    url: '#'
                },
                {
                    text: 'CPSC Certificates',
                    url: '#'
                },
                {
                    text: 'Ratinas',
                    url: '#'
                },
                {
                    text: 'Shop Help',
                    url: '#'
                },
                {
                    text: 'Contact Us',
                    url: '#'
                }
            ],

            siteLink: [

                {
                    text: 'DC',
                    url: '#'
                },
                {
                    text: 'MAD Magazine',
                    url: '#'
                },
                {
                    text: 'DC Kids',
                    url: '#'
                },
                {
                    text: 'DC Universe',
                    url: '#'
                },
                {
                    text: 'DC Power Visa',
                    url: '#'
                }
            ]


        }
    }

}
</script>

<style lang="scss" scoped>
@import "../styles/variabiles.scss";

.col ul{
    padding: 0;
    list-style-type: none;

    li{
        color: $colorLink;
        margin: 10px 0px;
        cursor: pointer;

        &:hover{
        color: $textColor;
    }
    }

    
}

h4{
        text-transform: uppercase;
        color: $textColor;
    }

div .ms_container{
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
}

.image {
    background-image: url('../assets/img/dc-logo-bg.png');
    overflow: hidden;
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

</style>