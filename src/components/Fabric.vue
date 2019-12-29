<template>
    <div class="demo">
        <h1>{{ msg }}</h1>
        <canvas id="canvas" :width=width :height=height></canvas>
    </div>
</template>

<script>
    import fabric from "fabric";
    const Fabric = fabric.fabric;
    export default {
        name: 'HelloWorld',
        props: {
            msg: String,
            width: {
                type: Number,
                required: true
            },
            height: {
                type: Number,
                required: true
            }
        },
        mounted() {
            window.console.log(Fabric);
            this.canvas = new Fabric.Canvas('canvas', {preserveObjectStacking: true});
            this.canvas.loadFromJSON('{"objects":[{"type":"rect","left":50,"top":50,"width":20,"height":20,"fill":"green","overlayFill":null,"stroke":null,"strokeWidth":1,"strokeDashArray":null,"scaleX":1,"scaleY":1,"angle":0,"flipX":false,"flipY":false,"opacity":1,"selectable":true,"hasControls":true,"hasBorders":true,"hasRotatingPoint":false,"transparentCorners":true,"perPixelTargetFind":false,"rx":0,"ry":0},{"type":"circle","left":100,"top":100,"width":100,"height":100,"fill":"red","overlayFill":null,"stroke":null,"strokeWidth":1,"strokeDashArray":null,"scaleX":1,"scaleY":1,"angle":0,"flipX":false,"flipY":false,"opacity":1,"selectable":true,"hasControls":true,"hasBorders":true,"hasRotatingPoint":false,"transparentCorners":true,"perPixelTargetFind":false,"radius":50}],"background":"rgba(0, 0, 0, 0)"}');
        }
    }
</script>
<style>
    canvas{
        border: aquamarine 2px dashed;
    }
</style>
