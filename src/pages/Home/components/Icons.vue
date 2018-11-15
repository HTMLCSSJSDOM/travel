<template>
	<div class="icons">
		<swiper>
			<swiper-slide 
			v-for="page of pages"
			:key="page">
				<div class="icon-item" 
				v-for="item of page" 
				:key="item.id">
					<div class="icon-img">
						<img :src="item.imgUrl" alt="">
					</div>
					<p class="icon-text">{{ item.desc}}</p>
				</div>
			</swiper-slide>
			
		</swiper>
	</div>
</template>
<script type="text/javascript">

	export default {
		data() {
			return {
					iconsList: [{
						id: '001',
						imgUrl: "http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png",
						desc: '景点门票'
					},{
						id: '002',
						imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/ea/01d081dacb03cc02.png',
						desc: '秋色美'
					},{
						id: '003',
						imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/ea/01d081dacb03cc02.png',
						desc: '秋色美'
					},{
						id: '004',
						imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/ea/01d081dacb03cc02.png',
						desc: '秋色美'
					},{
						id: '005',
						imgUrl: "http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png",
						desc: '景点门票'
					},{
						id: '006',
						imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/ea/01d081dacb03cc02.png',
						desc: '秋色美'
					},{
						id: '007',
						imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/ea/01d081dacb03cc02.png',
						desc: '秋色美'
					},{
						id: '008',
						imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/ea/01d081dacb03cc02.png',
						desc: '秋色美'
					},{
						id: '009',
						imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/ea/01d081dacb03cc02.png',
						desc: '秋色美'
					}]
				}
			},
		created() {
			console.log(this.iconsList)
		},
		computed: {
			pages() {
				 const pages = []

				 this.iconsList.forEach((item, index) => {
				 	let page = Math.floor(index / 8)
				 	if(!pages[page]) {
				 		pages[page] = []
				 	}
				 	pages[page].push(item)
				 })

				 return pages
			}
		}
	}
</script>
<style lang="stylus" scoped>
	@import '~styles/variables'
	@import '~styles/mixins'
	.icons >>> .swiper-container
		overflow hidden
		height 0 
		padding-bottom 50%
		// background-color green
	.icon-item
		position relative
		float left
		width 25%
		height 0 
		padding-bottom 25%
		text-align center
		// background-color red
		.icon-img
			box-sizing boder-box
			position absolute
			top 0
			left 0
			right 0
			bottom .44rem
			padding .1rem
			// background-color blue
			img
				width 100%
				height 100% 
		.icon-text
			position absolute
			bottom 0
			right 0
			left 0
			height .44rem
			line-height .44rem
			color $darkTextColor
			ellipsis()
</style>