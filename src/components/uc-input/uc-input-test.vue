<template>
	<div id="app">
		<h3>测试输入框</h3>
		<!-- <UcInput @click.native="alert(1)"/> -->
		<UcInput />
		<!-- <uc-input v-model="ipt" :value="ipt" @input="show"></uc-input> -->
		<uc-input v-model="ipt"></uc-input>
		<uc-input v-model="ipt2" type="password" label="密 码"></uc-input>
	</div>
</template>

<script>
	import UcInput  from '../components/uc-input/uc-input.vue'
	export default {
		name: 'App',
		data(){
			return {
				ipt:'bmw',
				ipt2:'k5'
			}
		},
		
		components: {
			UcInput
		},
		
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
