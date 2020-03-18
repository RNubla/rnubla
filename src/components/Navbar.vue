<template>
    <section class="hero">
        <div class="hero-body">
            <nav class="navbar">
               <div class="container">
                   <div class="navbar-brand">
                       <div class="navbar-item">
                           <h5 class="title">
                               <router-link class="level-item" to='/'>Robert Nubla</router-link>
                           </h5>
                       </div>
                       <span class="navbar-burger burger" v-on:click="toggleBurger" v-bind:class="{'is-active':isActive}" data-target="navbarMenus">
                           <span></span>
                           <span></span>
                           <span></span>
                       </span>
                   </div>
                   <div id="navbarMenus" class="navbar-menu" v-bind:class="{'is-active':isActive}">
                       <div class="navbar-end">
                            <router-link class="navbar-item" to='/'>Home</router-link>
                            <router-link class="navbar-item" to="/about">About</router-link>
                            <router-link class="navbar-item" to="/projects">Projects</router-link>
                       </div>
                   </div>
               </div>
            </nav>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Navbar',
    data: function(){
        return{
            isActive: false
        }
    },

    methods:{
        toggleBurger: function(){
            this.isActive = !this.isActive;
        }
    }
}
</script>