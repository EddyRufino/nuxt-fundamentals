<template>
	<div class="container-post">
		<PostList
			v-for="(post, index) in posts"
			:key="index"
			:post="post"
		/>
	</div>
</template>

<script>
import PostList from "@/components/PostList";

export default {
	name: "Posts",
	components: {
		PostList
	},
	data() {
		return {
			id: this.$route.params.id,
			posts: [
				{
				    id: 1,
				    title: 'sunt aut facere repellat' ,
				},
				{
				    id: 2,
				    title: 'post 2 repellat aut facere repellat',
				},
				{
				    id: 3,
				    title: 'post 3 aut facere repellat repellat',
				}
			]
		}
	},
	computed: {
		post() {
			return this.posts.find(post => post.id === this.id)
		}
	}
}
</script>

<style scoped>
.container-post {
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	padding: 1rem;
}
</style>