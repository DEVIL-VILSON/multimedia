<template>
	<view>
		<view class="top">
			<view class="tab">
				<image src="/static/Frame6@2x.png" alt="" class="tabimg"  @click=""></image>
			</view>
			<view class="box1">
				<view class="box2">
					<view class="box3">
						<view class="box4">
							<view class="user">
							    <image src="/static/Ellipse1@2x.png" mode="" class="userimg"></image>
						    </view>
						</view>						
					</view>
				</view>
			</view>
			<view class="tx">
				<text class="welcm">消防安全</text>
				<view class="line1"></view>
				<view class="line2"></view>
				<text class="tx_text">防火从心开始，安全伴我行</text>
				<view class="line3"></view>
			</view>
		</view>
		<view class="mid">
			<view class="mid_left">
				<view class="left_up"><image src="/static/ar.png" style="height: 320rpx;
				width: 350rpx;"></image></view>
				<view class="left_down"><image src="/static/question.png" style="height: 240rpx;
				width: 300rpx;"></image></view>
			</view>
			<view class="mid_right">
				<view class="right_up"><image src="/static/video.png" style="height: 240rpx;
				width: 300rpx;"></image></view>
				<view class="right_down"><image src="/static/safe.png" style="height: 320rpx;
				width: 350rpx;"></image></view>
			</view>
		</view>
		<view class="bottom">
			<view class="bottom_title">今日新鲜学</view>
			<view class="bottom_context">
				<view class="context">
					<view class="context_line"></view>
					<view class="context_main">
						<view class="main_title">问卷：火灾预防？</view>
						<view class="main_time">35min</view>
						<view class="main_label">
							<view class="label1">火灾预防</view>
							<view class="label1">初中</view>
						</view>
					</view>
					<view class="context_point"><image src="../../static/point.png" style="height: 20rpx; width: 5rpx;"></image></view>
				</view>
				<view class="context">
					<view class="context_line"></view>
					<view class="context_main">
						<view class="main_title">视频</view>
						<view class="main_time">1hour25min</view>
						<view class="main_label">
							<view class="label1">楼层防火</view>
							<view class="label1">初中</view>
						</view>
					</view>
					<video class="context_video" src="/static/firesafety.mp4" style="height: 150rpx; width: 250rpx; border-radius: 20rpx;"></video>
					<view class="context_point2"><image src="../../static/point.png" style="height: 20rpx; width: 5rpx;"></image></view>
				</view>
				<view class="context">
					<view class="context_line"></view>
					<view class="context_main">
						<view class="main_title">问卷：火灾中如何安全逃生</view>
						<view class="main_time">35min</view>
						<view class="main_label">
							<view class="label1">逃生</view>
							<view class="label1">初中</view>
						</view>
					</view>
					<view class="context_point"><image src="../../static/point.png" style="height: 20rpx; width: 5rpx;"></image></view>
				</view>
			</view>
			
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss">
	.top{
		height: 180rpx;
		// border: 1px solid #000;
		position: relative;
		.tab{
			width: 40rpx;
			height: 40rpx;
			padding-left: 40rpx;
			padding-top: 40rpx;
			// background-color: #5f5f5f;
			.tabimg{
				height: 100%;
				width: 100%;
			}
		}
		
		.box1{
			width: 278rpx;
			height: 278rpx;
			border: 1rpx solid rgba(121, 76, 235, .05);
			border-radius: 139rpx;
			display: flex;
			justify-content: center;
			align-items: center;
			position: absolute;
			left: 500rpx;
			top: -70rpx;
			.box2{
				width: 239rpx;
				height: 239rpx;
				border: 1rpx solid rgba(110, 76, 235, .1);
				border-radius: 120rpx;
				display: flex;
				justify-content: center;
				align-items: center;
				.box3{
					width: 187rpx;
					height: 187rpx;
					border: 1rpx solid rgba(140, 76, 235, .2);
					border-radius: 93rpx;
					display: flex;
					justify-content: center;
					align-items: center;
					.box4{
						width: 139rpx;
						height: 139rpx;
						border: 1rpx solid rgba(129, 76, 235, .3);
						border-radius: 68rpx;
						display: flex;
						justify-content: center;
						align-items: center;
						.user{
							width: 77rpx;
							height: 77rpx;
							border: 1rpx solid rgba(116, 76, 235, .4);
							border-radius: 38rpx;
							display: flex;
							justify-content: center;
							align-items: center;
							.userimg{
								width: 60rpx;
								height: 60rpx;
								display: flex;
								justify-content: center;
								align-items: center;
						}
				    }
				}
			}
		}
	}
	.tx{
		margin: 30rpx 0 0 40rpx;
		
		
		.welcm{
			font-size: 40rpx;
		}
		.line1{
			height: 2rpx;
			width: 130rpx;
			background-color: rgba(110, 76, 215, 0.7);
			margin: 0 0 0 -20rpx;
		}
		.line2{
			height: 2rpx;
			width: 250rpx;
			background-color: rgba(110, 76, 235, 0.7);
			margin: 10rpx 0 0 40rpx;
		}
		.tx_text{
			font-size: 25rpx;
			margin: 20rpx 0 0 0;
		}
		.line3{
			height: 3rpx;
			width: 160rpx;
			background-color: rgba(45, 7, 184, 1);
			margin: 5rpx 0 0 -20rpx;
		}
	}}
	.mid{
		display: flex;
		
		.mid_left{
			display: flex;
			flex-direction: column;
			.left_up{
				display: flex;
				margin: 60rpx 0 0 15rpx;
				}
			.left_down{
				display: flex;
				margin: 30rpx 0 0 15rpx;
					}
				}
		.mid_right{
				display: flex;
				flex-direction: column;
				margin: 60rpx 0 0 20rpx;
				.right_up{
					display: flex;
					
				}
				.right_down{
					display: flex;
					margin: 30rpx 0 0 0;
				}
			}
		}
		
		.bottom{
			display: flex;
			flex-direction: column;
			
			.bottom_title{
				font-size: 45rpx;
				margin: 20rpx 0 0 30rpx;
				
			}
			.bottom_context{
				display: flex;
				flex-direction: column;
				
				.context{
					display: flex;
					flex-direction: row;
					width: 700rpx;
					height: 230rpx;
					background-color: #F9FAFD;
					border-radius: 30rpx;
					margin: 20rpx 0 0 25rpx;
					.context_video{
						margin: 30rpx 0 0 -100rpx;
					}
					
					.context_line{
						height: 80rpx;
						width: 5rpx;
						background-color: #8F99EB;
						border-radius: 5rpx;
						margin: 30rpx 0 0 30rpx;
					}
					.context_main{
						display: flex;
						flex-direction: column;
						margin: 30rpx 0 0 20rpx;
						width: 400rpx;
						.main_title{
							font-size: 30rpx;
						}
						.main_time{
							font-size: 25rpx;
							color: #9AA8C7;
							margin: 25rpx 0 0 0;
						}
						.main_label{
							display: flex;
							flex-direction: row;
							font-size: 23rpx;
							color: #8F99EB;
							margin: 35rpx 0 0 0;
						}
						.label1{
							height: 40rpx;
							width: 120rpx;
							background-color: rgba(143, 153, 235, 0.2);
							border-radius: 10rpx;
							text-align: center;
							margin: 0 20rpx 0 0;
						}
					}
					.context_point{
						position: relative;
						top: 25rpx;
						left: 200rpx;
					}
					.context_point2{
						position: relative;
						top: 25rpx;
						left: 55rpx;
					}
				}
			}
		}
	

</style>
	
