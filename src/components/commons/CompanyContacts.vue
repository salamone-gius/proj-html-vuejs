<template>
    <div class="company-contacts">
        <img :src="require('../../assets/img/mobile-light-pet-logo-2x.png')" alt="Logo">
        <p>
            1234 Avada Avenue Avadaville<br>
            info@your-company.com<br>
            Call us: (1) 234 5678
        </p>
    </div>
</template>

<script>
export default {
    name: 'CompanyContacts',
}
</script>

<style lang="scss" scoped>
img {
    width: 80%;
    margin-bottom: 3rem;
}
</style>