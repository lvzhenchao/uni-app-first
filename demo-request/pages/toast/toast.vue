<template>
	<view>
		<button type="primary" @click="onclick">点我</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			onclick: function(){
				// uni.showToast({
				// 	title: "ok",
				// 	duration:1500,
				// 	icon:'loading',
				// }),
				uni.showModal({
					title:"是否删除",
					success:function(res){
						console.log(res);
					}
				})
			},
			
		}
	}
</script>

<style>

</style>
