<template>
  <div class="content">
    <FormSignUp />
    <ContentDescription />
    <Nav />
  </div>
</template>

<script>

import Nav from '../components/Nav.vue'
import ContentDescription from '../components/ContentDescription.vue'
import FormSignUp from '../components/FormSignUp.vue'

export default {
  components: { Nav, ContentDescription, FormSignUp },
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