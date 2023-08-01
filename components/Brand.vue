<template>
	<div class="brand__container">
		<div>
			<img src="~/assets/img/google.png" alt="goggle" />
		</div>
		<div>
			<img src="~/assets/img/slack.png" alt="slack" />
		</div>
		<div>
			<img src="~/assets/img/atlassian.png" alt="atlassian" />
		</div>
		<div>
			<img src="~/assets/img/shopify.png" alt="shopify" />
		</div>
		<div>
			<img src="~/assets/img/dropbox.png" alt="dropbox" />
		</div>
	</div>
</template>

<script setup></script>

<style scoped>
	.brand__container {
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
		align-items: center;
	}

	.brand__container div {
		flex: 1;
		max-width: 150px;
		min-width: 120px;
		margin: 1rem;
	}
</style>
