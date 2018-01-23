<template>
  <z-panel view="about">
    About Me
    <z-scale
      slot="circles"
      :angle="-45"
      gotoview="experience"
      size="large"
    >
      <span class="links">Experience</span>
    </z-scale>
    <z-scale
      slot="circles"
      :angle="-225"
      gotoview="bio"
      size="large"
    >
      <span class="links">Bio</span>
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
