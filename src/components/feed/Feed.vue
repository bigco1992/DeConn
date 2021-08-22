<template>
	<div class="feed">
		<div class="feedWrapper">
			<Share></Share>
			<Post></Post>
		</div>
	</div>
</template>

<script>
import Share from '../share/Share.vue';
import Post from '../post/Post.vue';

export default {
	components: {
		Share,
		Post,
	},
};
</script>

<style scoped>
.feed {
	flex: 5.5;
}

.feedWrapper {
	padding: 20px;
}
</style>
