<template>
    <div>
        <img :src="url" alt="title">
        <h3>{{ title }}</h3>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        url: String,
        title: String,
    }
};

</script>

<style scoped lang="scss">
h3 {
    font-size: 12px;
    padding-top: 10px;
}

img {
    height: 150px;
    width: 150px;
    object-fit: cover;
}
</style>