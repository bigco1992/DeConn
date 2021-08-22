<template>
	<div class="share">
		<div class="shareWrapper">
			<div class="shareTop">
				<img class="shareProfileImg" src="../../assets/person/1.jpeg" alt="" />
				<input class="shareInput" placeholder="What's in your mind KIM?" />
			</div>
			<hr class="shareHr" />
			<div class="shareBottom">
				<div class="shareOptions">
					<div class="shareOption">
						<i class="fas fa-photo-video shareIcon"></i>
						<span class="shareOptionText">Photo or Video</span>
					</div>
					<div class="shareOption">
						<i class="fas fa-tag shareIcon"></i>
						<span class="shareOptionText">Tag</span>
					</div>
					<div class="shareOption">
						<i class="fas fa-map-marker-alt shareIcon"></i>
						<span class="shareOptionText">Location</span>
					</div>
					<div class="shareOption">
						<i class="far fa-smile-beam shareIcon"></i>
						<span class="shareOptionText">Feelings</span>
					</div>
				</div>
				<button class="shareButton">Share</button>
			</div>
		</div>
	</div>
</template>

<script>
export default {};
</script>

<style scoped>
.share {
	width: 100%;
	height: 170px;
	border-radius: 10px;
	-webkit-box-shadow: 0px 0px 16px -8px rgba(0, 0, 0, 0.68);
	box-shadow: 0px 0px 16px -8px rgba(0, 0, 0, 0.68);
}

.shareWrapper {
	padding: 10px;
}

.shareTop {
	display: flex;
	align-items: center;
}

.shareProfileImg {
	width: 50px;
	height: 50px;
	border-radius: 50%;
	object-fit: cover;
	margin-right: 10px;
}

.shareInput {
	border: none;
	width: 80%;
}

.shareInput:focus {
	outline: none;
}

.shareHr {
	margin: 20px;
}

.shareBottom {
	display: flex;
	align-items: center;
	justify-content: space-between;
}

.shareOptions {
	display: flex;
	margin-left: 20px;
}

.shareOption {
	display: flex;
	align-items: center;
	margin-right: 15px;
	cursor: pointer;
}

.shareIcon {
	font-size: 18px;
	margin-right: 3px;
}

.fa-photo-video {
	color: tomato;
}

.fa-tag {
	color: blue;
}

.fa-map-marker-alt {
	color: green;
}

.fa-smile-beam {
	color: goldenrod;
}

.shareOptionText {
	font-size: 14px;
	font-weight: 500;
}

.shareButton {
	border: none;
	padding: 7px;
	border-radius: 5px;
	background-color: green;
	font-weight: 500;
	margin-right: 20px;
	cursor: pointer;
	color: #ffffff;
}
</style>
