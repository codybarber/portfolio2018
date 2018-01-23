<template>
  <z-panel view="email">
    <span class="email-address">cody.n.barber@gmail.com</span>
    <z-scale
      slot="circles"
      :angle="45"
      gotoview="phone"
      size="large"
    >
    <a class="email-link" href="mailto:cody.n.barber@gmail.com" target="_top">
      Send Mail
    </a>
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
.email-address {
  font-size: 1.0em;
  color: #869BA5;
}
.email-link {
  font-size: .7em;
  text-decoration: none;
  color: #869BA5;
}
.email-link:hover {
  color: #3697DA;
}
</style>
