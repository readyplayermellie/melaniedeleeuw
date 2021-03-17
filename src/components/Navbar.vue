<template>
    <nav class="nav-container">
        <div id="nav-logo">
            <p>[Ready player mellie]</p>
        </div>
        <div id="icons" v-for="icon in icons" :key="icon.index">
            <a :href="icon.href">
                <img :src="`${icon.src}`" :alt="icon.alt">
            </a>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'Navbar',
    data() {
        return {
            icons: [
                {
                    name: 'instagram',
                    href: 'https://www.instagram.com/melaniedeleeuw_',
                    src: '../assets/instagram.png',
                    alt: 'Instagram of Melanie'
                }
            ]
        }
    }
}
</script>

<style scoped>
.nav-container {
    margin: 15px;
    display: flex;
    justify-content: space-between;
    padding: 5px;
}
p,
a {
    text-transform: uppercase;
}
</style>
