<template class="template">
  <a-layout id="components-layout-demo-top-side-2">
    <NavBar />
    <SideBar />
    <LayoutContent />
  </a-layout>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
// import { Component, Prop, Vue } from 'vue-property-decorator';
import NavBar from '../primary/NavBar/index.vue';
import SideBar from '../primary/SideBar/index.vue';
import LayoutContent from '../primary/LayoutContent/index.vue';

@Component({
  props: {
    propTitle: String,
  },
  components: {
    NavBar,
    SideBar,
    LayoutContent,
  },
})
class IndexTemplate extends Vue {
  /* mounted = () => ({
    formLayout: 'horizontal',
  }); */
}

export default IndexTemplate;
</script>

<style style="sass" scoped>
#components-layout-demo-top-side-2 .logo {
  width: 120px;
  height: 31px;
  background: rgba(255, 255, 255, 0.2);
  margin: 16px 28px 16px 0;
  float: left;
}
</style>
