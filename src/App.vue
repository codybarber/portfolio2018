<template>
    <z-canvas class="theme--light .color--blue">
          <z-view-manager :list='$options.components'/>
    </z-canvas>
</template>
<script>
import Vue from 'vue'
import Router from 'vue-router'
import about from '@/components/about/about'
import experience from '@/components/about/experience'
import contact from '@/components/contact/contact'
import phone from '@/components/contact/phone'
import email from '@/components/contact/email'
Vue.use(Router)

const home = {
  template: `<z-panel view="Home">
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
</z-panel>`
}

const router = new Router({
  mode: 'history',
  routes: [
  {
    path: '/',
    redirect: '/home'
  },
  {
    path: '/home',
    name: 'home',
    component: home
  },
  {
    path: '/about',
    name: 'about',
    component: about
  },
  {
    path: '/about/experience',
    name: 'experience',
    component: experience
  },
  {
    path: '/contact',
    name: 'contact',
    component: contact
  },
  {
    path: '/contact/phone',
    name: 'phone',
    component: phone
  },
  {
    path: '/contact/email',
    name: 'email',
    component: email
  }]
})

export default {
  data () {
    return {
      initialView: 'Home',
      enableRouter: true
    }
  },
  components: {
    home,
    about,
    contact,
    phone,
    email,
    experience
  },
  router,
  beforeMount () {
    this.$zircleStore.routerHooks(this)
  }
}
</script>
<style>
.links {
  font-size: .7em;
}
</style>
