<template class="template">
  <div class="container">
    Hi from IndexTemplate!
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
// import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
class IndexTemplate extends Vue {
  mounted = () => ({
    formLayout: 'horizontal',
  });
}

export default IndexTemplate;
</script>

<style style="sass" scoped>
.container {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: #E6E4E4;
}
</style>
