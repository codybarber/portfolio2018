<template>
  <z-panel view="Home">
    <h1>Cody Barber</h1><hr>
    <h5>Frontend Developer</h5>
    <z-scale
      slot="circles"
      :angle="45"
      gotoview="about"
      size="large"
    >
      <span class="links">About Me</span>
    </z-scale>
    <z-scale
      slot="circles"
      :angle="-90"
      gotoview="contact"
      size="large"
    >
      <span class="links">Contact</span>
    </z-scale>
  </z-panel>
</template>
<script>
export default {
  name: 'Home',
  data () {
    return {
      msg: 'Welcome to Your Vue.js PWA'
    }
  }
}
</script>
