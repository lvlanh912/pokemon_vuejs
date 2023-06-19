<template>
        <div class="card" :style="`width:${_width}px;height:${_height}px`">
            <div class="card-inner">
                <div class="card_face"></div>

            </div>
    </div>
</template>

<script>
export default {
  props: {
   _width:{
    type:Number
   },
   _height:{
    type:Number
   }
  },
    data(){
        return{
           
        }
    }
        
}
</script>

<style scoped>
.card-inner{
    width: 100%;
    height: 100%;
    transition: transform 1s;
    transform-style: preserve-3d;
    cursor: pointer;
    position: relative;
}
.card_face{
    position: absolute;
    width: 100%;
    height: 100%;
    -webkit-backface-visibility: hidden;
    backface-visibility: hidden;
    overflow: hidden;
    border-radius: 1rem;
    padding: 1rem;
    box-shadow: 0 3px 18px 3px rgba(0,0,0,.2);
}
</style>