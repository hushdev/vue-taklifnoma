<template>
    <h2 class="h2">{{text}}</h2>
</template>

<script>
export default {
    el: '.h2',
    props: {
        text: String
    }
}
</script>

<style lang="scss" scoped>
    h2 {
        font-family: 'Proxima-Black';
        color: var(--blue);
        font-size: 60px;
        font-weight: 900;
    }

</style>