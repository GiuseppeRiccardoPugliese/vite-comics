<script>
export default {
    name: 'AppFooter',
}
</script>

<template>
    <footer>
        <div class="container">

            <div class="left"> <!-- BTN SIGN-UP -->
                <button>SIGN-UP NOW!</button>
            </div>

            <div class="right"> <!-- SOCIALS W/ICONS -->
                <span>FOLLOW US</span>
                <a href="#"><img src="/public/footer-facebook.png" alt=""></a>
                <a href="#"><img src="/public/footer-twitter.png" alt=""></a>
                <a href="#"><img src="/public/footer-youtube.png" alt=""></a>
                <a href="#"><img src="/public/footer-pinterest.png" alt=""></a>
                <a href="#"><img src="/public/footer-periscope.png" alt=""></a>
            </div>

        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

footer {
    height: 119px;
    width: 100%;
    background-color: $bg-light_black;
    display: flex;

    .container {
        display: flex;
        flex-grow: 1;
        justify-content: space-between;
        align-items: center;

        .left button {
            background-color: $bg-light_black;
            border: 2px solid $blue;
            padding: 0.5rem;
            color: $primary;
            font-weight: 600;
            cursor: pointer;

            &:hover {
                background-color: $blue;
                opacity: 0.6;
            }
        }

        .right {
            display: flex;
            align-items: center;
        }

        .right span {
            color: $blue;
            font-weight: 800;
            margin-right: 10px;
        }

        .right a {
            padding: 0.4rem;
        }
    }

}
</style>

