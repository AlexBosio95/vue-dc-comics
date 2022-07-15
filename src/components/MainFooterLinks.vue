<template>
  <div class="ms_container">
      <div class="container">
          <div class="row row-cols-2">
              <div class="col my-5">
                  <div class="row row-cols-3">
                      <div class="col">
                          <div>
                            <h4 class="fw-bold">Dc Comics</h4>
                            <ul>
                                <li v-for="(link, index) in DcComicList" :key="index">{{link.text}}</li>
                            </ul>
                          </div>
                      </div>
                  </div>
                  
              </div>
              <div class="col image">
              </div>
          </div>
      </div>

  </div>
</template>

<script>

export default {
    data: function(){
        return{
            DcComicList: [
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
            ]

        }
    }

}
</script>

<style lang="scss" scoped>
@import "../styles/variabiles.scss";

.col ul{

    list-style: none;

    li{
        color: $colorLink;
        margin: 10px 0px;
    }
}

h4{
        text-transform: uppercase;
        color: $textColor;
    }

div .ms_container{
    background-image: url('../assets/img/footer-bg.jpg');
    height: 40rem;
}

.image {
    background-image: url('../assets/img/dc-logo-bg.png');
    overflow: hidden;
    height: 100%;
}

</style>