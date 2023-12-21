<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true,
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false,
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false,
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<template>
    <header>

        <!-- Logo principale -->
        <a href="#">
            <img src="/public/dc-logo.png" alt="DC LOGO">
        </a>

        <nav>
            <ul>
                <li v-for="link in links">
                    <a :href="link.url" :class="link.current ? 'active' : ''">
                        {{ link.text }}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header {
    display: flex;
    justify-content: space-between;
    padding: 20px 0;

    a {
        align-items: center;
        display: flex;

        img {
            width: 80px;
        }
    }

    nav {
        display: flex;

        ul {
            list-style: none;
            @include center();

            li a {
                padding: 1rem;
                text-decoration: none;
                font-weight: 600;
                font-size: $font14;
                color: $bg-black;

                &.active,
                &:hover {
                    color: ($blue);
                }
            }
        }
    }


}
</style>

