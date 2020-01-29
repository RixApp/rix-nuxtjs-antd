<template>
  <IndexTemplate />
</template>

<script type="ts">
import { Component, Vue } from 'vue-property-decorator';
// import { Component, Prop, Vue } from 'vue-property-decorator';
import IndexTemplate from '../components/templates/IndexTemplate.vue';

@Component({
  props: {
    propTitle: String,
  },
  components: {
    IndexTemplate,
  },
})
class Index extends Vue {
  mounted = () => ({
    formLayout: 'horizontal',
  });
}

export default Index;
</script>
