<template>
  <div>
    <increment-button></increment-button>
    <increment-button></increment-button>
  </div>
</template>

<script>
import IncrementButton from './components/IncrementButton.vue';

export default {
  name: 'app',
  components: { IncrementButton },
  data() {
    return {};
  }
}
</script>