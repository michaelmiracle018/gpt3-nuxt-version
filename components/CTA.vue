<template>
	<div class="container">
		<div class="cta">
			<div class="cta__content">
				<p>Request Early Access to Get Started</p>
				<h3>Register Today & start exploring the endless possibilities.</h3>
			</div>
			<div class="cta__btn">
				<button type="button">Get Started</button>
			</div>
		</div>
	</div>
</template>

<script setup></script>

<style scoped>
	.cta {
		display: flex;
		justify-content: space-between;
		align-items: center;
		flex-direction: row;

		padding: 2rem;
		margin: 4rem;
		border-radius: 1rem;
		background: var(--gradient-bar);
	}

	.cta__content {
		display: flex;
		flex-direction: column;
		text-align: left;
		color: #fff;
	}

	.cta__content p {
		font-family: var(--font-family);
		font-size: 12px;
		line-height: 30px;
		font-weight: 500;
	}

	.cta__content h3 {
		font-family: var(--font-family);
		font-size: 24px;
		line-height: 45px;
		font-weight: 800;
	}

	.cta__btn button {
		background: #000;
		color: #fff;
		font-family: var(--font-family);
		font-weight: 700;
		font-size: 18px;
		line-height: 30px;
		padding: 0.5rem 1rem;
		border-radius: 2rem;

		border: none;
		outline: none;
		cursor: pointer;
		min-width: 150px;
	}

	@media screen and (max-width: 650px) {
		.cta {
			flex-direction: column;
		}
	}

	@media screen and (max-width: 700px) {
		.cta {
			flex-direction: column;
			margin: 4rem 2rem;
		}
		.cta__content h3 {
			font-size: 18px;
			line-height: 32px;
		}

		.cta__btn button {
			font-size: 14px;
			line-height: 28px;
		}

		.cta__btn {
			margin: 2rem 0 0;
		}
	}
</style>
