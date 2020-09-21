<template>
	<div id="app">
		<h3>测试按钮</h3>
		<UcButton />
		<uc-button text="登 录" />
		<uc-button bg-color="#399" />
		<uc-button>注 册</uc-button>
		<uc-button @click="show">点 击</uc-button>
	</div>
</template>

<script>
	import UcButton from '../components/uc-button/uc-button.vue'
	export default {
		name: 'App',
		components: {
			UcButton
		},
		methods: {
			show(ev) {
				console.log(ev)
			}
		}
	}
</script>

<style>
	#app {
		font-family: Avenir, Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
		margin-top: 60px;
	}
</style>
