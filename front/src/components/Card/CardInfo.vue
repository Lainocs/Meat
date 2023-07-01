<template>
	<div class="card-info">
		<h2>{{ name }}</h2>
		<small>{{ status }}</small>
	</div>
</template>
<script>
	export default {
		name: 'CardInfo',
		props: ['name', 'status'],
	}
</script>
<style lang="scss" scoped>
	.card-info {
		width: 80%;
		margin: 0 auto;
		color: #2c3e50;
		position: absolute;
		bottom: 120px;
		left: 30px;
		text-align: left;
		color: white;
		line-height: 0.8;

		h2 {
			font-size: 1.5rem;
			margin-bottom: 10px;
		}

		small {
			font-size: 1rem;
		}
}
</style>
