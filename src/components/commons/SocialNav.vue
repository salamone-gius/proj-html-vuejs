<template>
    <div class="social">
        <a href="#">
            <i class="fa-brands fa-facebook-f"></i>
        </a>
        <a href="#">
            <i class="fa-brands fa-twitter"></i>
        </a>
        <a href="#">
            <i class="fa-brands fa-instagram"></i>
        </a>
        <a href="#">
            <i class="fa-brands fa-youtube"></i>
        </a>
    </div>
</template>

<script>
export default {
    name: 'SocialNav0',
}
</script>

<style lang="scss" scoped>
.social {
    padding-bottom: 5rem;
    text-align: center;

    a {
        text-decoration: none;
        color: var(--primary-txt-color);
        margin-right: 1.4rem;

        svg {
            font-size: 1.5rem;
        }

        &:hover {
            color: var(--exanary-txt-color);
        }
    }
}
</style>