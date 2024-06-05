<template>
	<view class="container">
		<Home></Home>
		<Content></Content>
		<Me></Me>
		<BottomNav/>
	</view>
</template>

<script setup>
	import Content from '../components/Content/index.vue'
	import Home from '../components/Home/index.vue'
	import Me from '../components/Me/index.vue'
	import BottomNav from '../components/BottomNav/BottomNav.vue'
</script>

<style>
	.container {
		background-color: lightgray;
	}
</style>
