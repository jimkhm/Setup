<template>
    <div>
        <input type="text" v-model="pid">
        <button @click="onLoadProduct">Product</button>
    </div>
    
</template>
<script>
export default {
    data() {
        return {
                pid: ''
        }
    },

    methods: {
        onLoadProduct() {
            this.$router.push('/products/' + this.pid);
        }
    }
}
</script>