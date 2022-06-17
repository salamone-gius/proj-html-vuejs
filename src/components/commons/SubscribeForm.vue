<template>
    <div :style="containerStyle" class="subscribe-form">
        <form :style="formStyle" action="">
            <input :style="inputStyle" class="email-input" type="email" id="email" name="email" placeholder="Insert your email ...*" required>
            <CommonButton
                buttonType="submit"
                buttonClass="secondary"
                buttonText="Subscribe"
            />
        </form>
    </div>
</template>

<script>
import CommonButton from './CommonButton.vue';

export default {
    name: 'SubscribeForm',

    props: {
        containerStyle: String,
        formStyle: String,
        inputStyle: String,
    },

    components: {
        CommonButton,
    }
}
</script>

<style lang="scss" scoped>
.email-input {
    padding: var(--standard-inputbar-padding);
    background-color: var(--pentenary-bg-color);
    border-radius: var(--standard-border-radius);
    width: 21.875rem;
    border: none;
}
</style>