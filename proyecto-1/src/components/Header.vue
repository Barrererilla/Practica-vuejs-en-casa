<template>
    <header class="head">
        <img src="@/assets/paisaje-azul.svg" alt="Logo" @click="load" >
        <h1><span>Cash</span>Flow</h1>
        <span></span>
    </header>
</template>

<script>
export default{
    methods: {
        load(){
            location.reload();
        }
    }
}

</script>

<style scoped>
header{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}
.head h1 {
    color: var(--brand-blue);
    font-size: 25px;
}
img,
span{
    width: 38px;
}
.head h1 span {
    color: var(--brand-green);
}
</style>