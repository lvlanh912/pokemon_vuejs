<template>
  <h1 class="text-center">POKEMON MEMORIES by LVLANH</h1>
  <h3 class="text-center">Select mode to start game </h3>
  <div class="cointainer">
        <button class="btn-game">
            <span>4x4</span>
            <span>Easy</span>
        </button>
        <button class="btn-game">
            <span>6x6</span>
            <span>Medium</span>
        </button>
        <button class="btn-game">
            <span>8x8</span>
            <span>Hard</span>
        </button>
        <button class="btn-game">
            <span>10x10</span>
            <span>Super Hard</span>
        </button>
    </div>
</template>

<script>

export default {

}
</script>

<style>
h1{
    font-size: 4.5rem;
    text-transform: uppercase;
}
h3{
    font-size: 2rem;
}
.cointainer{
    display: flex;
    justify-content: center;
    align-content: center;
    text-align: center;
    margin-top: 2rem;
}

.text-center{
    text-align: center;
}
.btn-game{
    margin-right: 15px;
    box-sizing: border-box;
    height: 150px;
    width: 150px;
    box-shadow: none;
    border: 1px solid #fff;
    border-radius: 15%;
}
.btn-game:hover,.btn-game:hover span{
    background-color: #fff!important;
    color: black;
    transition: 0.5s;
}
.btn-game span{
    display: block;
    font-size: 2rem;
}
.btn-game span:last-child{
    display: block;
    font-size: 1.25rem;
    margin-top:.5rem ;
}
</style>