<template>
  <div class="ms_container mt-4">
      <div class="container d-flex align-items-center">
        <h1>Content goes here</h1>
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
    background-color: $standardBg;
    

    .container{
        height: 7rem;
    }

    h1{
        color: $textColor;
    }
}

</style>