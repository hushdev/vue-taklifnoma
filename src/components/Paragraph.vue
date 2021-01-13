<template>
    <p class="paragraph">{{text}}</p>
</template>

<script>
export default {
    el: '.paragraph',
    props: {
        text: String
    }
}
</script>

<style lang="scss" scoped>
    p {
        color: var(--dark);
        font-size: 20px;
    }
</style>