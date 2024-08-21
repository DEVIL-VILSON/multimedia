<template>
  <view class="all">
	  <image src="../../static/bg.png" style="height: 1250rpx; width: 750rpx; z-index: -10;position: absolute;"></image>
	  <view class="dialog">
	    <view class="dialog-container">
	      <view v-for="(message, index) in messages" :key="index" class="message">
	             <view class="message-content">{{ message }}</view>
				  <image class="avatar" src="/static/Ellipse1@2x.png"  style="height: 80rpx;width: 80rpx;"/>
	            </view>
	    </view>
	  	<view class="input-container">
	      <input v-model.lazy="inputMessage" @confirm="addMessage" type="text" placeholder="   输入消息并按回车发送"  class="input">
	    </view>
	  </view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      inputMessage: '',
      messages: []
    };
  },
  methods: {
    addMessage() {
      if (this.inputMessage.trim() !== '') {
        this.messages.push(this.inputMessage);
        this.inputMessage = '';
      }
    }
  },
  
};
</script>

<style lang="scss">
	.all{
	height: 1250rpx; 
	width: 750rpx;
		
		.dialog{
				position: relative;
				height: 1000rpx;
				width: 620rpx;
				background-color: #FDFCFD;
				top: 100rpx;
				left: 70rpx ;
				border-radius: 20rpx;
			}
			
		.input-container {
		  margin: 10px;
		  width: 500rpx;
		  height: 50rpx;
		  position: fixed;
		  top: 1100rpx;
		  background-color: #F2F2F2;
		  border-radius: 20rpx;
		  font-size: 30rpx;
		  font-weight: 600;
		  box-shadow: 0rpx 10rpx 10rpx #D8D8D8;
		}
		
		.dialog-container {
			display: flex;
			flex-direction: column;
		  margin: 10rpx;
		  padding: 10rpx;
		  width: 520rpx;
		}
		
		.message{
			display: flex;
			flex-direction: row;
			width: 550rpx;
			
			.message-content {
				width: 480rpx;
			  background-color: #fff;
			  padding: 10rpx;
			  margin:15rpx 0 5rpx 0;
			  border-radius: 10px;
			  word-break: break-all;
			  box-shadow: 0rpx 10rpx 10rpx #D8D8D8;
			}
			.avatar{
				margin: 0 0 0 50rpx;
			}
		}
	}
</style>