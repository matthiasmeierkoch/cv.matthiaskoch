<template>
    <div>
        <h1>hallo</h1>
        <nuxt-link to="/">Home</nuxt-link>
        <nuxt-link to="/Work/overview">work</nuxt-link>
    </div>
</template>

<script>
    export default {
        name: "hallo",
        mounted () {
            this.$nextTick(() => this.$sal())
        }
    }
</script>

<style scoped>

</style>