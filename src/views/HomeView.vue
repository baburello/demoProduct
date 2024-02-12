<template>
    <div class="home">
        <ProductView msg="Welcome to my Vue.js App" />
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
};
</script>
