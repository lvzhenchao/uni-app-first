<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')//第一次打开的时候
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		},
		globalData:{
			name: "lzc"
		}
	}
</script>

<style>
	/*每个页面公共css */
	/* .title{
		color: blue;
	} */
</style>
