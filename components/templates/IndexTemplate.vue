<template class="template">
  <a-layout>
    Hi from IndexTemplate!
    <NavBar />
    <SideBar />
  </a-layout>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
// import { Component, Prop, Vue } from 'vue-property-decorator';
import NavBar from '../primary/NavBar/index.vue';
import SideBar from '../primary/SideBar/index.vue';

@Component({
  props: {
    propTitle: String,
  },
  components: {
    NavBar,
    SideBar,
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
