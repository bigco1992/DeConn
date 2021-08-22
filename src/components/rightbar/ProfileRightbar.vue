<template>
	<div class="rightbar">
		<div class="rightbarWrapper">
			<h4 class="rightbarTitle">User Information</h4>
			<div class="rightbarInfo">
				<div class="rightbarInfoItem">
					<span class="rightbarInfoKey">City:</span>
					<span class="rightbarInfoValue">New York</span>
				</div>
				<div class="rightbarInfoItem">
					<span class="rightbarInfoKey">From:</span>
					<span class="rightbarInfoValue">Madrid</span>
				</div>
				<div class="rightbarInfoItem">
					<span class="rightbarInfoKey">Relationship:</span>
					<span class="rightbarInfoValue">Signle</span>
				</div>
				<h4 class="rightbarTitle">User Friends</h4>
				<div class="rightbarFollowings">
					<div class="rightbarFollowing">
						<img
							class="rightbarFollowingImg"
							src="../../assets/person/1.jpeg"
							alt=""
						/>
						<span class="rightbarFollowingName">Kiyoung</span>
					</div>
					<div class="rightbarFollowing">
						<img
							class="rightbarFollowingImg"
							src="../../assets/person/1.jpeg"
							alt=""
						/>
						<span class="rightbarFollowingName">Kiyoung</span>
					</div>
					<div class="rightbarFollowing">
						<img
							class="rightbarFollowingImg"
							src="../../assets/person/1.jpeg"
							alt=""
						/>
						<span class="rightbarFollowingName">Kiyoung</span>
					</div>
					<div class="rightbarFollowing">
						<img
							class="rightbarFollowingImg"
							src="../../assets/person/1.jpeg"
							alt=""
						/>
						<span class="rightbarFollowingName">Kiyoung</span>
					</div>
					<div class="rightbarFollowing">
						<img
							class="rightbarFollowingImg"
							src="../../assets/person/1.jpeg"
							alt=""
						/>
						<span class="rightbarFollowingName">Kiyoung</span>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {};
</script>

<style scoped>
.rightbar {
	flex: 3.5;
}

.rightbarWrapper {
	padding: 20px 20px 0 0;
}
.rightbarTitle {
	font-size: 18px;
	font-weight: 500;
	margin-bottom: 10px;
}

.rightbarInfo {
	margin-bottom: 30px;
}

.rightbarInfoItem {
	margin-bottom: 10px;
}

.rightbarInfoKey {
	font-weight: 500;
	margin-right: 15px;
	color: #555;
}

.rightbarInfoValue {
	font-weight: 300;
}

.rightbarFollowings {
	display: flex;
	flex-wrap: wrap;
	justify-content: space-between;
}

.rightbarFollowing {
	display: flex;
	flex-direction: column;
	margin-bottom: 20px;
	margin-right: 10px;
	cursor: pointer;
}

.rightbarFollowingImg {
	width: 100px;
	height: 100px;
	object-fit: cover;
	border-radius: 5px;
}
</style>
