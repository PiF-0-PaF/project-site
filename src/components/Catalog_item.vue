<template>
    <div class="Catalog_item">
        <p>Каталог товаров</p>
        <div class="kartochki">
            <Kartochka_item class="solo_kartochka"
            v-for="product in PRODUCTS"
            :key="product.id"
            :product_data="product"
            @addToCart="addToCart"
            />
        </div>
    </div>
</template>

<script>

import Kartochka_item from './Kartochka_item.vue';
import { mapActions, mapGetters } from 'vuex'
    export default {
        name: "Catalog_item",
        components: {
            Kartochka_item
        },
        data() {
            return{
                
            }
        },
        computed: {
            ...mapGetters([
                'PRODUCTS'
            ]),
        },
        methods: {
            ...mapActions([
                'GET_PRODUCTS_FROM_API',
                'ADD_TO_CART'
            ]),
            addToCart(data){
               this.ADD_TO_CART(data)
            }
        },
        mounted() {
          this.GET_PRODUCTS_FROM_API()
          .then((responce) => {
            if (responce.data) {
                console.log('Data arrived!')
            }
          })  
        }
    }
</script>

<style>
     .Catalog_item{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        align-items: center;
        font-size: 20px;
        font-weight: 600;
        color: black;
        font-family: cursive;
        flex-direction: row;
        align-content: center;
        padding: 20px;
        margin-bottom: 20px;
        box-shadow: 0 0 8px 0 #c0c0c0;
    } 
    .kartochki{
        display: flex;
        flex-wrap: wrap;
        align-content: center;
        justify-content: center;
        align-items: center;
        flex-direction: row;
        padding-left: 50px;
        padding-right: 50px;
    }
    .solo_kartochka{
        margin-left: 25px;
        margin-right: 25px;
        padding: 25px;
        margin-bottom: 25px;
        border: #e0e0e0 2px solid;
        box-shadow: 0 0 8px 0 #c0c0c0;
    }

</style>