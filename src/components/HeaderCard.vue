<template>
    <!-- <div class="header-card">
        <div>
            <img :src="img" alt="image">
        </div>

        <h2> {{ headerText }} </h2>
        <p> {{ paragText }} </p>
    </div> -->
    <img :src="img" alt="image">
</template>


<script setup lang="ts">

defineProps(["img"]);

</script>


<style scoped lang="scss">
// .header-card {
//     width: 282px;
//     height: 270px;
//     background: #FFFFFF;
//     // background: #000;
//     box-shadow: 0px 1.03704px 2.47917px rgba(0, 0, 0, 0.052963);
//     border-radius: 10px;

//     > div {
//         width: 60px;
//         height: 60px;
//         background: #ECEEFF;
//         border-radius: 50%;
//         // display: flex;
//         // justify-content: center;
//         // align-items: center;
//         // text-align: center;

//         > img {
//             width: 50px;
//             height: 50px;
//             background: #000;
//         }
//     }
// }
</style>