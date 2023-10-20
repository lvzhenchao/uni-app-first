<!-- 
快捷键：ut
文本输入,文本只能写在text中，而不能写在view的text区域
变量前添加冒号代表变量，也可以不加冒号，直接赋值即可
 -->
<template>
	<text> lzc </text>
	<rich-text :nodes="html_s"></rich-text>
	<icon :type="iconType" size="20" color="red"/>
	<progress percent="20" stroke-width="10" show-info active-color="green" active="true"/>
</template>

<script>
	export default {
		data() {
			return {
				// html_s: "<h1>hello world fuck</h1>",
				iconType: ['success']
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
