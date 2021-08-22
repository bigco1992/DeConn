<template>
	<div>
		<Topbar></Topbar>
		<div class="homeContainer">
			<Sidebar></Sidebar>
			<Feed></Feed>
			<Rightbar></Rightbar>
		</div>
	</div>
</template>

<script>
// @ is an alias to /src
import Topbar from '../components/topbar/Topbar.vue';
import Sidebar from '../components/sidebar/Sidebar.vue';
import Feed from '../components/feed/Feed.vue';
import Rightbar from '../components/rightbar/Rightbar.vue';

export default {
	name: 'Home',
	components: {
		Topbar,
		Sidebar,
		Feed,
		Rightbar,
	},
};
</script>

<style scoped>
.homeContainer {
	display: flex;
}
</style>
