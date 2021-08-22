<template>
	<div>
		<li class="rightbarFriend" v-for="user in Users" :key="user.id">
			<div class="rightbarProfileImgContainer">
				<img src="../../assets/person/1.jpeg" class="rightbarProfileImg" />
				<span class="rightbarOnline"></span>
			</div>
			<span class="rightbarUsername">{{ user.username }}</span>
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
.rightbarFriend {
	display: flex;
	align-items: center;
	margin-bottom: 15px;
}

.rightbarProfileImgContainer {
	margin-left: 10px;
	position: relative;
}

.rightbarProfileImg {
	width: 40px;
	height: 40px;
	border-radius: 50%;
	object-fit: cover;
}

.rightbarOnline {
	width: 12px;
	height: 12px;
	border-radius: 50%;
	background-color: limegreen;
	position: absolute;
	top: -2;
	right: 0;
	border: 2px solid #ffffff;
}

.rightbarUsername {
	font-weight: 500;
}
</style>
