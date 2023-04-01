<template>
    <div>
        <!-- <img :src="j" alt="image">
        <h2> {{ headerText }} </h2>
        <p> {{ paragText }} </p> -->
    </div>
</template>


<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    props: ["img", "headerText", "paragText"],
    setup(prop) {
        console.log(prop.headerText, prop.paragText)
    }
})

</script>


<style scoped lang="scss">

</style>