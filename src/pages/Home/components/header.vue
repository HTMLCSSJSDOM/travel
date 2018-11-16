<template>
	<div class="header-wrapper">
		<div class="header-left">
			<div class="iconfont">&#xe624;</div>
		</div>
		<div class="header-input">
			<span class="iconfont">&#xe632;</span>
			输入城市/景点/游玩主题
		</div>
		<div class="header-right">{{ city }}
			<span class="iconfont arrow-icon">&#xe64a;</span>
		</div>
	</div>
</template>

<script type="text/javascript">
	export default {
		name: 'home-header',
		data(){
			return {
				
			}
		},
		props: {
			city: {
				type: String,
				default: 'shen'
			}
		}
	}
</script>

<style scoped lang="stylus">
	@import '~styles/variables'
	
	.header-wrapper
		display flex
		line-height .86rem
		background-color $bgColor
		color #fff
		.header-left
			float left
			width .64rem
			text-align center
		.header-input
			height .64rem
			padding-left .2rem
			margin-top .12rem
			margin-left .2rem
			flex-grow 1
			border-radius .1rem
			line-height .64rem
			color #ccc
			background-color #fff
		.header-right
			float right
			width 1.24rem
			text-align center
			.arrow-icon
				font-size .24rem
			
</style>



