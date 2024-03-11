<template>
  <div id="left-side" class="left-side col-12 md:col-6 side flex align-items-center flex-column">
    <card class="w-full">
      <template #title> <h1>Welcome to Acme</h1></template>
      <template #subtitle> <h6>Create your account by filling the form bellow.</h6></template>
      <template #content>
        <div class="flex align-items-center field">
          <FloatLabel class="flex-auto">
            <InputText id="username" v-model="value" class="w-full" />
            <label for="username">Username</label>
          </FloatLabel>
        </div>
        <div class="flex align-items-center field">
          <FloatLabel class="flex-auto">
            <InputText id="password" v-model="password" class="w-full" />
            <label for="password">Password</label>
          </FloatLabel>
        </div>
        <div class="flex align-items-center">
          <Checkbox v-model="rememberMe" inputId="remember" name="remember" value="1" />
          <label for="remember" class="ml-2"> Remember me</label>
        </div>
      </template>
      <template #footer>
        <div class="flex align-items-center">
          <Button label="Sign up" class="ml-auto" />
        </div>
      </template>
    </card>
    <div class="left-footer w-full pt-5">
      &copy; 2015, Inc. <Button label="Terms" link /> <Button label="Privacy" link />
      <Button icon="pi pi-ellipsis-h" link />
    </div>
  </div>
</template>
<script>
import FloatLabel from 'primevue/floatLabel'
import InputText from 'primevue/inputtext'
import Checkbox from 'primevue/checkbox'
import Button from 'primevue/button'
import Card from 'primevue/card'

export default {
  components: { Card, Button, Checkbox, InputText, FloatLabel },
  data: () => {
    return {
      rememberMe: false
    }
  }
}
</script>
