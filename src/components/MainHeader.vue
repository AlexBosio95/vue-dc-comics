<template>

<div class="container">
    <div class="row row-cols-2 align-items-center">
        <div class="col-3">
            <img src="../assets/img/dc-logo.png" alt="dc logo">
        </div>
        <div class="col-9">
            <nav>
                <ul class="d-flex justify-content-end">
                    <li :class="{'active' : items.active}" v-for="(items, index) in navList" :key="index">{{items.text}}</li>
                </ul>
            </nav>
        </div>

    </div>
</div>
  
</template>

<script>
export default {
    data: function(){
        return{
            navList: [
                {
                    text: "CHARACTERS",
                    url: '#',
                    active: false
                },
                {
                    text: "COMICS",
                    url: '#',
                    active: true
                },
                {
                    text: "MOVIES",
                    url: '#',
                    active: false
                },
                {
                    text: "TV",
                    url: '#',
                    active: false
                },
                {
                    text: "GAMES",
                    url: '#',
                    active: false
                },
                {
                    text: "COLLECTIBLES",
                    url: '#',
                    active: false
                },
                {
                    text: "VIDEOS",
                    url: '#',
                    active: false
                },
                {
                    text: "FANS",
                    url: '#',
                    active: false
                },
                {
                    text: "NEWS",
                    url: '#',
                    active: false
                },
                {
                    text: "SHOP",
                    url: '#',
                    active: false
                },

            ]
        }
    }

}
</script>

<style lang="scss" scoped>

@import "../styles/variabiles.scss";

    img{
        height: 4.1rem;
    }

    ul{
        list-style: none;

            li{
                margin: 0.5rem;
            }

    }

    .active{
        color: $colorPrimary;
    }

</style>