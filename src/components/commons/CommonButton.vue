<template>
    <button :type="buttonType" :class="buttonClass">
        <a :href="buttonLink">{{buttonText}}</a>
    </button>
</template>

<script>
export default {
    name: 'CommonButton',

    props: {
        buttonType: String,
        buttonClass: String,
        buttonLink: String,
        buttonText: String,
    }
}
</script>

<style lang="scss" scoped>
button {
    border-radius: var(--standard-border-radius);
    padding: var(--standard-microcomp-padding);
    border: none;
    cursor: pointer;

    &:active {
        transform: translateY(0.125rem);
    }

    &.primary {
        background-color: var(--primary-button-bg);
        color: var(--primary-button-txt);

        &:hover {
            background-color: var(--primary-button-hover-bg);
            color: var(--primary-button-hover-txt);
        }
    }

    &.secondary {
        background-color: var(--secondary-button-bg);
        color: var(--secondary-button-txt);
    
        &:hover {
            background-color: var(--secondary-button-hover-bg);
            color: var(--secondary-button-hover-txt);
        }
    }
}
</style>