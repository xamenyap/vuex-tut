<template>
  <div>
    <span>Total count is: {{count}}</span><br/>
    <increment-button></increment-button>
    <increment-button></increment-button>
    <increment-button></increment-button>
  </div>
</template>

<script>
import IncrementButton from './components/IncrementButton.vue';
import {mapState} from 'vuex';

export default {
  name: 'app',
  components: { IncrementButton },
  computed: {
    ...mapState({
      count: 'count'
    })
  }
}
</script>