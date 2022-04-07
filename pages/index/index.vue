<template>
	<view>
		<view class="top"></view>
		<view class="xiugou" v-show="show">
			<p>你好！我是I陪伴小助手!</p>
		</view>
		<image class="aixin" v-show="show" src="../../static/icons/xin.png" @click="sgo()">
		<image class="gouzi" src="../../static/icons/xiugou.png" @click="sgo()">
		<view class="swiper-c">
			<swiper indicator-dots="true" autoplay="autoplay" interval="1000" duration="500">
				<swiper-item>
					<image src="../../static/picture/ppp1.png"></image>
				</swiper-item>
				<swiper-item>
					<image src="../../static/picture/ppp2.png"></image>
				</swiper-item>
				<swiper-item>
					<image src="../../static/picture/ppp3.png"></image>
				</swiper-item>
				<swiper-item>
					<image src="../../static/picture/ppp4.png"></image>
				</swiper-item>
				<swiper-item>
					<image src="../../static/picture/ppp5.png"></image>
				</swiper-item>
			</swiper>
		</view>
		<view class="items">
			<view class="item">
				<image src="../../static/icons/fi1.png"></image>
				<p>会员</p>
			</view>
			<view class="item">
				<image src="../../static/icons/fi2.png"></image>
				<p>活动</p>
			</view>
			<view class="item">
				<image src="../../static/icons/fi3.png"></image>
				<p>附近</p>
			</view>
			<view class="item">
				<image src="../../static/icons/fi4.png"></image>
				<p>冠军</p>
			</view>
			<view class="item">
				<image src="../../static/icons/fi5.png"></image>
				<p>积分</p>
			</view>
			<view class="item">
				<image src="../../static/icons/fi6.png"></image>
				<p>评论</p>
			</view>
			<view class="item">
				<image src="../../static/icons/fi7.png"></image>
				<p>运动</p>
			</view>
			<view class="item">
				<image src="../../static/icons/fi8.png"></image>
				<p>生活休闲</p>
			</view>
		</view>
		<view class="someting">
			<image src="../../static/picture/tu1.png"></image>
			<p>心理学：三位老人，你认为哪一位最慈祥？</p>
			<p class="jia"></p>
		</view>
		<view class="someting">
			<image src="../../static/picture/tu2.png"></image>
			<p>老年人养生有讲究，这4个“慢”要做好，很有帮助！</p>
			<p class="jia"></p>
		</view>
		<view class="someting">
			<image src="../../static/picture/tu3.png"></image>
			<p>小人物 | 被智能手机“抛弃”的老年人</p>
			<p class="jia"></p>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				show: true
			}
		},
		onLoad() {
			uni.navigateTo({
				url:"../wj/wj"
			})
		},
		methods: {
			sgo(){
				this.show = !this.show;
			}
		}
	}
</script>

<style>
	.top {
		height: var(--status-bar-height);
		width: 100%;
		background-color: #FFFFFF;
	}
	.xiugou{
		position: fixed;
		z-index: 500;
		left: 25rpx;
		top: 700rpx;
		width: 700rpx;
		height: 300rpx;
		border-radius: 30rpx;
		background: #FFD700;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: cneter;
	}
	.xiugou p{
		font-size: 100rpx;
		width: 650rpx;
		margin-left: 30rpx;
	}
	.gouzi{
		position: fixed;
		z-index: 500;
		left: 5rpx;
		top: 1000rpx;
		width: 260rpx;
		height: 210rpx;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: cneter;
	}
	.aixin{
		position: fixed;
		z-index: 500;
		left: 200rpx;
		top: 1000rpx;
		width: 100rpx;
		height: 100rpx;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: cneter;
	}
	.swiper-c{
		width: 100%;
		height: 450rpx;
	}
	.swiper-c swiper{
		width: 100%;
		height: 100%;
	}
	.swiper-c swiper swiper-item image{
		width: 100%;
		height: 100%;
	}
	.items{
		flex-wrap: wrap;
		width: 100%;
		height: 360rpx;
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
	}
	.item{
		width: 180rpx;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.item image{
		width: 80rpx;
		height: 80rpx;
	}
	.item p{
		font-size: 40rpx;
		color: #555555;
	}
	.someting{
		position: relative;
		width: 100%;
		height: 180rpx;
		border-bottom: #000000 solid 1rpx;
	}
	.someting image{
		width: 150rpx;
		height: 150rpx;
		margin-top: 15rpx;
		margin-left: 15rpx;
	}
	.someting p{
		position: absolute;
		top: 35rpx;
		left: 180rpx;
		font-size: 40rpx;
		width: 580rpx;
		height: 50rpx;
	}
	.someting .jia{
		position: absolute;
		width: 580rpx;
		height: 50rpx;
		font-size: 40rpx;
		top: 60rpx;
		color: gold;
		left: 580rpx;
	}
</style>
