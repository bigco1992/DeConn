<template>
	<div class="sidebar">
		<div class="sidebarWrapper">
			<ul class="sidebarList">
				<li class="sidebarListItem">
					<i class="fas fa-rss sidebarIcon"></i>
					<span class="sidebarListItemText">Feed</span>
				</li>
				<li class="sidebarListItem">
					<i class="fas fa-comments sidebarIcon"></i>
					<span class="sidebarListItemText">Chats</span>
				</li>
				<li class="sidebarListItem">
					<i class="fas fa-play-circle sidebarIcon"></i>
					<span class="sidebarListItemText">Videos</span>
				</li>
				<li class="sidebarListItem">
					<i class="fas fa-user-friends sidebarIcon"></i>
					<span class="sidebarListItemText">Groups</span>
				</li>
				<li class="sidebarListItem">
					<i class="fas fa-bookmark sidebarIcon"></i>
					<span class="sidebarListItemText">Bookmarks</span>
				</li>
				<li class="sidebarListItem">
					<i class="far fa-question-circle sidebarIcon"></i>
					<span class="sidebarListItemText">Questions</span>
				</li>
				<li class="sidebarListItem">
					<i class="fas fa-briefcase sidebarIcon"></i>
					<span class="sidebarListItemText">Jobs</span>
				</li>
				<li class="sidebarListItem">
					<i class="far fa-calendar-alt sidebarIcon"></i>
					<span class="sidebarListItemText">Events</span>
				</li>
				<li class="sidebarListItem">
					<i class="fas fa-graduation-cap sidebarIcon"></i>
					<span class="sidebarListItemText">Courses</span>
				</li>
			</ul>
			<button class="sidebarButton">Show More</button>
			<hr class="sidebarHr" />
			<ul class="sidebarFriendList">
				<!-- <li class="sidebarFriend">
					<img
						class="sidebarFriendImg"
						src="../../assets/person/2.jpeg"
						alt=""
					/>
					<span class="sidebarFriendName">jane don</span>
				</li> -->
				<CloseFriend></CloseFriend>
			</ul>
		</div>
	</div>
</template>

<script>
import CloseFriend from '../closeFriend/CloseFriend.vue';

export default {
	components: {
		CloseFriend,
	},
};
</script>

<style scoped>
.sidebar {
	flex: 3;
	height: calc(100vh - 50px);
	overflow-y: scroll;
	position: sticky;
	top: 50px;
}

::-webkit-scrollbar {
	width: 5px;
}
::-webkit-scrollbar-track {
	background-color: #f1f1f1;
}
::-webkit-scrollbar-thumb {
	background-color: rgb(179, 179, 179);
}

.sidebarWrapper {
	padding: 20px;
}

.sidebarList {
	padding: 0;
	margin: 0;
	list-style: none;
}

.sidebarListItem {
	display: flex;
	align-items: center;
	margin-bottom: 20px;
}

.sidebarIcon {
	margin-right: 15px;
}

.sidebarButton {
	width: 150px;
	border: none;
	padding: 10px;
	border-radius: 5px;
	font-weight: 500;
}

.sidebarHr {
	margin: 20px 0;
}

.sidebarFriendList {
	padding: 0;
	margin: 0;
	list-style: none;
}
</style>
