<template>
    <div class="card">
        <div id="toast">
            <Achievement :num="number"/>
        </div>
        <div id="slide">
            <slot></slot>
        </div>
    </div>
</template>

<script>
    import Achievement from './Achievement.vue'

    export default {
        data: () => ({
            show: false,
        }),
        components: {
            Achievement
        },
        props: {
            title: String,
            number: Number
        }
    }
</script>

<style>
    .card {
        position: relative;
        overflow: hidden;
        width: 375px;
        height: 580px;
        border-radius: 20px;
    }
    #slide {
        position: absolute;
        left: -100%;
        transition: 1s;
    }
    .card:hover #slide {
        transition: 1s;
        left: 0;
    }
    .card:hover #toast {
        display: block;
    }
    #toast {
        display: none;
    }
</style>
