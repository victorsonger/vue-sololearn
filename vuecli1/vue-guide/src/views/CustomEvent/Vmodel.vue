<template>
  <div class="custom-event-vmodel">
    <h2>自定义v-model</h2>
    <VmodelChild v-model="childValue"></VmodelChild>
  </div>
</template>

<script>
import VmodelChild from './VmodelChild.vue';
export default {
  name: 'Vmodel',
  components: {
    VmodelChild,
  },
  data() {
    return {
      childValue: false,
    }
  },
  watch: {
    childValue(val, oldVal) {
      console.log('val:', val, 'oldVal:', oldVal);
    }
  },
  methods: {
  }
}
</script>
