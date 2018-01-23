<template>
  <z-panel view="foo">
    Foo View
    <z-scale
      slot="circles"
      :angle="45"
      gotoview="bar"
    >
      Bar
      <span slot="label">Go to</span>
    </z-scale>
  </z-panel>
</template>
<script>
export default {
  data () {
    return {
      msg: 'Projects'
    }
  }
}
</script>
