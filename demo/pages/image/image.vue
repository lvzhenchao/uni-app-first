<template>
	<view>
		<image src="../../static/logo.png" mode=""></image>
		<audio style="text-align: left" :src="current.src" :poster="current.poster" :name="current.name" :author="current.author" :action="audioAction" controls></audio>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				current: {
					poster: 'https://qiniu-web-assets.dcloud.net.cn/unidoc/zh/music-a.png',
					name: '致爱丽丝',
					author: '暂无',
					src: 'https://bjetxgzv.cdn.bspapp.com/VKCEYUGU-hello-uniapp/2cc220e0-c27a-11ea-9dfb-6da8e309e0d8.mp3',
				},
				audioAction: {
					method: 'pause'
				}
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
