<template>
	<view>
		<view class="top"></view>
		<view class="bg"></view>
		<view class="name">
			<image src="../../static/icons/tx.png"></image>
			<p class="p1">六道轮回</p>
			<p class="p2">Ta很蓝，什么都没留下</p>
		</view>
		<view class="items">
			<view class="item">
				<image src="../../static/icons/ss1.png"></image>
				<p class="xin">我的信息</p>
				<p class="zuo">></p>
			</view>
			<view class="item">
				<image src="../../static/icons/ss2.png"></image>
				<p class="xin">我的评价</p>
				<p class="zuo">></p>
			</view>
			<view class="item">
				<image src="../../static/icons/ss3.png"></image>
				<p class="xin">我的收藏</p>
				<p class="zuo">></p>
			</view>
			<view class="item">
				<image src="../../static/icons/ss4.png"></image>
				<p class="xin">关于</p>
				<p class="zuo">></p>
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

<style>
	.top {
		height: var(--status-bar-height);
		width: 100%;
		background-color: #FFFFFF;
	}
	.bg{
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 400rpx;
		background: linear-gradient(blue, pink);
	}
	.name{
		position: absolute;
		width: 100%;
		height: 200rpx;
		top: 120rpx;
	}
	.name image{
		width: 150rpx;
		height: 150rpx;
		border-radius: 75rpx;
		margin-top: 30rpx;
		margin-left: 30rpx;
	}
	.p1{
		color: #FFFFFF;
		font-size: 30rpx;
		position: absolute;
		top: 50rpx;
		left: 200rpx;
	}
	.p2{
		color: #FFFFFF;
		font-size: 30rpx;
		position: absolute;
		top: 120rpx;
		left: 200rpx;
	}
	.items{
		position: absolute;
		width: 100%;
		top: 400rpx;
	}
	.item{
		position: relative;
		float: left;
		width: 100%;
		height: 150rpx;
		border-bottom: #808080 solid 1px;
	}
	.item image{
		position: absolute;
		left: 30rpx;
		top: 25rpx;
		width: 100rpx;
		height: 100rpx;
	}
	.item .xin{
		position: absolute;
		font-size: 50rpx;
		left: 180rpx;
		top: 45rpx;
		font-weight: 500;
	}
	.item .zuo{
		position: absolute;
		left: 700rpx;
		top: 50rpx;
		color: #555555;
	}
</style>
