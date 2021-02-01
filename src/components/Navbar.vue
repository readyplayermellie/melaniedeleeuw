<template>
    <nav class="nav-container">
        <div id="nav-logo">
            <p>Melanie de Leeuw</p>
        </div>
        <div>
            <router-link to="/">Home</router-link> |
            <router-link to="/about">About</router-link> |
            <router-link to="/projects">Projects</router-link> |
            <router-link to="/blog">Blog</router-link>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'Navbar',
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