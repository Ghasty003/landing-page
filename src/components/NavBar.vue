<template>
    <nav>
        <div class="logo">
            <img src="../assets/logo.png" alt="logo">
            <p>Brands.io</p>
        </div>

        <div ref="header" class="headers">
            <p>Home</p>
            <p>About Us</p>
            <p>Services</p>
            <p>Contact Us</p>

            <svg ref="close" class="close" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
            </svg>
        </div>

        <div>
            <button>Login</button>
        </div>

        <p ref="open" class="open">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
            </svg>
        </p>
    </nav>
</template>


<script setup lang="ts">
import { onMounted, ref } from "vue";


const open = ref<HTMLDivElement>(null!);
const close = ref<HTMLDivElement>(null!);
const header = ref<HTMLDivElement>(null!);


onMounted(() => {

    document.addEventListener("click", (e) => {
        if (!open.value.contains(e.target as Node) && !header.value.contains(e.target as Node)) {
            header.value.style.right = "-100%";
        }
    });

    open.value.addEventListener("click", () => {
        header.value.style.right = "0";
    });


    close.value.addEventListener("click", () => {
        header.value.style.right = "-100%";
    });

});

</script>



<style scoped lang="scss">

nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding-top: 20px;
}

.logo {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 15px;

    img {
        width: 30px;
        height: 34px;
    }

    p {
        color: #3E4581;
        font-weight: 700;
    }
}

.headers {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 60px;
    transition: all 1s;

    @media (max-width: 670px) {
        background: #E5E5E5;
        flex-direction: column;
        position: fixed;
        right: -100%;
        top: 0;
        height: 100%;
        gap: 90px;
        justify-content: center;
        width: 300px;
        z-index: 100000;
    }

    p {
        font-weight: 500;
        font-size: 14px;
        cursor: pointer;
        color: #3E4581;

        &:first-child {
            background: linear-gradient(89.97deg, #AE67FA 1.84%, #F49867 102.67%), linear-gradient(106.23deg, #4EF0F0 0%, #05C580 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        @media (max-width: 670px) {
            font-size: 20px;
        }
    }
}

button {
    background: linear-gradient(89.97deg, #AE67FA 1.84%, #F49867 102.67%), linear-gradient(106.23deg, #4EF0F0 0%, #05C580 100%);
    border-radius: 5px;
    border: none;
    width: 100px;
    height: 48px;
    color: white;
}

svg {
    width: 30px;
    cursor: pointer;
    display: none;

    @media (max-width: 670px) {
        display: block;
    }
}

.close {
    position: absolute;
    top: 20px;
    right: 20px;
}

</style>