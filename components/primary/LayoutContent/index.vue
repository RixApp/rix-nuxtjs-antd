<template class="template">
  <a-layout-content
    :style="{ margin: '24px 16px', padding: '24px', background: '#fff', minHeight: '280px' }"
  >
    Content
  </a-layout-content>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  props: {
    collapsed: Boolean,
  },
})
class LayoutContent extends Vue {
  mounted = () => ({
    formLayout: 'horizontal',
  });
}

export default LayoutContent;
</script>

<style style="sass" scoped>
</style>
