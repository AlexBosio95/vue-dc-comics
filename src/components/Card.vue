<template>

  <div class="ms_card">
      <img :src="card.thumb" :alt="card.series">
      <h5 class="fs-6 mt-3">{{card.series}}</h5>
  </div>

</template>

<script>
export default {

    props:{
        card: Object,
    },

}
</script>

<style lang="scss" scoped>
@import "../styles/variabiles.scss";

div.ms_card{
    width: calc(100% / 6 - 1rem);
    margin: 2rem 0.5rem;
    cursor: pointer;

    img{
        width: 100%;
        height: 200px;
        object-fit: cover;
        object-position: top;

        &:hover{
            transform: scale(1.05);
            transition: 0.5s;
        }
    }


    h5{
        margin: 0 0.2rem;
        color: $textColor;
        text-transform: uppercase;
    }
}

</style>