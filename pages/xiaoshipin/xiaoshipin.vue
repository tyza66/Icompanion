<template>
	<view>
		<view class="top"></view>
		<view class="mianfei"><p>免费资源</p></view>
		<view class="mainfei1">
			<view class="one">
				<view class="im"><image src="../../static/icons/hh1.png"></image></view>
				<view class="ti"><p>外国老年人整活</p></view>
				<view class="up"><p>观看：1000</p></view>
			</view>
			<view class="one">
				<view class="im"><image src="../../static/icons/hh2.png"></image></view>
				<view class="ti"><p>老年人也想看短视频</p></view>
				<view class="up"><p>观看：900</p></view>
			</view>
			<view class="one">
				<view class="im"><image src="../../static/icons/hh3.png"></image></view>
				<view class="ti"><p>老年人进军短视频了</p></view>
				<view class="up"><p>观看：900</p></view>
			</view>
			<view class="one">
				<view class="im"><image src="../../static/icons/hh4.png"></image></view>
				<view class="ti"><p>老年人学做短视频</p></view>
				<view class="up"><p>观看：780</p></view>
			</view>
			<view class="one">
				<view class="im"><image src="../../static/icons/hh5.png"></image></view>
				<view class="ti"><p>老年人自媒体视频的好处</p></view>
				<view class="up"><p>观看：640</p></view>
			</view>
			<view class="one">
				<view class="im"><image src="../../static/icons/hh6.png"></image></view>
				<view class="ti"><p>公园</p></view>
				<view class="up"><p>观看：530</p></view>
			</view>
			<view class="one">
				<view class="im"><image src="../../static/icons/hh1.png"></image></view>
				<view class="ti"><p>外国老年人整活</p></view>
				<view class="up"><p>观看：1000</p></view>
			</view>
			<view class="one">
				<view class="im"><image src="../../static/icons/hh2.png"></image></view>
				<view class="ti"><p>老年人也想看短视频</p></view>
				<view class="up"><p>观看：900</p></view>
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
		onLoad() {

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
	.mianfei{
		width: 100%;
		height: 100rpx;
		background: #999999;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.one{
		float: left;
		height: 340rpx;
		width: 49%;
		margin-left: 1%;
		margin-top: 10rpx;
		border-radius: 10rpx;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		background: #F8F8F8;
	}
	.one .im{
		width: 100%;
		height: 60%;
	}
	.one .im image{
		width: 100%;
		height: 100%;
	}
	.one .ti{
		width: 100%;
		height: 20%;
	}
	.one .ti p{
		text-align: center;
		width: 100%;
		height: 20%;
	}
	.one .up{
		width: 100%;
		height: 20%;
	}
</style>
