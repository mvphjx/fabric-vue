<template>
    <div class="demo" :id="demo">
        <canvas id="canvas" :width="width" :height="height"></canvas>
    </div>
</template>

<script>

    export default {
        props: {
            width: {
                type: Number,
                required: true
            },
            height: {
                type: Number,
                required: true
            }
        },
        data() {
            return {
                canvas: null,
                currentObj: null
            };
        },
        mounted() {
            //this.canvas = fabric.Canvas('canvas', {preserveObjectStacking: true});
        }
    }
</script>
