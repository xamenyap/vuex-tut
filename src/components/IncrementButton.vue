<template>
	<div>
		<input type="button" value="Increase" @click="increaseCount"><br/>
		<span>{{count}}</span><br/>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				count: 0
			};
		},
		methods: {
			increaseCount() {
				this.$store.commit('increment');
				this.count++;
			}
		}
	}
</script>