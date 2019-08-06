<template>
    <div>
        <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="#">MabenaApp</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item :to="{ name: 'Home' }">Home</b-nav-item>
        <b-nav-item href="#" >New Complaint</b-nav-item>
        <b-nav-item href="#" >View Complaints</b-nav-item>

      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item :to="{ name: 'Login' }" right>Login</b-nav-item>

        <b-nav-item href="#" right>Register</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
    </div>
</template>

<script>
    export default {
        name: 'Navbar'
    }
</script>

<style scoped>
    .navs {
        
    }
    
    .account {
        
    }
</style>
