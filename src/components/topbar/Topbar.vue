<template>
	<div class="topbarContainer">
		<div class="topbarLeft">
			<span class="logo">DeConn</span>
		</div>
		<div class="topbarCenter">
			<div class="searchbar">
				<i class="fas fa-search searchIcon"></i>
				<input
					placeholder="Search for friend, post or video"
					class="searchInput"
				/>
			</div>
		</div>
		<div class="topbarRight">
			<div class="topbarLinks">
				<span class="topbarLink">Homepage</span>
				<span class="topbarLink">Timeline</span>
			</div>
			<div class="topbarIcons">
				<div class="topbarIconItem">
					<i class="fas fa-user"></i>
					<span class="topbarIconBadge">1</span>
				</div>
				<div class="topbarIconItem">
					<i class="fas fa-comments"></i>
					<span class="topbarIconBadge">2</span>
				</div>
				<div class="topbarIconItem">
					<i class="fas fa-bell"></i>
					<span class="topbarIconBadge">3</span>
				</div>
			</div>
			<img src="../../assets/person/1.jpeg" alt="" class="topbarImage" />
		</div>
	</div>
</template>

<script>
export default {};
</script>

<style scoped>
.topbarContainer {
	height: 50px;
	width: 100%;
	background-color: #1877f2;
	display: flex;
	align-items: center;
	position: sticky;
	top: 0;
	z-index: 999;
}

.topbarLeft {
	flex: 3;
}

.logo {
	font-size: 24px;
	margin-left: 20px;
	font-weight: bold;
	color: #ffffff;
	cursor: pointer;
}

.topbarCenter {
	flex: 5;
}

.searchbar {
	width: 100%;
	height: 30px;
	background-color: #ffffff;
	border-radius: 30px;
	display: flex;
	align-items: center;
}

.searchIcon {
	font-size: 14px !important;
	margin-left: 10px;
}

.searchInput {
	border: none;
	width: 70%;
}

.searchInput:focus {
	outline: none;
}

.topbarRight {
	flex: 4;
	display: flex;
	align-items: center;
	justify-content: space-around;
	color: #ffffff;
}

.topbarLink {
	margin-right: 10px;
	font-size: 14px;
	cursor: pointer;
}

.topbarIcons {
	display: flex;
}

.topbarIconItem {
	margin-right: 15px;
	cursor: pointer;
	position: relative;
}

.topbarIconBadge {
	width: 15px;
	height: 15px;
	background-color: red;
	border-radius: 50%;
	color: #ffffff;
	position: absolute;
	top: -5px;
	right: -5px;
	display: flex;
	align-items: center;
	justify-content: center;
	font-size: 12px;
}

.topbarImage {
	width: 32px;
	height: 32px;
	border-radius: 50%;
	object-fit: cover;
	cursor: pointer;
}
</style>
