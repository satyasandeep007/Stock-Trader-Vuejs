<template>
  <div class="container">
    <app-header></app-header>
    <div class="row">
      <div class="col-md-12">
        <router-view />
      </div>
    </div>
  </div>
</template>
<script>
import Header from './views/Header';

export default {
  components: {
    appHeader : Header,
  },
}
</script>

<style lang="scss">
.container{
  padding: 30px;
}
</style>
