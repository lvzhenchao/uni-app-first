<template>
	<view>
		<button type="primary" @click="getData">获取数据</button>
		<!-- <view class="">
			{{data}}
		</view> -->
		<view v-for="(item,index) in data" :key="index">
			{{item}}
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				data: ['php', 'java', 'python']
			}
		},
		// onLoad:function(){
		// 	uni.startPullDownRefresh({
		// 		success:function(){
		// 			this.data = "refresh data"
		// 		}
		// 	}),
		// 	uni.stopPullDownRefresh()
		// },
		onPullDownRefresh:function(){
			this.data.unshift(Math.random())
			uni.stopPullDownRefresh()
		},
		onReachBottom:function(){
			this.data.push(Math.random())
		},
		
		methods: {
			getData:function(){
				uni.request({
					url: "http://api.sungoal.com/",
					method:"POST",
					success:function(res){
						console.log(res)
					}
				})
			}
		}
	}
</script>

<style>

</style>
