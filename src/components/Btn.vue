<template>
  <button class="button">{{ text }}</button>
</template>

<script>
export default {
    el: '.button',
    props: {
        text: String
    }
};
</script>

<style lang="scss" scoped>
    button {
        font-family: 'Proxima-Bold';
        font-size: 20px;
        font-weight: 700;
        color: var(--white);
        padding: 11px 54px;
        background: var(--blue);
        border-radius: 6px;
        border: 0;
        outline: 0;
    }
</style>