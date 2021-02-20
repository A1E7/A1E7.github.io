<template>
    <div class="a1e7-title" :class="{ 'a1e7-title--fullfilled': fullfilled }">
        <h1 class="a1e7-title__Title a1e7-title__Title--background">
            {{ title }}
        </h1>
    </div>
</template>

<style lang="less" scoped>
.a1e7-title {
    height: 200px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-position: top;
    background-image: url(../assets/title-background.jpg);
    &--fullfilled {
        height: 100vh;
    }
    &__Title {
        color: white;
        padding: 10px 20px;
        &--background {
            background-color: rgba(0, 0, 0, 0.75);
        }
    }
}
</style>

<script lang="ts">
import { defineComponent } from "vue"

export default defineComponent({
    name: "Title",
    props: {
        title: {
            type: String,
            required: true,
        },
        fullfilled: {
            type: Boolean,
            default: false,
        },
    },
})
</script>
