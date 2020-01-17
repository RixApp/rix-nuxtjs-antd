<template>
  <div class="container">
    <IndexTemplate />
  </div>
</template>

<script type="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import IndexTemplate from '~/components/templates/IndexTemplate.vue';

@Component({
  props: {
    propTitle: String
  },
  components: {
    IndexTemplate
  }
})
class Index extends Vue {
  mounted () {
    return {
      formLayout: 'horizontal'
    }
  }
}

export default Index;
</script>
