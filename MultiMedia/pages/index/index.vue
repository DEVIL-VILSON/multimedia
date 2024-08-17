<template>
	<view>
		<view class="doctop">
			<button style="height: 1246rpx; width: 100%; background-color: rgba(0, 0, 0, 0);" @click="showBottomWindow = false"></button>
		</view>
		<button class="open" @click="showBottomWindow = true" ></button>
		<view v-show="showBottomWindow" class="bottom-window">
		  <!-- 底部窗口内容 -->
		  <view class="intop" >
		  	<view class="topline"></view>
		  </view>
		  
		  <view class="rowscroll" >
		  	<scroll-view class="scroll-view_H" scroll-x="true" @scroll="scroll" scroll-left="0">
		  		<view  class="scrollitem"  v-for="(item,index) in 10" :key="index" :class=" [index  == atv1 ?'active1':'active-1'] " @click="getindex1(index)">{{index + 1}}</view>
				<view class="docbody">
				<text class="docqus">1.111111111111111</text>
				<view class="doctext" v-for="(item,ind) in 4" :key="ind" >
					<view class="docchoose" :key="ind" @click="getindex2(ind)" :class=" [ind == act2 ? 'active2':'active-1'] ">
						{{ind +1}}
					</view>
					<text class="docanswer" @click="getindex2(ind)" :class=" [ind == act2 ? 'active3':'active-3'] ">11111111111222222222</text>
				</view>
			</view>
		  	</scroll-view>
			
			<view class="finish">
					<button class="Fbtn">完成问卷</button>
					<image src="../../static/oc-taking-note@2x.png" mode=""></image>
				</view>
		  </view>
		</view>
	</view>
</template>

<script >
	export default {
		data() {
			return {
				showBottomWindow: false,
				atv1: 0,
				act2: -1,
				
			}
		},
		methods: {
			scroll: function(e) {
				console.log(e)
				this.old.scrollTop = e.detail.scrollTop
		    },
			getindex1(index){
                this.atv1 = index
				
			},
			getindex2(ind){
			    this.act2 = ind
				console.log(this.act2)
			}
		}
	}
</script>

<style lang="scss" >
.doctop{
	height: 180rpx;
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
  .intop{
	padding-top: 30rpx;
  	// border: 1rpx solid #8C6FE5;
  	.topline{
  		width: 120rpx ;
  		height: 8rpx;
		margin-left: 300rpx;
  		border:1rpx solid #7D48EA;
  		border-radius:6rpx ;
  		background-color: #7D48EA;
  		// background-image: repeating-linear-gradient(to bottom, #7d48eb, #DDD2F4 , 100%);
  	}
  }
  .rowscroll{
	  height: 120rpx;
	  .scroll-view_H {
	  		white-space: nowrap;
	  		width: 100%;
			.scrollitem{
				 height: 50rpx;
				 width: 60rpx;
				 // border: 1rpx solid #8C6FE5;
				 
				 display: inline-block;
				 text-align: center;
				 border-radius: 30rpx;
				 margin: 30rpx 20rpx;
				 padding-top: 10rpx;
			 }
	  	}
	    .finish{
			height: 240rpx;
			
	    	.Fbtn{
				position: relative;
				left: -120rpx;
	    		height: 80rpx;
				width: 320rpx;
				border-radius: 30rpx;
				box-shadow: 0 10rpx 4px rgba(0, 0, 0, 0.1);
				background-color: #fff;
				font-size: 32rpx;
				color: #7D48EA;
	    	}
			image{
				position: relative;
				left: 430rpx;
				top: -180rpx;
				height: 360rpx;
				width: 380rpx;
			}
	    }
  }
}
.docbody{
	height: 700rpx;
	padding-left: 45rpx;
	// border: 1rpx solid #8C6FE5;
	.docqus{
		display: inline-block;
		height: 80rpx;
	}
	.doctext{
		margin: 20rpx 20rpx;
		display: flex;
		flex-direction: row;
		.docchoose{
			height: 60rpx;
			width: 80rpx;
			border-radius: 40rpx;
			text-align: center;
			// background-color: #D4D4D4;
			color: #fff;
			padding-top: 20rpx;
		}
		.docanswer{
			word-break: break-all;
			display: inline-block;
			margin-left: 30rpx;
		    height: 80rpx;
		    width: 500rpx;
		    // border: 1rpx solid #8C6FE5;
	    }
	}
}
.open{
	border-radius: 24rpx;
	background-color: #7D48EA;
	height: 100rpx;
}
.active1{
	background-color: #7D48EA;
}
.active-1{
	background-color: #D4D4D4;
}
.active2{
	background-color: #8C6FE5;
}
.active3{
	color: #8C6FE5;
}
.active-3{
	color: #000;
}
</style>
