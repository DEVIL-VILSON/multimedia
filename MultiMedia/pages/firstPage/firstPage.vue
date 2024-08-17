<template>
	<view >
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
				<text class="welcm">欢迎</text>
			</view>
			<view class="book">
				<image src="/static/illustration 5@2x.png" mode="" class="bookimg"></image>
			</view>
		</view>
		<swiper class="SWtab" :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000" >
			<swiper-item class="intab">
				<view class="swiper-item"></view>
			</swiper-item>
			<swiper-item class="intab">
				<view class="swiper-item"></view>
			</swiper-item>
		</swiper>
		<view class="tx">
			<text class="welcm">安全学习</text>
			<hr style="width: 28%; margin-left: 50rpx; color: #8C6FE5; border: 1px solid #8C6FE5; background: #8C6FE5"/>
			
		</view>
		<scroll-view class="SCtab" scroll-y="true" >
			<view class="store" v-for="item in 10" :key="item">
				<view class="storeimg" >
					<image src="" mode=""></image>
				</view>
				<view class="title">
					<text>1111111111</text>
					<br/>
					<text>2222222</text>
					
				</view>
				<view class="into">
					<image src="/static/Arrow Icon@2x.png" mode=""></image>
				</view>
			</view>
			
		</scroll-view>
		<view class="Kbutton">
			一键打卡
		</view>
		<view class="grass">
			
		</view>
	</view>
</template>

<script setup>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
		
		},
		mounted() {
			// uni.showToast({
				
			// })
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
	.book{
		position: absolute;
		left: 130rpx;
		top: 55rpx;
		.bookimg{
			width: 210rpx;
			height: 115rpx;
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
}
.SWtab{
	width: 746rpx;
	height: 340rpx;
	// border: 1rpx solid rgba(116, 76, 235, .4);
	margin-top: 20rpx ;
	.swiper-item{
		width: 75%;
		height: 254rpx;
		display: flex;
		justify-content: center;
		border: 10rpx solid rgba(116, 76, 235, .4);
		margin: 0 auto;
		margin-top: 24rpx;
		border-radius: 24rpx;
	}
}
.SCtab{
	width: 746rpx;
	height: 520rpx;
	// border: 1rpx solid rgba(116, 76, 235, .4);
}
.tx{
	padding: 20rpx;
	.welcm{
		font-size: 40rpx;
	}
}
.store{
	width: 640rpx;
	height: 120rpx;
	margin-left: 50rpx;
	margin-top: 24rpx;
	padding-top: 24rpx;
	border-radius: 20rpx;
	box-shadow: 0 0 4px rgba(0, 0, 0, 0.2);
	position: relative;
	.storeimg{
		width: 90rpx;
		height: 90rpx;
		border: 20rpx;
		margin-left: 30rpx;
		border-radius: 12rpx;
		box-shadow: 0 0 4px rgba(0, 0, 0, 0.2);
	}
	.title{
		position: absolute;
		left: 160rpx;
		top: 24rpx;
		
	}
	.into{
		position: relative;
		left: -25rpx;
		top: -56rpx;
			float: right;
			image{
				height: 40rpx;
				width: 40rpx;
			}
		}
}
.Kbutton{

	background-color: #8C6FE5;
	position: relative;
	left: 40rpx;
	top: -100rpx;
	border-radius: 35rpx;
	width: 180rpx;
	height: 60rpx;
	padding-top: 18rpx;
	text-align: center;
	font-size: 24rpx;
	
}
.grass{
	background-image: url("/static/illustration 1@1x.png");
	 background-position: 20% 30%;
}
</style>
