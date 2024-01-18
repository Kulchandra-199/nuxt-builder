<template>

<div class="wrapper">
    <div class="inner">
        <div class="title">Cotton Shirt </div> 
        <div class="img">  <img class="image" src='~/assets/shirt.webp' >   </div>
            <div class="description">   
                <div class="text"> Buy this very good product</div>
                <div class="priceBar">  <div class="price"> $290</div>  <div class="counter">  - 0 + </div></div>
            </div>
      
    </div>


</div>

</template>
<script setup>
import ('https://fonts.googleapis.com/css2?family=Bungee&family=Phudu&family=Poppins:wght@300&family=Salsa&display=swap')


</script>


<style scoped>

.wrapper{
    border: 1px solid black;
    height: auto;
    max-width: 15rem;
    box-sizing: border-box;
    font-family: 'poppins';
}


.inner{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.image{
    height: 15rem;
    
}

.description{
    padding: 0.5rem;
}
.title{
    padding: 0.5rem;
    font-size: 25px;
    font-weight: 700;
}

.priceBar{
    display: flex ;
    justify-content: space-between;
    padding: 0.3rem;
}

.price{
    font-size: 20px;
}
.counter{
    border: 1px solid black;
    padding:  0.2rem 0.5rem;
    border-radius: 5px;
}

</style>