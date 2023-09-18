<template>
	<!-- <scroll-view class="scroll-y" scroll-y="true" >
		<view class="v1">v1</view>
		<view class="v2">v2</view>
		<view class="v3">v3</view>
	</scroll-view> -->
	<scroll-view class="scroll-x" scroll-x="true" >
		<view class="vv1">vv1</view>
		<view class="vv2">vv2</view>
		<view class="vv3">vv3</view>
	</scroll-view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.scroll-x {
		white-space: nowrap;
	}
	.vv1 {
		display: inline-block;
		width: 100%;
		height: 300rpx;
		background-color: red;
	}
	.vv2 {
		display: inline-block;
		width: 100%;
		height: 300rpx;
		background-color: blue;
	}
	.vv3 {
		display: inline-block;
		width: 100%;
		height: 300rpx;
		background-color: gold;
	}
	
	.scroll-y {
		height: 300rpx;
	}
	.v1 {
		width: 100%;
		height: 300rpx;
		background-color: red;
	}
	.v2 {
		width: 100%;
		height: 300rpx;
		background-color: blue;
	}
	.v3 {
		width: 100%;
		height: 300rpx;
		background-color: gold;
	}
</style>
