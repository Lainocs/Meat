<template>
	<div>
		<nav>
			<router-link to="/">Home</router-link> |
			<router-link to="/login">Login</router-link>
		</nav>
		<router-view />
	</div>
</template>
<script>
export default {
	name: "MainLayout",

}
</script>
<style lang="scss" scoped>
	nav {
	display: flex;
	justify-content: flex-end;
  padding: 30px;
	background-color: #ecf0f1;

  a {
		margin: 0 10px;
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>