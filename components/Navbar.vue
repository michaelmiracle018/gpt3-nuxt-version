<template>
	<div class="container">
		<div class="navbar">
			<div class="navbar__links">
				<div class="navbar__logo">
					<img src="~/assets/img/logo.svg" alt="navbar-logo" />
				</div>
				<div class="navbar__links-container">
					<Menu />
				</div>
			</div>
			<div class="navbar__sign">
				<div class="navbar__sign-btn">
					<p>sign in</p>
					<button type="button">sign up</button>
				</div>
				<div class="navbar__menu-btn">
					<i class="fa-solid fa-bars" @click="handleToggleMenu"></i>
					<!-- <i class="fa-solid fa-xmark" v-if="(toggleMenu = false)"></i> -->
				</div>
			</div>
		</div>
		<div class="navbar__sm_menu-container scale-up-center" v-if="toggleMenu">
			<div class="navbar__sm-menu">
				<Menu />
				<div class="navbar__sm_menu-button">
					<p>sign in</p>
					<button type="button">sign up</button>
				</div>
			</div>
		</div>
	</div>
</template>

<script setup>
	const toggleMenu = ref(false);

	const handleToggleMenu = () => {
		toggleMenu.value = !toggleMenu.value;
	};
</script>

<style>
	.navbar {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 2rem 0;
		position: relative;
	}

	.navbar .navbar__links {
		display: flex;
		justify-content: space-between;
		align-items: center;
		gap: 50px;
	}

	.navbar .navbar__logo img {
		width: 62.56px;
		height: 16.02px;
		object-fit: cover;
	}
	.navbar .navbar__links-container .menu__links {
		display: flex;
		justify-content: center;
		align-items: center;
		gap: 20px;
	}

	.navbar .navbar__links-container .menu__links a,
	.navbar__sign p,
	.navbar__sm-menu p,
	.navbar__sm-menu .menu__links a {
		color: #fff;
		font-family: "montserrat";
		font-weight: 500;
		font-size: 18px;
		line-height: 25px;
		text-transform: capitalize;
		cursor: pointer;
	}

	.navbar .navbar__sign,
	.navbar__sign-btn {
		display: flex;
		align-items: center;
		gap: 20px;
	}

	.navbar .navbar__sign button,
	.navbar__sm-menu button {
		padding: 0.5rem 1rem;
		color: #fff;
		background: #ff4820;
		font-family: "montserrat";
		font-weight: 500;
		font-size: 18px;
		line-height: 25px;
		border: none;
		outline: none;
		cursor: pointer;
		border-radius: 5px;
	}
	.navbar__menu-btn {
		display: none;
	}

	.navbar__menu-btn i {
		font-size: 20px;
		color: #fff;
	}

	.navbar__sm_menu-container {
		display: none;
		position: relative;
	}

	.navbar__sm-menu {
		text-align: end;
		background: var(--dark-color);
		padding: 2rem;
		position: absolute;
		right: 0;
		top: -10px;
		margin-top: 3rem;
		min-width: 210px;
		border-radius: 5px;
		box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.2);
	}

	.navbar__sm-menu .menu__links p,
	.navbar__sm_menu-button p {
		margin: 10px 0;
	}
	@media screen and (max-width: 1050px) {
		.navbar .navbar__links-container .menu__links {
			display: none;
		}
		.navbar__sm_menu-container {
			display: block;
		}
		.navbar__menu-btn {
			display: block;
		}
		.navbar__sm_menu-button {
			display: none;
		}
	}
	@media screen and (max-width: 550px) {
		.navbar__sign-btn {
			display: none;
		}
		.navbar__sm_menu-button {
			display: block;
		}
	}
</style>
