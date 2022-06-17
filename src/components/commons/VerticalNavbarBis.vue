<template>
    <div class="vertical-navbar">
        <h5>Useful links</h5>
        <ul>
            <li v-for="(link, index) in links" :key="index">
                <a :href="link.url">
                    {{link.name}}
                </a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'VerticalNavbarBis',

    data() {
        return {
            links: [
                {
                    name: "My account",
                    url: "#"
                },
                {
                    name: "Orders",
                    url: "#"
                },
                {
                    name: "Checkout",
                    url: "#"
                },
                {
                    name: "Cart",
                    url: "#"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.vertical-navbar {
    ul {
        list-style: none;
        padding: 0;

        li {
            padding: 0.8rem 0;

            a {
                text-decoration: none;
                color: inherit;
                cursor: pointer;

                &:hover {
                    color: var(--exanary-txt-color);
                }
            }
        }
    }
}
</style>