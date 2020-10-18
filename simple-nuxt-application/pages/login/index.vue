<template>
    <section>
        <h1>login page</h1>
        <input type="text" v-model="email">

        <button @click="onLogin">Login</button>
    </section>
</template>
<script>
export default {
    data() {
        return {
            email: '',
        }
    },
    methods: {
        onLogin() {
            this.$router.push('/login/' + this.email)
        }
    }

}
</script>