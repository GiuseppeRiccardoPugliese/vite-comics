<script>
export default {
    name: 'AppContent',
}
</script>

<template>
    <main>
        <div class="container">
            <h2> ... Content goes here ...</h2>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

main {
    background-color: $bg-black;
    height: 130px;

    .container {
        width: 100%;
        height: 100%;
        display: flex;
        align-items: center;
    }


    h2 {
        color: $primary;
    }
}
</style>

