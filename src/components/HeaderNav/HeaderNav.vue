<template>
    <div class="nav_header">
        <b-navbar toggleable="lg" type="light" >
            <b-navbar-brand href="/"><img src="../../assets/images/peexoo.svg" alt="Peexoo Logo" class="peexoo_logo"></b-navbar-brand>

            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>

                <!-- Right aligned nav items -->
                <b-navbar-nav class="ml-auto white_bg">
                    <b-navbar-nav class="nav_header_inner">
                        <b-nav-item  ><router-link to="">I am a photographer</router-link></b-nav-item>
                        <b-nav-item ><router-link to="">Explore photos</router-link></b-nav-item>
                        <b-nav-item ><router-link to="">Find a photographer</router-link></b-nav-item>
                        <b-nav-item ><router-link to="">Find my photos</router-link></b-nav-item>
                        
                    </b-navbar-nav>
                    <b-navbar-nav class="login-nav">
                        <b-nav-item ><router-link to="" class="login-btn"><font-awesome-icon icon="lock" class="plus_icon"/> Login or Register</router-link></b-nav-item>
                    </b-navbar-nav>
                </b-navbar-nav>
            </b-collapse>
        </b-navbar>
    </div>
</template>

<script>
    export default {
        name: "HeaderNav.vue"
    }
</script>

<style scoped>
    a{
        text-decoration: none;
    }
    a:hover, a:focus, a:active{
        text-decoration: none;
        /*color: #FECB32;*/
    }
    .nav_header{
        padding: 0.5rem 2rem;
    }

</style>