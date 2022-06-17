<template>
    <div class="vertical-navbar">
        <h5>Shop by brand</h5>
        <ul>
            <li v-for="(category, index) in shopByBrand" :key="index">
                <a :href="category.url">
                    {{category.name}}
                </a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'VerticalNavbar',

    data() {
        return {
            shopByBrand: [
                {
                    name: "Bed",
                    url: "#"
                },
                {
                    name: "Food",
                    url: "#"
                },
                {
                    name: "Toys",
                    url: "#"
                },
                {
                    name: "Transport",
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