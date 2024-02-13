<template>
    <div class="home">
        <header id="header">
            <div class="container">
                <div class="cart">
                    <p><i class="fas fa-shopping-cart"></i>{{ cart.length }}</p>
                </div>
            </div>
        </header>
        <ProductView :member="member" @addtocart="updatecart" />
        <!-- <ProductView/> -->
    </div>
</template>

<script>
// @ is an alias to /src
import ProductView from "@/components/ProductView.vue";

export default {
    name: "HomeView",
    components: {
        ProductView,
    },
    data() {
        return {
            member: false,
            cart: [],
        };
    },
    methods: {
        updatecart(id) {
            this.cart.push(id);
        },
    },
};
</script>
