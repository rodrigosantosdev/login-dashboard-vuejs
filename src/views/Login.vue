<template>
  <div class="content">
    <Nav />
    <ContentDescription />
    <FormLogin />
  </div>
</template>

<script>

import Nav from '../components/Nav.vue'
import ContentDescription from '../components/ContentDescription.vue'
import FormLogin from '../components/FormLogin.vue'

export default {
  components: { Nav, ContentDescription, FormLogin },
}

</script>

<style lang="scss">
.content {
  width: 1230px;
  height: 580px;
  display: flex;
  border-radius: 15px;
  background: var(--secondary);
}
</style>