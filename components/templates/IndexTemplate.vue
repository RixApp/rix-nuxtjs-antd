<template class="template">
  <a-layout>
    Hi from IndexTemplate!
    <NavBar />
  </a-layout>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
// import { Component, Prop, Vue } from 'vue-property-decorator';
import NavBar from '../primary/NavBar/index.vue';

@Component({
  props: {
    propTitle: String,
  },
  components: {
    NavBar,
  },
})
class IndexTemplate extends Vue {
  mounted = () => ({
    formLayout: 'horizontal',
  });
}

export default IndexTemplate;
</script>

<style style="sass" scoped>
</style>
