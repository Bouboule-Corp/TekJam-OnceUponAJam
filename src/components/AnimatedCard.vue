<template>
    <div class="card">
        <div id="toast" @mouseover="play" @mouseleave="stop">
            <Achievement :num="number"/>
        </div>
        <div id="slide">
            <slot></slot>
        </div>
    </div>
</template>

<script>
    import Achievement from './Achievement.vue'
    import { useSound } from '@vueuse/sound'
    import sound from '../assets/advancement.mp3'

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
        },
        setup() {
            const { play, stop } = useSound(sound)

            return {
            play,
            stop,
            }
        },
    }
</script>

<style>
    .card {
        position: relative;
        overflow: hidden;
        width: 28vw;
        height: 90vh;
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
