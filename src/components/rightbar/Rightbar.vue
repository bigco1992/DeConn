<template>
	<div class="rightbar">
		<div class="rightbarWrapper">
			<div class="birthdayContainer">
				<img class="birthdayImg" src="../../assets/gift.png" alt="" />
				<sapn class="birthdayText"
					>pola Foster and 3 other friends hav a birthday today</sapn
				>
			</div>
			<img src="../../assets/ad.png" alt="" class="rightbarAd" />
			<h4 class="rightbarTitle">Online Friend</h4>
			<ul class="rightbarFriendList">
				<Online></Online>
			</ul>
		</div>
	</div>
</template>

<script>
import { Users } from '../../dummyData.js';
import Online from '../online/Online.vue';

export default {
	components: {
		Online,
	},
	data() {
		return {
			Users,
		};
	},
};
</script>

<style scoped>
.rightbar {
	flex: 3.5;
}

.rightbarWrapper {
	padding: 20px 20px 0 0;
}

.birthdayContainer {
	display: flex;
	align-items: center;
}

.birthdayImg {
	width: 40px;
	height: 40px;
	margin-right: 10px;
}

.birthdayText {
	font-weight: 300;
	font-size: 15px;
}

.rightbarAd {
	width: 100%;
	border-radius: 10px;
	margin: 30px 0;
}

.rightbarTitle {
	margin-bottom: 20px;
}

.rightbarFriendList {
	padding: 0;
	margin: 0;
	list-style: none;
}
</style>
