<template>
    <nav>
        <div class="logo">
            <img src="../assets/logo.png" alt="logo">
            <p>Brands.io</p>
        </div>

        <div class="headers">
            <p>Home</p>
            <p>About Us</p>
            <p>Services</p>
            <p>Contact Us</p>
        </div>

        <div>
            <button>Login</button>
        </div>
    </nav>
</template>



<style scoped lang="scss">

nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    margin-top: 20px;
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

    p {
        font-weight: 500;
        font-size: 14px;
        cursor: pointer;

        &:first-child {
            background: linear-gradient(89.97deg, #AE67FA 1.84%, #F49867 102.67%), linear-gradient(106.23deg, #4EF0F0 0%, #05C580 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
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

</style>