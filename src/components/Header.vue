<template>

<div class="container mt-3">
    <div class="row row-cols-2 align-items-center">
        <div class="col-3">
            <img src="../assets/img/dc-logo.png" alt="dc logo">
        </div>
        <div class="col-9">
            <nav>
                <ul class="d-flex justify-content-end m-0">
                    <li @click="changeActive(index)" class="mb-0 fw-semibold" 
                    :class="{'active' : item.active}" 
                    v-for="(item, index) in navList" :key="index">
                        {{item.text}}  
                        <div v-if="(item.active)" class="nav-mark"></div>
                    </li>
                   
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
    },
    methods: {
        changeActive: function(currentIndex) {

            for (let i = 0; i < this.navList.length; i++) {
                this.navList[i].active = false
            }

            if (!this.navList[currentIndex].active){
                this.navList[currentIndex].active = true
            }
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
        padding: 0;

            li{
                margin: 0.5rem;
                cursor: pointer;
                position: relative;
            }

            .nav-mark{
                position: absolute;
                top: 57px;
                left: 0;
                height: 5px;
                width: 100%;
                background-color: $colorPrimary;

            }

    }

    .active{
        color: $colorPrimary;
    }

</style>