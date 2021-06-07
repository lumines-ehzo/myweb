<template>
  <div>
      <b-navbar type="dark" variant="dark">
          <b-navbar-nav>
              <nuxt-link class="nav-item nav-link" to="/">Home</nuxt-link>
              <nuxt-link class="nav-item nav-link" to="/users">Profile</nuxt-link>
              <nuxt-link class="nav-item nav-link" to="/parallax">Parallax-test</nuxt-link>
          </b-navbar-nav>
      </b-navbar>
      <nuxt/>
  </div>
</template>
<style>
 html,body{
     overflow: hidden;
 }
</style>