<template>

    <div class="wrapper">
        <div class="inner">
            <div class="title">Black Friday Sale | Get upto 70% off on all your favorate products</div>
          
            <div class="img">  <img class="image" src='~/assets/halfCamp.jpg' >   
               </div>
                <!-- <div class="description">   
                    <div class="text"> Buy this very good product</div>
                    <div class="priceBar">  <div class="price"> $290</div>  <div class="counter">  - 0 + </div></div>
                </div> -->
                
          
        </div>
    
    
    </div>
    
    </template>
    <script setup>
   import ('https://fonts.googleapis.com/css2?family=Bungee&family=Phudu&family=Poppins:wght@300&family=Salsa&display=swap')

    
    </script>
    
    
    <style scoped>
    
    .wrapper{
        /* border: 1px solid black; */
        height: auto;
        width: 45rem;
        box-sizing: border-box;
        font-family: 'poppins';
        background-color:  #DCDCDC;
        padding: 0.4rem;
        border-radius: 5px;
    }
    
    
    .inner{
        display: flex;
       
        justify-content: center;
        align-items: center;
    }
    .image{
        height: 20rem;
        border-radius: 5px;
        
    }
    
    .description{
        padding: 0.5rem;
        text-align: left;
    }
    .title{
        /* padding: 0.5rem; */
        font-size: 45px;
        font-weight: 700;
        text-align: left;
        width: 25vw;
        font-family: 'poppins'
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