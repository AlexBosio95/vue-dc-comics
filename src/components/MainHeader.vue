<template>
<div class="container">
    <div class="row">
        <div class="col">
            <img src="../assets/img/dc-logo.png" alt="dc logo">
        </div>
        <div class="col">
            <ul>
                <li v-for="(items, index) in navList" :key="index">{{items.text}}</li>
            </ul>

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
                    active: false
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

<style>


</style>