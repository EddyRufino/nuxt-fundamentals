<template>
	<nuxt-link :to="`posts/${post.id}`">{{ post.title }}</nuxt-link>
</template>

<script>
export default {
	name: "PostList",
	props: ['post'],
}
</script>