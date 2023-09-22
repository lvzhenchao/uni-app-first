<template>
	<view>
		<button type="primary" @click="uploadImg">选择图片</button>
		<text>{{url}}</text>
		<img :src="url" mode="aspectFill" alt="">
	</view>
	
</template>

<script>
	export default {
		data() {
			return {
				url: '',
			}
		},
		methods: {
			uploadImg:function(){
				var that = this
				//第一种
				uni.chooseImage({
					success:function(res){
						console.log(res)
						that.url = res.tempFilePaths
						//预览
						uni.previewImage({
							urls:res.tempFilePaths
						})
						//获取图片信息,直接出来
						uni.getImageInfo({
							src: res.tempFilePaths
						})
						//保存到本地
						uni.saveImageToPhotosAlbum({
							filePath:res.tempFilePaths,
							success:function(){
								console.log("保存成功")
							}
						})
					}
				})
				//第二种：不好使
				// uni.chooseImage({
				// 	success: (chooseImageRes) => {
				// 		const tempFilePaths = chooseImageRes.tempFilePaths;
				// 		uni.uploadFile({
				// 			url: 'https://www.example.com/upload', //仅为示例，非真实的接口地址
				// 			filePath: tempFilePaths[0],
				// 			name: 'file',
				// 			formData: {
				// 				'user': 'test'
				// 			},
				// 			success: (uploadFileRes) => {
				// 				console.log(uploadFileRes.data);
				// 				that.url = res.tempFilePaths[0]
				// 			}
				// 		});
				// 	}
				// });
			}
		}
	}
</script>

<style>

</style>
