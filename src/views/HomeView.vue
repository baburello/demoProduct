<template>
    <div class="home">
        <ProductView :member="member" />
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
        };
    },
};
</script>
