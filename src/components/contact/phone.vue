<template>
  <z-panel view="phone">
    <span class="phone-number">706-202-9182</span>
    <z-scale
      slot="circles"
      :angle="45"
      gotoview="phone"
      size="large"
    >
      <a class="phone-link" href="tel:706-202-9182">Call</a>
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
.phone-number {
  font-size: 1.8em;
  color: #869BA5;
}
.phone-link {
  font-size: .7em;
  text-decoration: none;
  color: #869BA5;
}
.phone-link:hover {
  color: #3697DA;
}
</style>
