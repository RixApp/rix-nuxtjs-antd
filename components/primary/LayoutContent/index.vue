<template>
  <a-layout-content
    :style="{ background: '#fff', padding: '24px', margin: 0, height: '100%' }"
  >
    Content ------
  </a-layout-content>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  props: {
    contentType: String,
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
