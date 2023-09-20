<template>
	<view>
		this is router vue
		<view class="">
			<navigator url="/pages/router/test/test">点我跳转到/pages/router/test页面</navigator>
		</view>
		<view class="">
			<button @click="go" type="primary">跳转</button>
		</view>
		<view class="">
			<button type="primary" @click="redirect">重定向</button>
		</view>
		
		<view class="">
			<button type="primary" @click="goTab">跳tab栏页面</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			go:function(){
				uni.navigateTo({
					url:"/pages/router/test/test?id=123&name=lzc"
				})
			},
			redirect:function(){
				uni.redirectTo({
					url:"./test/test"
				})
			},
			goTab:function(){
				uni.switchTab({
					url:'/pages/index/index'
				})
			}
			
		}
	}
</script>

<style>

</style>
