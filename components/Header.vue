<template>
	<div class="header__container container" id="home">
		<div class="header__content">
			<h1 class="gradient__text">
				Let&apos;s Build Something amazing with GPT-3 OpenAI
			</h1>
			<p>
				Yet bed any for travelling assistance indulgence unpleasing. Not
				thoughts all exercise blessing. Indulgence way everything joy alteration
				boisterous the attachment. Party we years to order allow asked of.
			</p>

			<div class="header__content-input">
				<input type="email" placeholder="Your Email Address" />
				<button type="button">Get Started</button>
			</div>

			<div class="header__content-people">
				<img src="~/assets/img/people.png" alt="people" />
				<p>1,600 people requested access a visit in last 24 hours</p>
			</div>
		</div>
		<div class="header__image">
			<img src="~/assets/img/ai.png" alt="ai" />
		</div>
	</div>
</template>

<script></script>

<style scoped>
	.header__container {
		display: flex;
		flex-direction: row;
		gap: 20px;
	}

	.header__content {
		flex: 1;
		display: flex;
		justify-content: center;
		align-items: flex-start;
		flex-direction: column;
	}
	.header__content h1 {
		font-family: var(--font-family);
		font-weight: 800;
		font-size: 55px;
		line-height: 65px;
		letter-spacing: -0.04em;
		margin-bottom: 2rem;
	}

	.header__content p {
		font-family: var(--font-family);
		font-weight: 400;
		font-size: 20px;
		line-height: 28px;
		color: var(--color-text);
	}

	.header__content-input {
		width: 100%;
		margin: 2rem 0 1rem;
		display: flex;
		flex-direction: row;
	}

	.header__content-input input {
		flex: 2;
		width: 100%;
		min-height: 50px;
		font-family: var(--font-family);
		font-weight: 400;
		font-size: 20px;
		line-height: 28px;
		background: var(--color-footer);
		border: 2px solid var(--color-footer);
		padding: 0 1rem;
		outline: none;
		color: #fff;

		border-top-left-radius: 5px;
		border-bottom-left-radius: 5px;
	}

	.header__content-input button {
		flex: 0.6;
		width: 100%;
		min-height: 50px;
		font-family: var(--font-family);
		font-weight: 400;
		font-size: 20px;
		line-height: 28px;
		background: #ff4820;
		border: 2px solid #ff4820;
		padding: 0 1rem;
		color: #fff;
		cursor: pointer;
		outline: none;

		border-top-right-radius: 5px;
		border-bottom-right-radius: 5px;
	}

	.header__content-people {
		width: 100%;
		display: flex;
		justify-content: flex-start;
		align-items: center;
		flex-direction: row;
		gap: 1rem;

		margin-top: 2rem;
	}
	.header__content-people img {
		width: 181.79px;
		height: 38px;
	}

	.header__content-people p {
		margin: 0 0 0 1rem;
		font-family: var(--font-family);
		font-weight: 500;
		font-size: 12px;
		line-height: 38px;
		color: #fff;
		text-align: center;
	}

	.header__image {
		flex: 1;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	.header__image img {
		width: 100%;
		height: 100%;
	}

	@media screen and (max-width: 1050px) {
		.header__container {
			flex-direction: column;
		}
		.header__content h1 {
			font-size: 45px;
			line-height: 55px;
		}
	}

	@media screen and (max-width: 650px) {
		.header__content-people {
			flex-direction: column;
		}
		.header__content h1 {
			font-size: 36px;
			line-height: 60px;
		}

		.header__content p {
			font-size: 16px;
			line-height: 24px;
		}

		.header__content-input input,
		.header__content-input button {
			font-size: 14px;
			line-height: 16px;
		}
	}

	@media screen and (max-width: 490px) {
		.header__content h1 {
			font-size: 30px;
			line-height: 48px;
		}

		.header__content p {
			font-size: 14px;
			line-height: 24px;
		}

		.header__content-input input,
		.header__content-input button {
			font-size: 12px;
			line-height: 16px;
		}
	}
</style>
