<template>

    <div class="wrapper">
        <div class="inner">
            <div class="titleWrap">
                <div class="title">Black Friday Sale | Get upto 70% off on all your favorate products</div>
            <div class="spaan">
                Extra 5% on HDFC Accounts
            </div>
            </div> 
         
          
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
        
        width: auto;
        box-sizing: border-box;
        font-family: 'poppins';
        background-color:  #DCDCDC;
        padding: 2rem;
        border-radius: 5px;
    }
    
    
    .titleWrap{
        /* padding: 2rem; */
        display: flex;
        flex-direction: column;
        gap: 1rem;  
    }
    .inner{
        display: flex;
        margin-left: auto;
        margin-right: auto;
        justify-content: space-around;
        align-items: center;
    }
    .image{
        height: 20rem;
        border-radius: 5px;
        
    }

    .spaan{
        margin-top: 1rem;
        padding:  0.5rem;
        border-radius: 4px;
        background-color: white;
        width: fit-content;
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
        width: auto; 
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



<!-- penia -->

// nuxt.config.js
export default defineNuxtConfig({
  modules: [
    '@pinia/nuxt',
  ],
});


// store/cart.js
<!-- import { defineStore } from 'pinia';

export const useCartStore = defineStore('cart', {
  state: () => ({
    items: [],
    totalQuantity: 0,
    totalPrice: 0,
  }),

  actions: {
    // Add a product to the cart
    async addProduct(product) {
      // Check for existing item
      const existingItem = this.items.find((item) => item.id === product.id);

      if (existingItem) {
        existingItem.quantity++;
      } else {
        this.items.push({
          id: product.id,
          name: product.name,
          price: product.price,
          quantity: 1,
          image: product.image, // Assuming a product image property
        });
      }

      this.updateTotals();
    },

    // Remove a product from the cart
    async removeProduct(productId) {
      this.items = this.items.filter((item) => item.id !== productId);
      this.updateTotals();
    },

    // Update product quantity
    async updateQuantity(productId, quantity) {
      const productIndex = this.items.findIndex((item) => item.id === productId);
      this.items[productIndex].quantity = quantity;
      this.updateTotals();
    },

    // Clear the cart
    clearCart() {
      this.items = [];
      this.totalQuantity = 0;
      this.totalPrice = 0;
    },

    // Recalculate totals
    updateTotals() {
      this.totalQuantity = this.items.reduce((sum, item) => sum + item.quantity, 0);
      this.totalPrice = this.items.reduce((sum, item) => sum + item.price * item.quantity, 0);
    },
  },
});


<template>
    <div>
      <p>Total items: {{ cartStore.totalQuantity }}</p>
      <p>Total price: {{ cartStore.totalPrice }}</p>
    </div>
  </template>
  
  <script>
  import { useCartStore } from '~/stores/cart';
  
  export default {
    setup() {
      const cartStore = useCartStore();
  
      return {
        cartStore,
      };
    },
  };
  </script> -->