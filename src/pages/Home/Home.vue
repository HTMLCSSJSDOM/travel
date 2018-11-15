<template>
	<div>
		
		<home-header></home-header>
		<home-icon></home-icon>
	</div>
</template>

<script type="text/javascript">
	import header from './components/header'
	import homeIcon from './components/Icons.vue'
	export default {
		name: 'home',
		components: {
			'home-header': header,
			'home-icon': homeIcon
		},
		data(){
			return {
				
			}
		}
	}
</script>

<style scoped>
	
</style>

