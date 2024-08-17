<template>
	<view class="bcimg">
		<view class="kongbai" style="height: 300rpx;">
			<button style="height: 1246rpx; width: 100%; background-color: rgba(0, 0, 0, 0);" @click="showBottomWindow = false"></button>
		</view>
		<view class="" style="height: 500rpx; " >
			<view class="dengluimg">
			    <image src="/static/illustration 3@2x.png" mode="" style="height: 460rpx; width: 400rpx;"></image>
			</view>
		</view>
		<button class="denglu" @click="showBottomWindow = true">
			<image src="/static/注册@2x.png" mode="" style="height: 32rpx; width: 180rpx;"></image>
		</button>
		<button class="denglu" @click="showBottomWindow = true">
			<image src="/static/注册@2x(1).png" mode="" style="height: 32rpx; width: 180rpx;"></image>
		</button>
		<view class="" style="height: 176rpx;">
			
		</view>
		<view v-show="showBottomWindow" class="bottom-window">
		  <!-- 底部窗口内容 -->
		  <view class="box boximg" style="margin: 0 auto;width: 100%; height: 210rpx; ">
		  	<view class="" style="margin: 0 auto; width: 200rpx; height: 200rpx; padding-top: 100rpx;">
		  		<image src="/static/手机号登录@2x.png" mode="" style="height: 36rpx; width: 160rpx; "></image>
		  	</view>
		  </view>
		  <view class="" style="margin: 0 auto ; width: 100%; height: 500rpx; " >
			<view class="" style=" margin: 0 auto ; width:450rpx;">
				<text style="font-size: 12rpx; color: #D8D8D8;">手机号</text>
				<view class="box11" style="">
					<input type="text" class="puttext"/>			
				</view>
				<text style="font-size: 12rpx; color: #D8D8D8;">验证码</text>
				<view class="box22">
					<input type="text" class="puttext"/><text class="get" style="font-size: 8rpx;">获取验证码</text>
				</view>
			</view>
			<navigator url="/pages/firstPage/firstPage">
				<button class="box33"><img src="/static/立即登录@2x.png" alt="" style="height: 24rpx; width: 120rpx;"/></button>
			</navigator>
			
		  </view>
		  
		  <view class="" style="height: 220rpx;">
			<view class="otherway">
				<hr class="HRcss"/>
			<text style="font-size: 12rpx; color: #D8D8D8;">其他方式登录</text>
			<hr class="HRcss"/>
			</view>
			<view class="otherway">
				<view class="qinbox">
					<image src="/static/wechat-fill@2x.png" mode="" style="height: 40rpx; width: 40rpx;"></image>
				</view>
				<view class="qinbox" >
					<image src="/static/qq-fill@2x.png" mode="" style="height: 40rpx; width: 40rpx;"></image>
				</view>
			</view>	
		  </view>
			
		  <!-- </view> -->
		  <!-- <button @click="showBottomWindow = false">隐藏底部窗口</button> -->
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
.dengluimg{
	margin-left: 160rpx;;
	height: 350rpx;
	width: 250rpx;
		
}
.denglu{
	width: 500rpx;
	height: 90rpx;
	border-radius: 30rpx;
	background-color: #fff;
	margin: 30rpx auto;
	padding-top: 2rpx;
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
.bottom-window {
  position: fixed;
  bottom: 0;
  left: 0;
  height: 940rpx;
  width: 100%;
  background-color: #fff;
  border-radius: 20px 20px 0 0;;
  border-top: 1px solid #ddd;
}
.boximg{
	background-image: url("/static/oc-on-the-laptop@2x.png");
	background-size: 240rpx;
	background-repeat: no-repeat;
	background-position: 480rpx 20rpx;
}

.box11{
	border-radius: 20rpx;
	height: 60rpx;
	padding-left: 60rpx;
	margin: 20rpx 0;
	border: 1rpx solid rgba(116, 76, 235, .4);
	background-image: url("/static/user@2x.png");
	background-size: 28rpx;
	background-repeat: no-repeat;
	background-position: 16rpx 12rpx;
}
.box22{
	border-radius: 20rpx;
	height: 60rpx;
	padding-left: 60rpx; 
	margin: 20rpx 0;
	border: 1rpx solid rgba(116, 76, 235, .4);
	background-image: url("/static/mail-send-fill@2x.png");
	background-size: 28rpx;
	background-repeat: no-repeat;
	background-position: 16rpx 12rpx;
	
}
.box33{
	border-radius: 30rpx;
	height: 90rpx;
	width: 520rpx;
	margin: 0 auto;
	margin-top: 80rpx;
	box-shadow: -2rpx 6rpx 12px rgba(10, 10, 10, 0.2);
	background-image: url("/static/illustration 1@1x.png");
	background-size: 34rpx;
	background-repeat: no-repeat;
	background-position: 350rpx 12rpx;
}
.puttext{
	font-size: 24rpx;
	display: inline-block;
	margin: 12rpx 0;
	width: 220rpx;
}
.get{
	margin-top: 12rpx;
	margin-right: 8rpx;
	color: rgba(116, 96, 235, .8);
	float: right;
}
.otherway{
	display: flex;
	margin-top: 40rpx;
	flex-direction: row;
	justify-content: space-evenly;
	align-items: center;
	/* border: 1rpx solid rgba(116, 76, 235, .4); */
}
.qinbox{
	height: 60rpx; 
	width: 60rpx;
	/* border: 1rpx solid rgba(116, 76, 235, .4); */
}
	
.HRcss{
	width:160rpx ;
	border: 1px solid #D8D8D8;
	background: #D8D8D8;
}
</style>
