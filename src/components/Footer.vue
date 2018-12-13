<template>
  <div class="header">
    <!-- Navbar Code -->
    <b-navbar toggleable="md" type="dark" variant="info" fixed="bottom">

      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>

      <b-navbar-brand href="#">{{ title }}</b-navbar-brand>

      <b-collapse is-nav id="nav_collapse">

        <b-navbar-nav>
          <b-nav-item href="#">Link</b-nav-item>
          <b-nav-item href="#" disabled>Disabled</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-text>© All rights reserved. Made with ❤️ by S. Reyes</b-nav-text>
        </b-navbar-nav>

      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: 'footer',
  props: {
    title: String
  }
}
</script>

<style>
/* Nothing for now */
</style>