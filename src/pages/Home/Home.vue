<template>
	<div>
		
		<home-header></home-header>
		<home-icons></home-icons>
		<!-- <home-recommand></home-recommand> -->
	</div>
</template>

<script type="text/javascript">
	import header from './components/header'
	import icons from './components/Icons'
	// import recommand from './components/Recommand'
	export default {
		name: 'home',
		components: {
			'home-header': header,
			'home-icons': icons,
			// 'home-recommand': recommand
		},
		data(){
			return {
				
			}
		}
	}
</script>

<style scoped>
	
</style>

