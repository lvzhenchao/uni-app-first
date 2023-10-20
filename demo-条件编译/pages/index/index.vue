<template>
	<view class="container">
		<!-- #ifdef H5 -->
			<text>这个只会在H5下显示哦</text>
		<!-- #endif -->
		
		<!-- #ifdef MP-WEIXIN -->
			<text>这个只会在小程序下显示</text>
		<!-- #endif -->
		
		<view class="">
			<text>{{msg}}</text>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				// #ifdef H5
				msg: 'hello h5',
				// #endif
				
				// #ifdef MP-WEIXIN
				msg: 'hello 小程序',
				// #endif
			}
		},
		methods: {

		}
	}
</script>

<style>
	.container {
		padding: 20px;
		font-size: 14px;
		line-height: 24px;
	}
	
	/* #ifdef H5 */
		text {
			color: red;
		}
	/* #endif */
	
	/* #ifdef MP-WEIXIN */
		text {
			color: blue;
		}
	/* #endif */
</style>
