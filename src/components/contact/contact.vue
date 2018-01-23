<template>
  <z-panel view="contact">
    Contact
    <z-scale
      slot="circles"
      :angle="45"
      gotoview="phone"
      size="large"
    >
      <span class="links contact-icons fa fa-phone" ></span>
    </z-scale>
    <z-scale
      slot="circles"
      :angle="-135"
      gotoview="email"
      size="large"
    >
      <span class="links contact-icons fa fa-envelope" ></span>
    </z-scale>
  </z-panel>
</template>
<script>
export default {
  data () {
    return {
    }
  }
}
</script>
<style>
.links {
  font-size: .7em;
}
.contact-icons {
  font-size: 1.5em;
}
</style>
