<template>
    <form class="d-flex align-items-center">
        <button type="submit">
            <i class="fa-solid fa-magnifying-glass align-middle"></i>
        </button>
        <input type="search" name="searchbar" placeholder="Search...">
    </form>
</template>

<script>
export default {
    name: 'SearchBar',
}
</script>

<style lang="scss" scoped>
form {
    padding: var(--standard-searchbar-padding);
    background-color: var(--pentenary-bg-color);
    border-radius: var(--standard-border-radius);

    & > * {
        border: none;
        background-color: transparent;
    }

    button {
        cursor: pointer;
        margin-right: 1rem;
    }
}
</style>