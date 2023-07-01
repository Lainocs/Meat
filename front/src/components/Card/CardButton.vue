<template>
	<!-- change background color on hover -->
	<button
		class="card-button"
		:style="{ backgroundColor: color, boxShadow: `0 0 10px ${color}` }"
	>
		<img :src="image" />
	</button>
</template>
<script>
	export default {
		name: 'CardButton',
		props: ['image', 'color'],
	}
</script>
<style lang="scss" scoped>
	.card-button {
		height: 60px;
		width: 60px;
		border-radius: 50%;
		display: flex;
		justify-content: center;
		align-items: center;
		border: none;
		outline: none;
		cursor: pointer;
		transition: all 0.2s ease-in-out;
		box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
		&:hover {
			transform: scale(1.1);
		}

		img {
			height: 80%;
			width: 80%;
			margin: 0 auto;
			border-radius: 50%;
		}
	}
</style>
