<template>
    <Layout>
        <template #head>
            <Header />
        </template>
    </Layout>
</template>


<script>
import Header from "./Header.vue";
import Layout from "./Layout.vue";

export default {
components: {
    Header,
    Layout
}
}

</script>