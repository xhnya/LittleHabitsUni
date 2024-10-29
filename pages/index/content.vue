<template>
	<view class="">
		<uni-section title="常用" type="line" padding>
			<uni-grid :column="3" :show-border="false" :square="false" @change="change">
				<uni-grid-item v-for="(item ,index) in list" :index="index" :key="index">
					<view class="grid-item-box">
						<text class="text">{{item.text}}</text>
						<!-- <image class="image" :src="item.url" mode="aspectFill" />
						<text class="text">{{item.text}}</text>
						<view v-if="item.badge" class="grid-dot">
							<uni-badge :text="item.badge" :type="item.type" />
						</view> -->
					</view>
				</uni-grid-item>
			</uni-grid>
		</uni-section>
	</view>
</template>

<script setup>
	let list = [{
			url: '',
			text: 'xxx'
		},
		{
			url: '',
			text: 'xxx'
		},
		{
			url: '',
			text: 'xxx'
		}
	]

	const change = () => {

	}
</script>

<style>
</style>