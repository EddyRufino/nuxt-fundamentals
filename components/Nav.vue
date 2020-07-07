<template>
	<section class="main">
		<nuxt-link class="container-logo" to="/">Fundamentals</nuxt-link>
		<ul class="container-nav">
			<li class="container-link">
				<nuxt-link class="container-href" to="/posts">Posts</nuxt-link>	
			</li>
			<li class="container-link">
				<nuxt-link class="container-href" to="#">WerEver</nuxt-link>
			</li>
		</ul>
	</section>
</template>

<style>
.main {
	display: flex;
	justify-content: space-around;
	align-items: center;
}
.container-nav {
	display: flex;
	justify-content: space-between;
	list-style: none;
	max-width: 1200px;
}
.container-link {
	padding: 1rem;
}
.container-href {
	text-decoration: none;
}
.container-logo {
	text-decoration: none;
	font-size: 1.3rem;
	font-family: sans-serif;
}
</style>