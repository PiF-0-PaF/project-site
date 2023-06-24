<template>
    <div class="Korzina_item">
        <img class="Korzina_item__image" :src=" require('../assets/images/' + cart_item_data.image)">
        <div class="Korzina_item__info">
            <p>{{cart_item_data.name}}</p>
            <p>{{cart_item_data.price}} Руб.</p>
            <p>ID товара:{{cart_item_data.id}}</p>
        </div>
        <div class="Korzina_item__quantity">
            <p>Количество:</p>
        {{cart_item_data.quantity}}
        </div>
        <button class="button_korzina_item" @click="deleteFromCart">Удалить</button>
    </div>
</template>

<script>
    export default{
        name: "Korzina_item",
        props: {
            cart_item_data: {
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
            deleteFromCart() {
                this.$emit('deleteFromCart')
            }
        },
        mounted() {
           const cartItemData = this.cart_item_data
           cartItemData.quantity = 1; 
        },
    }
</script>

<style>
    .Korzina_item {
        display: flex;
        flex-wrap: nowrap;
        justify-content: space-between;
        align-items: center;
        box-shadow: 0 0 8px 0 #c0c0c0;
        margin-bottom: 25px;
    }
    .Korzina_item__image {
        max-width: 150px;
    }
    .button_korzina_item {
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
    .button_korzina_item:hover {
        background: #2c3e50;
    }
</style>