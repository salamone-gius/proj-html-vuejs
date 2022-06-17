<template>
    <div class="footer-bottom">
        <i class="fa-regular fa-copyright"></i>
        <span>Copyright 2012 - 2022 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress</span>
    </div>
</template>

<script>
export default {
    name: 'FooterBottom',
}
</script>

<style lang="scss" scoped>
.footer-bottom {
    background-color: var(--quaternary-bg-color);
    padding: 3rem;
    text-align: center;

    svg {
        margin-right: 0.5rem;
        vertical-align: middle;
    }
}
</style>