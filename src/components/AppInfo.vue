<script>
export default {
    name: 'AppInfo',
}
</script>

<template>
    <section>
        <div class="container">

            <div class="left">
                <div>
                    <h2>DC COMICS</h2>
                    <ul>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                    </ul>
                </div>


                <h2>SHOP</h2>
                <ul>
                    <li>
                        <a href="#">Shop DC</a>
                    </li>
                    <li>
                        <a href="#">Shop DC Collectibles</a>
                    </li>
                </ul>
            </div>

            <div class="right">

            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

section {
    width: 100%;
    height: 400px;
    background-image: url(/public/footer-bg.jpg);
}
</style>