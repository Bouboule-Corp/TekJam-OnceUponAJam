<template>
    <div class="card">
        <div id="slide">
            <slot></slot>
        </div>
    </div>
</template>

<script>
  export default {
    data: () => ({
        show: false,
    }),
    props: {
        title: String
    }
  }
</script>

<style>
    .card {
        position: relative;
        overflow: hidden;
        width: 30vw;
        height: 100vh;
        border-radius: 20px;
    }

    #slide {
        position: absolute;
        left: -90%;
        transition: 1s;
    }

    .card:hover #slide {
        transition: 1s;
        left: 0;
    }
</style>
