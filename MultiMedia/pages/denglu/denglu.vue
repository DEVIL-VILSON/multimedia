<template>
	<view class="bcimg">
		<view class="kongbai" style="height: 350rpx;">
			
		</view>
		<view class="" style="height: 500rpx; " >
			<view class="dengluimg">
			    <image src="/static/illustration 2@1x.png" mode="" style="height: 320rpx; width: 280rpx;"></image>
			</view>
			<view class="" style="padding-top: 30rpx;">
				<image src="/static/lockdown can't stop your learn@1x.png" mode="" style="height: 100rpx; width: 300rpx; margin-left: 230rpx;"></image>
			</view>
		</view>
		<navigator url="/pages/dlpage/dlpage">
			<button class="denglu" >
			    <image src="/static/Frame 118@1x.png" mode="" style="height: 60rpx; width: 160rpx;"></image>
		    </button>
		</navigator>
		
		<view class="" style="height: 256rpx;">
			
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
			
		}
	}
</script>

<style>
	
.dengluimg{
	margin: 0 auto;
	height: 350rpx;
	width: 250rpx;
	
}
.denglu{
	width: 500rpx;
	height: 100rpx;
	border-radius: 30rpx;
	background-color: pink;
	margin: 20rpx auto;
	padding-top: 20rpx;
}
.bcimg{
	background-image: url('/static/Photo@1x(1).jpg');
	/* background-image: url('/static/Blur@2x(1).png'); */
	background-size: cover;
	border-radius: 12rpx;
}
.bcimg::before{
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url('/static/Blur@1x (1).png');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  z-index: 0; /* important! */
}
</style>
