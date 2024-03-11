<template>
  <div id="right-side" class="right-side col-12 md:col-6 p-0">
    <div class="right-side-background"></div>
    <div class="right-side-content side d-flex align-items-center">
      <Logo />
      <h2>Do you already have an account?</h2>
      <h4>
        This is awesome! You can login by clicking on the button below. To skip this next time, you
        can ask us to remember your login credentials.
      </h4>
      <Button label="Login" severity="secondary" />
    </div>
    <div class="clear"></div>
  </div>
</template>
<script>
import Button from 'primevue/button'
import Logo from './Logo.vue'

export default {
  components: { Logo, Button }
}
</script>
<style scoped lang="scss">
@import '@/assets/scss/components/fontFamily.scss';

.right-side {
  position: relative;
  &-background {
    background: url('@/assets/img/bridge.jpeg') no-repeat center center;
    /* Add the blur effect */
    filter: blur(5px);

    height: 100%;
    width: 100%;

    /* Center and scale the image nicely */
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    position: absolute;
  }

  &-content {
    color: #fff;
    position: relative;
    z-index: 10;
  }
}
</style>
