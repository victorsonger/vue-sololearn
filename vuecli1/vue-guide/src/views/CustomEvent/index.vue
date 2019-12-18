<template>
  <div class="custom-event-home">
    <button @click="goVmodel">自定义v-model</button>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'CustomEvent',
  methods: {
    goVmodel() {
      this.$router.push('/customEvent/vmodel')
    }
  }
}
</script>
