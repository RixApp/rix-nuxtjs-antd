<template>
  <a-layout style="padding: 0 24px 24px">
    <a-breadcrumb style="margin: 16px 0">
      <a-breadcrumb-item>Home</a-breadcrumb-item>
      <a-breadcrumb-item>List</a-breadcrumb-item>
      <a-breadcrumb-item>App</a-breadcrumb-item>
    </a-breadcrumb>
    <a-layout-content
      :style="{ background: '#fff', padding: '24px', margin: 0, minHeight: '535px' }"
    >
      Content
    </a-layout-content>
  </a-layout>
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
