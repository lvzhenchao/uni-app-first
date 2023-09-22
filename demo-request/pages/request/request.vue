<template>
	<view>
		<button type="primary" @click="getData">获取数据</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			getData:function(){
				uni.request({
					url: "http://api.sungoal.com/",
					method:"POST",
					data:{
						"name": "lzc"
					},
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
