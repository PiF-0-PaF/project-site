<template>
    <div class="Kartocka_item">
        <img class="Kartochka_item__image" :src=" require('../assets/images/' + product_data.image)" alt="">
        <p class="Kartochka_item__name">{{product_data.name}}</p>        
        <p>{{product_data.opis1}}</p>
        <p>{{product_data.opis2}}</p>
        <p>{{product_data.opis3}}</p>
        <p>{{product_data.opis4}}</p>
        <p>{{product_data.opis5}}</p>
        <p>{{product_data.opis6}}</p>
        <p class="Kartochka_item__price">Цена: {{product_data.price}} Руб.</p>
        <button 
        class="Kartochka_item__add_to_cart_btn" 
        @click="addToCart">Добавить в корзину
        </button>
    </div>
</template>

<script>
    export default{
        name: "Kartocka_item",
        props: {
            product_data: {
                type: Object,
                default() {
                    return {}
                }
            }
        },
        data() {
            return {}
        },
        computed: {},
        methods: {
            addToCart() {
                this.$emit('addToCart', this.product_data)
            }
        },
        mounted() {},
    }
</script>

<style>
    .Kartochka_item{
        flex-basis: 25%;        
        padding: 20px;
        margin-bottom: 20px;
        box-shadow: 0 0 8px 0 #000000;
    }
    .Kartochka_item__image{
        width: 200px;
    }
    .Kartochka_item__add_to_cart_btn{
        /* background: linear-gradient(85deg, #fb63f9, #c2e534);
        border-radius: 10px;
        border: 0px;
        height: 15px;
        width: 50px; */
        border: none;
        font-family: cursive;
        font-size: inherit;
        color: #fff;
        background:#34495e;
        cursor: pointer;
        padding: 20px 50px;
        display: inline-block;
        margin: 15px 30px;
        text-transform: uppercase;
        letter-spacing: 1px;
        font-weight: 700;
        outline: none;
        position: relative;
        -webkit-transition: all 0.3s;
        -moz-transition: all 0.3s;
        transition: all 0.3s;
    }
    .Kartochka_item__add_to_cart_btn:hover {
        background: #2c3e50;
    } 
    
</style>