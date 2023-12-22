<script>
export default {
    name: 'AppThumbs',
    props: {
        details: Object
    }
}
</script>

<template>
    <div class="thumb-card">
        <a href="#">
            <img :src="details.thumb" :alt="details.type">
            <h3>{{ details.series }}</h3>
        </a>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.thumb-card {
    width: calc((100% / 6) - 1rem);
    margin: 0.5rem;

    // flex-basis: 15%;
    a {
        text-decoration: none;

        h3 {
            color: $primary;
            // padding-bottom: 10px;
            margin: 1rem 0;
        }

        img {
            width: 200px;
            height: 250px;
        }
    }
}
</style>

