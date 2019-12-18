<template>
  <div class="custom-event-vmodel">
    <input
      type="checkbox"
      v-bind:checked="checked"
      v-on:change="$emit('change', $event.target.checked)"
    />
  </div>
</template>

<script>
export default {
  name: 'VmodelChild',
  props: {
    checked: Boolean
  },
  model: {
    prop: 'checked',
    event: 'change',
  },
}
</script>
