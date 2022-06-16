<template>
    <div class="header-bottom py-3">
        <NavBar/>
    </div>
</template>

<script>
import NavBar from './../commons/NavBar.vue';

export default {
    name: 'HeaderBottom',

    components: {
        NavBar,
    },
}
</script>

<style lang="scss" scoped>
.header-bottom {
    border-top: 1px solid var(--pentenary-bg-color);
}
</style>