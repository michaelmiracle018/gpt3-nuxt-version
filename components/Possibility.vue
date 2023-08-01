<template>
	<div class="container" id="possibility">
		<div class="possibility">
			<div class="possibility__image">
				<img src="~/assets/img/possibility.png" alt="possibility" />
			</div>

			<div class="possibility__content">
				<h4>Request Early Access to Get Started</h4>
				<h1 class="gradient__text">
					The possibilities are <br />
					beyond your imagination
				</h1>
				<p>
					Yet bed any for travelling assistance indulgence unpleasing. Not
					thoughts all exercise blessing. Indulgence way everything joy
					alteration boisterous the attachment. Party we years to order allow
					asked of.
				</p>
				<h4>Request Early Access to Get Started</h4>
			</div>
		</div>
	</div>
</template>

<script setup></script>

<style scoped>
	.possibility {
		display: flex;
		flex-direction: row;
		margin-bottom: 2rem;
	}

	.possibility__image {
		flex: 1;
		display: flex;
		justify-content: flex-start;
		align-items: center;
		margin-right: 2rem;
	}
	.possibility__image img {
		width: 100%;
		height: 100%;
		object-fit: cover;
	}
	.possibility__content {
		flex: 1;
		display: flex;
		flex-direction: column;
		justify-content: flex-end;
		align-items: flex-start;
	}
	.possibility__content h4 {
		font-family: var(--font-family);
		font-weight: 500;
		font-size: 16px;
		line-height: 30px;
		color: #71e5ff;
	}

	.possibility__content h4:last-child {
		color: #ff8a71;
	}

	.possibility__content h1 {
		font-family: var(--font-family);
		font-weight: 800;
		font-size: 34px;
		line-height: 45px;
		margin: 1rem 0;
	}

	.possibility__content p {
		color: var(--color-text);
		font-family: var(--font-family);
		font-weight: 400;
		font-size: 16px;
		line-height: 30px;

		margin-bottom: 2rem;
	}

	@media screen and (max-width: 950px) {
		.possibility {
			flex-direction: column;
		}

		.possibility__image {
			margin: 1rem 0;
		}

		.possibility__image img {
			width: 100%;
			height: 100%;
		}

		.possibility__content {
			margin-top: 2rem;
		}
	}

	@media screen and (max-width: 700px) {
		.possibility__image img {
			width: 100%;
			height: 100%;
		}
	}
</style>
