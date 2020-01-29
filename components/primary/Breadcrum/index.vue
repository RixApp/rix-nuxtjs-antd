<template>
  <a-breadcrumb style="margin: 16px 0">
    <a-breadcrumb-item>Home</a-breadcrumb-item>
    <a-breadcrumb-item>List</a-breadcrumb-item>
    <a-breadcrumb-item>App</a-breadcrumb-item>
  </a-breadcrumb>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  props: {
    collapsed: Boolean,
  },
})
class LayoutContent extends Vue {
  /* mounted = () => ({
    formLayout: 'horizontal',
  }); */
}

export default LayoutContent;
</script>

<style style="sass" scoped>
</style>
