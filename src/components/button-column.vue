<template>
    <div class="wrapper" @click="$emit('click')">
        <slot />
    </div>
</template>

<style lang="less" scoped>
.wrapper {
    height: 100vh;
    width: 12vw;
    flex-shrink: 0;
    padding: 7vh 1vw 7vh 1vw;
    flex-direction: column;
    justify-content: space-between;
}
</style>

<script>
export default {
    name: 'ButtonColumn',
}
</script>