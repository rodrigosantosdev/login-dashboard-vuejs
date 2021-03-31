<template>
  <div class="content">
    <Nav />
    <FormBanner />
    <FormSignUp />
  </div>
</template>

<script>

import Nav from '../components/Nav.vue'
import FormBanner from '../components/FormBanner.vue'
import FormSignUp from '../components/FormSignUp.vue'

export default {
  components: { Nav, FormBanner, FormSignUp },
}

</script>

<style lang="scss">

.content {
  max-width: 1300px;
  height: 580px;
  display: flex;
  border-radius: 15px;
  background: var(--secondary);
}

@media ( max-width: 1260px ) {

  .content {
    width: 600px;
    height: 800px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
}

@media ( max-width: 700px ) {

  .content {
    width: 340px;
    height: 800px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
}

@media ( max-width: 470px ) {

  .content {
    width: 320px;
    margin: 0 auto;
  }
}
</style>