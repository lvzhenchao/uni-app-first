<template>
	<view>
		<uni-combox label="" :candidates="city" placeholder="输入"></uni-combox>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				city:['青岛', '北京', '南京']
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
