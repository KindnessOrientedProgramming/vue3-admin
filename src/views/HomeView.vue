<template>
  <header>顶部导航栏</header>
  <section class="app-wrapper">
    <aside class="sidebar-container">侧边菜单栏</aside>
    <section>内容主体</section>
  </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'HomeView',
  components: {}
})
</script>

<style lang="scss" scoped>
@import '~@/styles/variables.scss';

header {
  background-color: #{$headerBgColor};
  height: #{$headerHeight};
}
.app-wrapper {
  display: flex;
  height: calc(100vh - #{$headerHeight});
  .sidebar-container {
    width: #{$sidebarWidth};
    background-color: #{$sidebarBgColor};
  }
}
</style>
