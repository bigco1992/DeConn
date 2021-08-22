<template>
	<div>
		<Topbar></Topbar>
		<div class="profile">
			<Sidebar></Sidebar>
			<div class="profileRight">
				<div class="profileRightTop">
					<div class="profileCover">
						<img class="profileCoverImg" src="../assets/post/3.jpeg" alt="" />
						<img class="profileUserImg" src="../assets/person/7.jpeg" alt="" />
					</div>
					<div class="profileInfo">
						<h4 class="profileInfoName">Kiyoung</h4>
						<span class="profileInfoDesc">Hellow my friends!</span>
					</div>
				</div>
				<div class="profileRightBottom">
					<Feed></Feed>
					<ProfileRightbar></ProfileRightbar>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import Topbar from '../components/topbar/Topbar.vue';
import Sidebar from '../components/sidebar/Sidebar.vue';
import Feed from '../components/feed/Feed.vue';
import ProfileRightbar from '../components/rightbar/ProfileRightbar.vue';

export default {
	components: {
		Topbar,
		Sidebar,
		Feed,
		ProfileRightbar,
	},
};
</script>

<style scoped>
.profile {
	display: flex;
}

.profileRight {
	flex: 9;
}

.profileCover {
	height: 320px;
	position: relative;
}

.profileCoverImg {
	width: 100%;
	height: 250px;
	object-fit: cover;
}

.profileUserImg {
	width: 150px;
	height: 150px;
	border-radius: 50%;
	object-fit: cover;
	position: absolute;
	left: 0;
	right: 0;
	margin: auto;
	top: 150px;
	border: 3px solid #ffffff;
}

.profileInfo {
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
}

.profileInfoName {
	font-size: 24px;
}

.profileInfoDesc {
	font-weight: 300;
}

.profileRightBottom {
	display: flex;
}
</style>
