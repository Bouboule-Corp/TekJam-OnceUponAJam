<template>
    <div class="card">
        <div>
            <!-- <img v-bind:src="'../assets/' + {img}" /> -->
            <img :src="resolve_img_url(img)">
        </div>
    </div>
</template>

<script>
  export default {
    data: () => ({
        show: false,
    }),
    props: {
        img: String
    },
    methods: {
        resolve_img_url: function (path) {
            let images = require.context('../assets', false, /\.png$|\.jpg$/)
            return images("./"+path)
        }
    }
  }
</script>

<style>
    .card {
        background-color: black;
        border-radius: 20px;
        width: 40vw;
        height: 35vh;
    }
</style>
