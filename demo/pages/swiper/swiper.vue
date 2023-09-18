<!-- 
轮播图
快捷键：usw
 -->
<template>
	<view>
		<swiper :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000">
			<swiper-item>
				<view class="v1"></view>
			</swiper-item>
			<swiper-item>
				<view class="v2"></view>
			</swiper-item>
			<swiper-item>
				<view class="v3"></view>
			</swiper-item>
		</swiper>
	</view>
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
