<template class="template">
  <a-layout-header style="background: #fff; padding: 0">
    <a-icon
      class="trigger"
      :type="collapsed ? 'menu-unfold' : 'menu-fold'"
      @click="()=> collapsed = !collapsed"
    />
  </a-layout-header>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  props: {
    collapsed: Boolean,
  },
})
class NavBar extends Vue {
  mounted = () => ({
    formLayout: 'horizontal',
  });
}

export default NavBar;
</script>

<style style="sass" scoped>
</style>
