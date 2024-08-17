<template>
	<view style="background-color: rgba(216, 216, 216, 0.3); border-radius: 10rpx;">
			<view class="usertop">
				<view class="Imguser">
					<image src="../../static/Ellipse1@2x.png" mode="" class="img1"></image>
					<text>小明</text>
					<image src="/static/plant-2@2x.png" mode="" class="img2"></image>
					<image src="/static/plant-1@2x.png" mode="" class="img3"></image>
				</view>
				<button class="changeUser"><text>编辑资料</text></button>
			</view>
			<view class="usertab" >
				<view class=" inusertab" v-for="item in 9">
					<image src="/static/copy@2x.png" mode=""></image>
					<view class=" tabtext">
						<text>学习学习</text>
					</view>
				</view>
			</view>
			<view class="othertab" >
				<view class="othertip" v-for="item in 4">
					<image src="/static/copy@2x.png" mode=""></image>
					<view class="tiptext">
						<text>1111111</text>
					</view>
					<view class="tipright">
						>
					</view>
				</view>
			</view>
			<view class="kb" style="height: 292rpx;">
				<image src="/static/illustration 4@2x.png" mode="" class="kbimg"></image>
			</view>
			<view class="buttontab">
				<view class="kbbutton" v-for="item in 4">
					
				</view>
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
	
	<style lang="scss">
	
	.usertop{
		height: 150rpx;
		width: 740rpx;
		padding-left: 30rpx;
		// border: 1px solid #8C6FE5;
		background-color: #fff;
		display: flex;
		flex-direction: row;
		justify-content: space-around;
		align-items: center;
		.Imguser{
			height: 88rpx;
			width: 88rpx;
			margin-right: 300rpx;
			// border: 1px solid #8C6FE5;
			.img1{
				height: 88rpx; 
				width: 88rpx;
				z-index: 1;
			}
			.img2{
				height: 110rpx;
				width: 60rpx;
				position: relative;
				left: -30rpx;
				top: -130rpx;
				z-index: 0;
			}
			.img3{
				height: 80rpx;
				width: 40rpx;
				left: 20rpx;
				top: -219rpx;
				z-index: 0;
				position: relative;
			}
			text{
				text-align: center;
				position: relative;
				font-size: 20rpx;
				left: 120rpx;
				top: -72rpx;
			}
		}
		.changeUser{
			background-color: #8C6FE5;
			width: 160rpx;
			height: 60rpx;
			border-radius: 40rpx;
			font-size:20rpx;
			color: #fff;
			
		}
	}
	.usertab{
		margin: 50rpx 0;
		height: 260rpx;
		width: 746rpx;
		.inusertab{
			background-color: #fff;
			display: inline-block;
			height: 114rpx;
			width: 140rpx;
			margin-left: 8rpx;
			box-shadow: 0 0 4px rgba(0, 0, 0, 0.2);
			// border: 2px solid #8C6FE5;
			border-radius: 16rpx;
			margin-bottom: 8rpx;
			padding-top: 16rpx;
			// padding-left: 30rpx;
			image{
				margin-left: 35rpx;
				height: 70rpx;
				width: 70rpx;
			}
			.tabtext{
				text-align: center;
				// border: 2px solid #8C6FE5;
				height: 16rpx;
				font-size: 12rpx;
			}
		}
	}
	.othertab{
		background-color: #fff;
		height:330rpx;
		.othertip{
			height: 80rpx;
			// border: 1px solid #8C6FE5;
			image{
				margin-left: 12rpx;
				margin-top: 10rpx;
				height: 60rpx;
				width: 60rpx;
			}
			.tiptext{
				width: 240rpx;
				height: 50rpx;
				font-size: 24rpx;
				// border: 1rpx solid #8C6FE5;
				position: relative;
				left: 100rpx;
				top: -65rpx;
				text{
					position: absolute;
					top: 50%;
					left: 30%;
					color: #000000;
					transform: translate(-50%, -50%);
					text-align: center;
				}
			}
			.tipright{
				height: 30rpx;
				width: 30rpx;
				color: #C9C9C9;
				position: relative;
				left: 650rpx;
				top: -110rpx;
			}
		}
	}
	.kb{
		.kbimg{
			position: relative;
			left: 300rpx;
			top: -80rpx;
			height: 300rpx;
			width: 350rpx;
		}
	}
	.buttontab{
		height: 100rpx; 
		background-color: #fff;
		.kbbutton{
			display: inline-block;
			border: 1rpx solid #8C6FE5;
			height: 100rpx;
			width: 182rpx;
		}
	}
	</style>
	