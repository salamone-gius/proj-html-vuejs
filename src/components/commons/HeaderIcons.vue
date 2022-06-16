<template>
    <div>
        <a href="#">
            <i class="fa-solid fa-cart-shopping align-middle"></i>
        </a>
        <a href="#">
            <i class="fa-solid fa-user align-middle"></i>
        </a>
    </div>
</template>

<script>
export default {
 name: 'HeaderIcons',
}
</script>

<style lang="scss" scoped>
a:first-child {
    margin-right: 1.2rem;
}

a {
    color: var(--secondary-txt-color);

    &:hover {
        color: var(--tertiary-txt-color);
    }
}

svg {
    font-size: 1.5rem;
}

</style>