<template>
	<div class="article">
		<div class="article__image">
			<img :src="imgUrl" alt="imgUrl" />
		</div>
		<div class="article__content">
			<div>
				<p>{{ date }}</p>
				<h3>{{ text }}</h3>
			</div>
			<p>Read Full Article</p>
		</div>
	</div>
</template>

<script setup>
	const props = defineProps(["text", "imgUrl", "date"]);
</script>

<style scoped>
	.article {
		width: 100%;
		height: 100%;

		display: flex;
		flex-direction: column;
		background: var(--color-footer);
	}

	.article__image {
		width: 100%;
		height: 100%;
		background: var(--color-bg);
	}

	.article__image img {
		width: 100%;
		height: 100%;
	}

	.article__content {
		display: flex;
		flex-direction: column;
		justify-content: space-between;

		padding: 1rem 1.5rem;
		height: 100%;
	}

	.article__content p {
		font-family: var(--font-family);
		font-size: 11.65px;
		font-weight: 700;
		line-height: 35px;

		color: #fff;
	}

	.article__content h3 {
		font-family: var(--font-family);
		font-size: 25.11px;
		font-weight: 800;
		line-height: 30.3px;

		color: #fff;
		margin-bottom: 5rem;
		cursor: pointer;
	}

	.article__content p:last-child {
		cursor: pointer;
	}

	@media screen and (max-width: 550px) {
		.article__content h3 {
			font-size: 18px;
			line-height: 25p;
		}
	}
</style>
