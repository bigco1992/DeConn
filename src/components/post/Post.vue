<template>
	<div>
		<div class="post" v-for="Post in Posts" :key="Post.id">
			<div class="postWrapper">
				<div class="postTop">
					<div class="postTopLeft">
						<img
							class="postProfileImg"
							src="../../assets/person/1.jpeg"
							alt=""
						/>
						<span class="postUsername">{{
							Users.filter(u => u.id === Post?.userId)[0].username
						}}</span>
						<span class="postDate">{{ Post.date }}</span>
					</div>
					<div class="postTopRight">
						<i class="fas fa-ellipsis-v"></i>
					</div>
				</div>
				<div class="postCenter">
					<span class="postText">{{ Post.desc }}</span>
					<img class="postImg" src="../../assets/person/1.jpeg" />
				</div>
				<div class="postBottom">
					<div class="postBottomLeft">
						<img class="likeIcon" src="../../assets/like.png" alt="" />
						<img class="likeIcon" src="../../assets/heart.png" alt="" />
						<span class="postLikeCounter">{{ Post.like }} People liked it</span>
					</div>
					<div class="postBottomRight">
						<span class="postCommentText">{{ Post.comment }} comments</span>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import { Posts, Users } from '../../dummyData.js';

export default {
	data() {
		return {
			Posts,
			Users,
		};
	},
	methods: {
		postProfilePicture() {
			return Users.filter(u => u.id === Post?.userId)[0].profilePicture;
		},
	},
};
</script>

<style scoped>
.post {
	width: 100%;
	border-radius: 10px;
	-webkit-box-shadow: 0px 0px 16px -8px rgba(0, 0, 0, 0.68);
	box-shadow: 0px 0px 16px -8px rgba(0, 0, 0, 0.68);
	margin: 30px 0;
}

.postWrapper {
	padding: 10px;
}

.postTop {
	display: flex;
	align-items: center;
	justify-content: space-between;
}

.postTopLeft {
	display: flex;
	align-items: center;
}

.postProfileImg {
	width: 32px;
	height: 32px;
	border-radius: 50%;
	object-fit: cover;
}

.postUsername {
	font-size: 15px;
	font-weight: 500;
	margin: 0 10px;
}

.postDate {
	font-size: 12px;
}

.postCenter {
	margin: 20px 0;
}

.postImg {
	margin-top: 20px;
	width: 100%;
	max-height: 500px;
	object-fit: contain;
}

.postBottom {
	display: flex;
	align-items: center;
	justify-content: space-between;
}

.postBottomLeft {
	display: flex;
	align-items: center;
}

.likeIcon {
	width: 24px;
	height: 24px;
	margin-right: 5px;
	cursor: pointer;
}

.postLikeCounter {
	font-size: 15px;
}

.postCommentText {
	cursor: pointer;
	border-bottom: 1px dashed gray;
	font-size: 15px;
}
</style>
