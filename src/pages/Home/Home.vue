<template>
	<div>
		
		<home-header :city="city"></home-header>

		<home-icons></home-icons>

		<home-recommand></home-recommand>

		<home-weekend></home-weekend>	

	</div>
</template>

<script type="text/javascript">
	import header from './components/header'

	import icons from './components/Icons'

	import recommand from './components/Recommand'
	import weekend from './components/Weekend.vue'

	export default {
		name: 'home',
		components: {
			'home-header': header,
			'home-icons': icons,
			'home-recommand': recommand,
			'home-weekend': weekend
		},
		data(){
			return {
				city: ''
			}
		},
		created() {
			console.log(this.$chidren)
		}
	}
</script>

<style scoped>
	
</style>

