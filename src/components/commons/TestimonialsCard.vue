<template>
    <div class="testimonials-card">
        <div class="card-image">
            <img :src="cardImg" :alt="cardAlt">
        </div>
        <div class="card-text">
            <p>{{firstCardTxt}}</p>
            <p>{{secondCardTxt}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'TestimonialsCard',

    props: {
        cardImg: String,
        cardAlt: String,
        firstCardTxt: String,
        secondCardTxt: String,
    }
}
</script>

<style lang="scss" scoped>
.testimonials-card {
    text-align: center;

    img {
        width: 30%;
        border-radius: 50%;
        margin-bottom: 2.5rem;
    }

    p:last-of-type {
        color: var(--exanary-txt-color);
    }
}
</style>