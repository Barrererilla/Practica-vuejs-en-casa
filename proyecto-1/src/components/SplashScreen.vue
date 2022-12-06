<template>
    <div class="splashscreen">
        <img src="@/assets/paisaje-azul.svg" alt="logo" />
        <h2 class=""><span>Splash</span>Screen</h2>
    </div>
</template>

<script>
export default {
    name: 'SplashScreen', 
    components: {

    }
}
</script>

<style scoped>
.splashscreen{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    flex-direction: column;
}
div h1{
    color: var(--brand-blue)
}
div span {
    color: var(--brand-green)
}

</style>