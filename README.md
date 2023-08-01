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
		top: 40px;
		margin-top: 3rem;
		min-width: 210px;
		border-radius: 5px;
		box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.2);
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
	}
	@media screen and (max-width: 550px) {
		.navbar__sign-btn {
			display: none;
		}
	}