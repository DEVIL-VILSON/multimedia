<template>
	<view>
		<view class="doctop">
			<button style="height: 1246rpx; width: 100%; background-color: rgba(0, 0, 0, 0);" @click="showBottomWindow = false"></button>
		</view>
		<button class="open" @click="showBottomWindow = true" ></button>
		<view v-show="showBottomWindow" class="bottom-window">
		  <!-- 底部窗口内容 -->
		  
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				showBottomWindow: false
			}
		},
		methods: {
			
		}
	}
</script>

<style>
.doctop{
	height: 160rpx;
	background-image: repeating-linear-gradient(to bottom, #7D48EA, #ffffff 100%);

}
.bottom-window {
  position: fixed;
  bottom: 0;
  left: 0;
  height: 1100rpx;
  width: 100%;
  background-color: #fff;
  border-radius: 20px 20px 0 0;;
  border-top: 1px solid #ddd;
  background-color: antiquewhite;
}
.open{
	background-color: #7D48EA;
	height: 100rpx;
}
</style>
