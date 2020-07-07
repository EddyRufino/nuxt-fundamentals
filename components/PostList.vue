<template>
	<nuxt-link :to="{ name: 'posts-id', params: {id: post.id} }">{{ post.title }}</nuxt-link>
</template>

<script>
export default {
	name: "PostList",
	props: ['post'],
}
</script>