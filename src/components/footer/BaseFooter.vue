<template>
    <footer>
        <CommonButton :buttonText='"Learn more about us"' :buttonClass="'primary'"/>
        <CommonButton :buttonText='"Learn more about us"' :buttonClass="'secondary'"/>

    </footer>
</template>

<script>
import CommonButton from './../commons/CommonButton.vue'
export default {
    name: 'BaseFooter',

    components: {
        CommonButton,
    }
}
</script>

<style lang="scss" scoped>

</style>