<template>
    <div class="Korzina_site">
        <h1>Ваша корзина</h1>
        <Korzina_item
            v-for="(item, index) in cart_data"
            :key="item.id"
            :cart_item_data="item"
            @deleteFromCart="deleteFromCart(index)"
        />
    </div>
</template>

<script>

import Korzina_item from './Korzina_item.vue'
import {mapActions} from 'vuex'

    export default{
        name: "Korzina_site",
        components: {
            Korzina_item
        },
        props: {
            cart_data: {
                type: Array,
                default() {
                    return []
                }
            }
        },
        data () {
            return {}
        },
        computed: {},
        methods: {
            ...mapActions([
                'DELETE_FROM_CART'
            ]),
            deleteFromCart(index) {
                this.DELETE_FROM_CART(index)
            }
        },
    }
</script>

<style>

</style>