<template>
	<view>
		<view class="">
			<button @click="save" type="primary">点击数据保存</button>
		</view>
		<view class="">
			<button @click="getData" type="primary">获取缓存的数据</button>
		</view>
		<view class="">
			<button @click="reMove" type="primary">移除缓存的数据</button>
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
			save:function(){
				uni.setStorage({
					key:'name',
					data:"lvzhenchao",
					success: function(){
						console.log('成功')
					},
					fail: function(){
						console.log('失败')
					},
					complete: function(){
						console.log('完成')
					}
				})
			},
			getData:function(){
				uni.getStorage({
					key:'name',
					success: function(res){
						console.log(res);
					}
	
				})
			},
			reMove:function(){
				uni.removeStorage({
					key: 'name',
					success: function (res) {
						console.log(res);
						console.log("移除成功")
					}
				})
			}
		}
	}
</script>

<style>

</style>
