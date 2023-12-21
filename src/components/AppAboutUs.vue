<script>
export default {
    name: 'AppAboutUs',
    data() {
        return {
            links: [
                {
                    text: "DIGITAL COMICS",
                    src: "../assets/buy-comics-digital-comics.png",
                },
                {
                    text: "DC MERCHANDISE",
                    src: "../assets/buy-comics-merchandise.png",
                    current: true,
                },
                {
                    text: "SUBSCRIPTION",
                    src: "../assets/buy-comics-subscriptions.png",
                },
                {
                    text: "COMIC SHOP LOCATOR",
                    src: "../assets/buy-comics-shop-locator.png",
                },
                {
                    text: "DC POWER VISA",
                    src: "../assets/buy-dc-power-visa.svg",
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
                    <img :src="link.src" alt="">
                    <a href="#">
                        {{ link.text }}
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
        align-items: center;

        // div {
        //     width: 100%;
        //     height: 100%;
        //     display: flex;
        //     align-items: center;
        //     justify-content: center;

        //     img {
        //         width: 50px;
        //         height: auto;
        //         margin-right: 1rem;
        //     }

        //     a {
        //         color: $primary;
        //         font-size: $font14;
        //         text-decoration: none;
        //     }
        // }
        ul {
            list-style: none;
            margin: 2.5rem 1rem 4rem;
            @include center();

            li a {
                text-align: center;
                display: inline-block;
                padding: 1rem;
                text-decoration: none;
                font-weight: 600;
                font-size: $font14;
                color: $bg-black;
            }
        }
    }
}
</style>

