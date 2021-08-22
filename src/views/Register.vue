<template>
	<div class="login">
		<div class="loginWrapper">
			<div class="loginLeft">
				<h3 class="loginLogo">DevBook</h3>
				<span class="loginDesc"
					>Connect with friends and the world around you on DevBook</span
				>
			</div>
			<div class="loginRight">
				<div class="loginBox">
					<input placeholder="Username" class="loginInput" />
					<input placeholder="Email" class="loginInput" />
					<input placeholder="Password" class="loginInput" />
					<input placeholder="Password Again" class="loginInput" />
					<button class="loginButton">Sign Up</button>
					<button class="loginRegisterButton">
						Log into Account
					</button>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {};
</script>

<style scoped>
.login {
	width: 100vw;
	height: 100vh;
	background-color: #f0f2f5;
	display: flex;
	align-items: center;
	justify-content: center;
}

.loginWrapper {
	width: 70%;
	height: 70%;
	display: flex;
}

.loginLeft,
.loginRight {
	flex: 1;
	display: flex;
	flex-direction: column;
	justify-content: center;
}

.loginLogo {
	font-size: 50px;
	font-weight: 800;
	color: #1775ee;
	margin-bottom: 10px;
}

.loginDesc {
	font-size: 24px;
}

.loginBox {
	height: 400px;
	padding: 20px;
	background-color: #ffffff;
	border-radius: 10px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

.loginInput {
	height: 50px;
	border-radius: 10px;
	border: 1px solid gray;
	font-size: 18px;
	padding-left: 20px;
}

.loginInput:focus {
	outline: none;
}

.loginButton {
	height: 50px;
	border-radius: 10px;
	border: none;
	background-color: #1775ee;
	color: white;
	font-size: 20px;
	font-weight: 500;
	cursor: pointer;
}

.loginForgot {
	text-align: center;
	color: #1775ee;
}

.loginRegisterButton {
	width: 60%;
	align-self: center;
	height: 50px;
	border-radius: 10px;
	border: none;
	background-color: #42b72a;
	color: #ffffff;
	font-size: 20px;
	font-weight: 500;
	cursor: pointer;
}
</style>
