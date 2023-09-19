<!-- 
@ 代表事件，vue的语法 
 -->
<template>
	<view>
		<button type="default">按钮</button>
		<label>
			<checkbox value="cb"  checked="true"/><text>选中</text>
		</label>
		<editor placeholder="富文本编辑器"></editor>
		
		<text>复选框</text>
		<checkbox-group name="" @change="chChange">
			<label>
				<checkbox value="php" /><text>php</text>
			</label>
			<label>
				<checkbox value="java" /><text>java</text>
			</label>
			<label>
				<checkbox value="golang" /><text>golang</text>
			</label>
		</checkbox-group>
		
		<form @submit="" @reset="">
			<text>用户名:{{username}}</text>
			<input type="text" @input="input1" value="" />
			<button form-type="submit">Submit</button>
			<button type="default" form-type="reset">Reset</button>
		</form>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				username: ''
			}
		},
		methods: {
			input1:function(e){
				this.username = e.detail.value
			},
			chChange:function(e){
				console.log(e.detail.value)
			}
		}
	}
</script>

<style>
	input {
		background-color: gray;
	}
</style>
