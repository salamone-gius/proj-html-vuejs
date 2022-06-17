<template>
    <nav>
        <ul class="d-flex justify-content-center align-items-center">
            <li v-for="(link, index) in links" :key="index" :class="{active : link.current}">
                <a :href="link.url">{{link.text}}</a>
            </li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: 'NavBarBis',

    data() {
        return {
            links: [
                {
                    text: "Home",
                    url: "#",
                    current: true,
                },
                {
                    text: "About",
                    url: "#",
                    current: false,
                },
                {
                    text: "Blog",
                    url: "#",
                    current: false,
                },
                {
                    text: "Contact",
                    url: "#",
                    current: false,
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false,
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
ul {
    list-style: none;
    margin: 0;
    padding: 3rem;

    li {
        margin: 0 2rem;
        cursor: pointer;

        a, svg {
            text-decoration: none;
            color: var(--exanary-txt-color);
            vertical-align: middle;
            font-weight: 500;
        }

        svg {
            margin-left: .5rem;
            font-size: .625rem;
        }

        &:hover > a, &:hover > svg {
            color: var(--primary-txt-color);
        }
    }
}

.active {
    & > * {
        color: var(--primary-txt-color);
    }
}

</style>