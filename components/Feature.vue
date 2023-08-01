<template>
	<div class="feature__container-feature">
		<div class="feature__container_feature-title">
			<div></div>
			<h1>{{ title }}</h1>
		</div>
		<div class="feature__container_feature-text">
			<p>{{ text }}</p>
		</div>
	</div>
</template>

<script setup>
	const props = defineProps(["text", "title"]);
	// const { text, title } = toRefs(props);
</script>

<style>
	.feature__container-feature {
		width: 100%;
		display: flex;
		justify-content: space-between;
		align-items: flex-start;
		flex-direction: row;

		margin: 1rem;
	}
	.feature__container_feature-title {
		flex: 1;
		max-width: 180px;
		margin-right: 2rem;
	}

	.feature__container_feature-title h1 {
		font-family: var(--font-family);
		font-weight: 800;
		font-size: 18px;
		line-height: 24px;
		letter-spacing: -0.04em;
		color: #fff;
	}

	.feature__container_feature-title div {
		width: 38px;
		height: 3px;
		background: var(--gradient-bar);
		box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
		margin-bottom: 0.25rem;
	}

	.feature__container_feature-text {
		flex: 2;
		max-width: 390px;
		display: flex;
	}

	.feature__container_feature-text p {
		font-family: var(--font-family);
		font-weight: 500;
		font-size: 14px;
		line-height: 24px;
		color: var(--color-text);
	}

	@media screen and (max-width: 550px) {
		.feature__container_feature-title h1 {
			font-size: 14px;
			line-height: 22px;
		}

		.feature__container_feature-text p {
			font-size: 12px;
			line-height: 20px;
		}
		.feature__container-feature {
			margin: 1rem 0;
		}
	}
</style>
