<template>
<!--	<view class="content">-->
<!--		<view class="text-area">-->
<!--			<text class="title">{{title}}</text>-->
<!--		</view>-->
<!--	</view>-->

	<!-- <view hover-class="v1">hello</view>
	<view >world</view> -->
	<!-- <scroll-view class="scroll-y" scroll-y="true" >
		<view class="v1"></view>
		<view class="v2"></view>
		<view class="v3"></view>
	</scroll-view> -->
	
	<scroll-view class="scroll-x" scroll-x="true" >
		<view class="v11"></view>
		<view class="v22"></view>
		<view class="v33"></view>
	</scroll-view>

</template>

<script>
	export default {
		// onLoad:function() {
		// 	console.log("index load")
		// },
		// onShow() {
		// 	console.log("index onshow")
		// 	console.log(getApp().globalData.name)
		// },
		// onReady() {
		// 	console.log("index ready")
		// },
		// data() {
		// 	return {
		// 		title: 'Hello lzc123'
		// 	}
		// },
		methods: {

		}
	}
</script>

<style>
	.scroll-x {
		white-space: nowrap;
	}
	.v11 {
		display: inline-block;
		width: 100%;
		height: 300rpx;
		background-color: royalblue;
	}
	.v22 {
		display: inline-block;
		width: 100%;
		height: 300rpx;
		background-color: aqua;
	}
	.v33 {
		display: inline-block;
		width: 100%;
		height: 300rpx;
		background-color: brown;
	}
	
	.scroll-y {
		height: 400rpx;
	}
	.v1 {
		width: 100%;
		height: 300rpx;
		background-color: royalblue;
	}
	.v2 {
		width: 100%;
		height: 300rpx;
		background-color: aqua;
	}
	.v3 {
		width: 100%;
		height: 300rpx;
		background-color: brown;
	}
	/* .v1 {
		color: red;
	} */
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
