<template>
  <main class="home">
		<h1>Home</h1>
		<section>
			<CardCell />
		</section>
  </main>
</template>

<script>
import CardCell from '@/components/Card/CardCell'
export default {
  name: 'HomeView',
	components: {
		CardCell
	}
}
</script>

<style scoped>
	section {
		display: flex;
		justify-content: center;
	}
</style>