<template>
	<view>
		this is test vue
		<view class="">
			<navigator open-type="navigateBack">跳回</navigator>
		</view>
		<view class="">
			<button type="primary" @click="back">按钮跳回</button>
		</view>
	</view>
</template>

<script>
	export default {
		onLoad: function(option) {
			console.log(option.id)
			console.log(option.name)
		},
		data() {
			return {
				
			}
		},
		methods: {
			back:function(){
				uni.navigateBack({
					
				})
			}
		}
	}
</script>

<style>

</style>
