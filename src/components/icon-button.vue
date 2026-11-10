<template>
    <div class="button" @click="$emit('click')">
        <image class="icon" :src="icon" />
    </div>
</template>

<script>
export default {
    name: 'IconButton',
    props: {
        icon: { type: String, required: true }
    },
}
</script>

<style lang="less" scoped>
@import "../styles/md-color.less";

.button {
    width: 10vw;
    height: 10vw;
    border-radius: 3vw;
    justify-content: center;
    align-items: center;
    background-color: @neutral;
}

.button:active {
    opacity: 0.6;
}

.icon {
    width: 60%;
    height: 60%;
}
</style>