<script>
export default {
    name: 'AppAboutUs',
    data() {
        return {
            links: [
                {
                    text: "DIGITAL COMICS",
                    src: "/public/buy-comics-digital-comics.png",
                },
                {
                    text: "DC MERCHANDISE",
                    src: "/public/buy-comics-merchandise.png",
                },
                {
                    text: "SUBSCRIPTION",
                    src: "/public/buy-comics-subscriptions.png",
                },
                {
                    text: "COMIC SHOP LOCATOR",
                    src: "/public/buy-comics-shop-locator.png",
                },
                {
                    text: "DC POWER VISA",
                    src: "/public/buy-dc-power-visa.svg",
                },
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="link in links">

                    <a href="#">
                        <div>
                            <img :src="link.src" alt="">
                        </div>
                        <span>
                            {{ link.text }}
                        </span>
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

section {
    width: 100%;
    height: 150px;
    background-color: $blue;

    .container {
        height: 100%;
        width: 100%;
        display: flex;
        justify-content: center;

        ul {
            list-style: none;
            @include center();

            div {
                display: flex;
                justify-content: center;
                margin-right: 10px;
                width: 60px;
                height: 60px;
            }

            li a {
                display: flex;
                align-items: center;
                padding: 1rem;
                text-decoration: none;
                font-size: $font14;
                color: $primary;
            }
        }
    }
}
</style>

