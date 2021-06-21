<template>
    <div class="nav ">
        <nav class="navbar is-dark" role="navigation" aria-label="main navigation">
            <div class="navbar-brand">
                <a class="navbar-item" href="/">
                    <img src="../assets/logo.png" width="100" height="200">
                </a>
                <a role="button" class="navbar-burger" :class="{ 'is-active': isHamburgerOpen }" @click="openHamburger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
                    <span aria-hidden="true"></span>
                    <span aria-hidden="true"></span>
                    <span aria-hidden="true"></span>
                </a>
            </div>

            <div id="navbarBasicExample" class="navbar-menu" :class="{ 'is-active': isHamburgerOpen }">
                <div class="navbar-end">
                    <router-link class="navbar-item" to="/about">
                        About
                    </router-link>

                    <router-link class="navbar-item" to="/contact">
                        Contact
                    </router-link>

                </div>
            </div>
</nav>
    </div>
</template>

<script>
export default {
    data() {
        return {
            isHamburgerOpen: false,
        }
    },
    methods: {
        openHamburger(){
            this.isHamburgerOpen = !this.isHamburgerOpen
        }
    }
}
</script>

<style>

</style>