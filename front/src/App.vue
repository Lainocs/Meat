<template>
  <MainLayout>
	</MainLayout>
</template>
<script>
	import MainLayout from '@/layouts/MainLayout'
	export default {
		name: 'App',
		components: {
			MainLayout
		}
	}
</script>
<style lang="scss">
* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}
#app {
  font-family: Montserrat, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
