<template>
	<div>
		<li class="sidebarFriend" v-for="user in Users" :key="user.id">
			<img class="sidebarFriendImg" src="../../assets/person/2.jpeg" alt="" />
			<span class="sidebarFriendName">{{ user.username }}</span>
		</li>
	</div>
</template>

<script>
import { Users } from '../../dummyData.js';

export default {
	data() {
		return {
			Users,
		};
	},
};
</script>

<style scoped>
.sidebarFriend {
	display: flex;
	align-items: center;
	margin-bottom: 15px;
}

.sidebarFriendImg {
	width: 32px;
	height: 32px;
	border-radius: 50%;
	object-fit: cover;
	margin-right: 10px;
}
</style>
