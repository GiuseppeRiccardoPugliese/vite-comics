<script>
export default {
    name: 'AppInfo',
}
</script>

<template>
    <section>
        <div class="container">

            <div class="left"> <!-- LISTS -->
                <div> <!-- DC COMICS & SHOP -->
                    <!-- DC COMICS -->
                    <h2>DC COMICS</h2>
                    <ul>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Comics</a>
                        </li>
                        <li>
                            <a href="#">Movies</a>
                        </li>
                        <li>
                            <a href="#">TV</a>
                        </li>
                        <li>
                            <a href="#">Games</a>
                        </li>
                        <li>
                            <a href="#">Videos</a>
                        </li>
                        <li>
                            <a href="#">News</a>
                        </li>
                    </ul>

                    <!-- SHOP -->
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

                <div> <!-- DC -->
                    <!-- DC -->
                    <h2>DC</h2>
                    <ul>
                        <li>
                            <a href="#">Terms Of Use</a>
                        </li>
                        <li>
                            <a href="#">Privacy policy (New)</a>
                        </li>
                        <li>
                            <a href="#">Ad Choices</a>
                        </li>
                        <li>
                            <a href="#">Advertising</a>
                        </li>
                        <li>
                            <a href="#">Jobs</a>
                        </li>
                        <li>
                            <a href="#">Subscriptions</a>
                        </li>
                        <li>
                            <a href="#">Talent Workshops</a>
                        </li>
                        <li>
                            <a href="#">CPSC Certificates</a>
                        </li>
                        <li>
                            <a href="#">Ratings</a>
                        </li>
                        <li>
                            <a href="#">Shop Help</a>
                        </li>
                        <li>
                            <a href="#">Contact Us</a>
                        </li>
                    </ul>
                </div>

                <div> <!-- SITES -->
                    <!-- SITES -->
                    <h2>SITES</h2>
                    <ul>
                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">MAD Magazine</a>
                        </li>
                        <li>
                            <a href="#">DC Kids</a>
                        </li>
                        <li>
                            <a href="#">DC Universe</a>
                        </li>
                        <li>
                            <a href="#">DC Power Visa</a>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="right"> <!-- BG IMG -->
                <img src="/public/dc-logo-bg.png" alt="">
            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

section {
    display: flex;
    width: 100%;
    height: 400px;
    background-image: url(/public/footer-bg.jpg);

    .container {
        display: flex;
        justify-content: space-between;
        flex-grow: 1;

        ul {
            list-style: none;

            li a {
                text-decoration: none;
                font-size: $font14;
                color: $primary;
                opacity: 0.5;
                line-height: 25px;

                &:hover {
                    color: ($blue);
                }
            }

        }

        h2 {
            color: $primary;
            margin: 15px 0;
        }

        .left {
            display: flex;
            width: 50%;
        }

        .left div {
            margin: 10px 15px;
        }

        .right {
            display: flex;
            justify-content: flex-end;
            position: relative;
            width: 50%;
        }

        .right img {
            width: 100%;
            height: 100%;
            position: absolute;
            object-fit: cover;
            top: 0;
            right: 0;
        }
    }


}
</style>