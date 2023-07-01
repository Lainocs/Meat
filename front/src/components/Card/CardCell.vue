<template>
	<div class="card-cell">
		<img
			src="@/assets/shrek.webp"
			alt="profile picture	"
		/>
		<CardInfo
			:name="'Shrek'"
			:status="'Ogre'"
		/>
		<div class="card-buttons">
			<CardButton
				:image="require('@/assets/cross.png')"
				:color="'rgba(255,255,255,0.3)'"
			/>
			<CardButton
				:image="require('@/assets/meat.png')"
				:color="'rgba(255,255,255,0.3)'"
			/>
		</div>
	</div>
</template>
<script>
	import CardButton from './CardButton.vue'
	import CardInfo from './CardInfo.vue'
	export default {
		name: 'CardCell',
		components: {
			CardButton,
			CardInfo,
		},
	}
</script>
<style lang="scss" scoped>
	.card-cell {
		height: 70vh;
		min-width: 300px;
		width: 30%;
		background-color: #ecf0f1;
		border-radius: 20px;
		position: relative;
		box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
		&::before {
			content: '';
			position: absolute;
			height: 100%;
			width: 100%;
			background: linear-gradient(
				0deg,
				rgba(0, 0, 0, 0.9) 0%,
				rgba(0, 0, 0, 0.5) 30%,
				rgba(0, 0, 0, 0.2) 100%
			);
			border-radius: 20px;
		}

		.card-buttons {
			display: flex;
			justify-content: space-around;
			position: absolute;
			width: 100%;
			bottom: 20px;
		}

		img {
			height: 100%;
			width: 100%;
			border-radius: 20px;
			object-fit: cover;
		}
	}
</style>
