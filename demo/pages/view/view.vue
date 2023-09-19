<!-- 
类似div,用于包裹各种元素内容
属性：
hover-class 指定按下去的样式类
hover-stop-propagation 阻止本节点的祖先节点出现点击态，阻止冒泡
 -->
<template>
	<!-- <view class="" hover-class="v1">hello lampol</view> -->
	<view class="v2">
		<view hover-class="v1">
			hello lzc {{id}}
		</view>
	</view>
	
	<view hover-class="v4" class="v2">
		<view hover-class="v3" class="v1" hover-stop-propagation>
			hello lampol
		</view>
	</view>
	
</template>

<script>
	export default {
		onLoad:function(options) {
			this.id = options.id
		},
		data() {
			return {
				id:''
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.v1 {
		background-color: blue;
	}
	.v2 {
		width: 200rpx;
		height: 200rpx;
		background-color: aqua;
	}
	.v3 {
		width: 100rpx;
		height: 100rpx;
		background-color: palegreen;
	}
	.v4 {
		width: 100rpx;
		height: 100rpx;
		background-color: royalblue;
	}
</style>
