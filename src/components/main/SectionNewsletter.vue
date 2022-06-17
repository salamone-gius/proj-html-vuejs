<template>
    <section class="newsletter-section container">
        <div class="join-newsletter">
            <h2>Join our newsletter</h2>
            <p>Volutpat vel turpis nulla lorem sed semper. Aliquam sagittis sem libero viverra vehicula nullam ut nisl.</p>
            <div class="subscribe-form">
                <SubscribeForm
                    inputStyle="margin-right: 6rem;"
                />
            </div>
        </div>
    </section>
</template>

<script>
import SubscribeForm from './../commons/SubscribeForm.vue';

export default {
    name: 'SectionNewsletter',

    components: {
        SubscribeForm,
    }
}
</script>

<style lang="scss" scoped>
.newsletter-section {
    width: 90%;
    background-color: var(--secondary-bg-color);
    background-image: url("./../../assets/img/banner-7-2x-scaled.jpg");
    background-size: 75rem;
    background-repeat: no-repeat;
    background-position: right;
    position: relative;
    top: -4.5rem;

    .join-newsletter {
        width: 60%;
        padding-left: 5rem;
        padding-top: 1rem;
        padding-bottom: 5rem;

        h2 {
            font-size: 2.5rem;
        }

        p {
            margin: 3rem 0;
        }
    }
}
</style>