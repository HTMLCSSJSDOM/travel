<template>
	<div>
		
		<home-header></home-header>
<<<<<<< HEAD
		<home-icons></home-icons>
		<!-- <home-recommand></home-recommand> -->
=======
		<home-icon></home-icon>
>>>>>>> homeSwiper
	</div>
</template>

<script type="text/javascript">
	import header from './components/header'
<<<<<<< HEAD
	import icons from './components/Icons'
	// import recommand from './components/Recommand'
=======
	import homeIcon from './components/Icons.vue'
>>>>>>> homeSwiper
	export default {
		name: 'home',
		components: {
			'home-header': header,
<<<<<<< HEAD
			'home-icons': icons,
			// 'home-recommand': recommand
=======
			'home-icon': homeIcon
>>>>>>> homeSwiper
		},
		data(){
			return {
				
			}
		}
	}
</script>

<style scoped>
	
</style>

