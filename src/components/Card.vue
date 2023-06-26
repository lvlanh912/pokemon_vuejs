<template>
        <div class="card" :style="`width:${_width}px;height:${_height}px`">
            <div class="card-inner ">
                <div class="card_face card--front ">
                <div class="card-content" style="background-size: 100% 75%;"></div>
                </div>
                <div class="card_face card--back">
                    <div class="card-content" :style="`background: url(src/assets/images/${_image}.png);`"></div>
                </div>

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
   },
   _image:{
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
.card-content{
    width: 100%;
    height: 100%;
    background: url(../assets/images/icon_back.png);
    background-repeat: no-repeat;
    box-sizing: border-box;
    background-position: center;
    background-size: 100% 75%!important;
}
.card--back .card-content{
    background-position: center !important;;
    background-repeat: no-repeat!important;
    background-size: contain;
    height: 100%;
    width: 100%;
    transform: rotateY(180deg);
}
.flipped{
    transform: rotateY(180deg);
}
</style>