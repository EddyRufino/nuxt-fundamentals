<template>
	<section class="container-post">
		<p>{{ this.$route.params.id }}</p>
	</section>
</template>

<style scoped>
.container-post {
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	padding: 1rem;
}
</style>