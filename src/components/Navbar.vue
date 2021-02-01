<template>
    <nav class="nav-container">
        <div id="nav-logo">
            <p>Melanie de Leeuw</p>
        </div>
        <ul class="nav-social">
            
            <li class="list-item"><a href="#">About me</a></li>
            <li class="list-item"><a href="#">Projects</a></li>
            <li 
                v-for="item in socialItems"
                class="list-item"
                :key="item.key"
            >
                <a :href="item.href">
                    <img :src="item.src" class="icons">
                </a>
            </li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: 'Navbar',
    data() {
        return {
            socialItems: [
                { 
                    key: 'social-item-gitlab',
                    href: 'https://gitlab.com/readyplayermellie',
                    src: '../assets/gitlab.png'
                },
                { 
                    key: 'social-item-instagram',
                    href: 'https://www.instagram.com/melaniedeleeuw_/',
                    src: '../assets/instagram.png'
                },
                { 
                    key: 'social-item-github',
                    href: 'https://github.com/readyplayermellie',
                    src: './src/assets/github.png'
                }
            ]
        }
    }
}
</script>

<style scoped>
.nav-social {
    display: flex;
}
.nav-container {
    margin: 15px;
    display: flex;
    justify-content: space-between;
    padding: 5px;
}
.list-item {
    margin-left: 15px;
}

.icons {
    width: 18px;
}

p,
a {
    text-transform: uppercase;
}

</style>