<template>
    <Title title="site building..." :fullfilled="true" />
</template>

<script lang="ts">
import { defineComponent } from "vue"
import Title from "./components/Title.vue"

export default defineComponent({
    name: "App",
    components: { Title },
})
</script>

<style lang="less">
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}
</style>
