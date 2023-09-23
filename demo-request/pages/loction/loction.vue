<template>
	<view>
		<button type="primary" @click="getLocation"> 获取位置 </button>
		<map :latitude="latitude" :longitude="longitude" scale="20"></map>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				longitude: '',
				latitude: '',
			}
		},
		methods: {
			getLocation:function(){
				var that = this
				uni.getLocation({
					success:function(res){
						that.res.latitude
						that.res.longitude
						console.log(res)
					}
				})
			}
		}
	}
</script>

<style>

</style>
