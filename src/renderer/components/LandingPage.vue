<template>
  <section class="hero is-success is-fullheight">
  <div class="hero-body">
    <div class="container">
      <h1 class="title">
        自动更新测试第二次
      </h1>
      <h2 class="subtitle">
        build(3)
      </h2>
    </div>
  </div>
</section>
</template>

<script>
  import SystemInformation from './LandingPage/SystemInformation'

  export default {
    name: 'landing-page',
    components: { SystemInformation },
    created () {
      console.log(this.$electron)
    },
    methods: {
      open (link) {
        this.$electron.shell.openExternal(link)
      }
    }
  }
</script>

<style>
</style>
