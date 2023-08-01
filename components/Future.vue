<template>
	<div class="container" id="features">
		<div class="future">
			<div class="future__heading">
				<h1 class="gradient__text">
					The Future is Now and You Just Need to Realize It. Step into Future
					Today. & Make it Happen.
				</h1>
				<p>Request Early Access to Get Started</p>
			</div>

			<div class="future__content">
				<div v-for="(item, index) in futureData" :key="index">
					<Feature :title="item.title" :text="item.text" />
				</div>
			</div>
		</div>
	</div>
</template>

<script setup>
	const futureData = ref([
		{
			title: "Improving end distrusts instantly",
			text: "From they fine john he give of rich he. They age and draw mrs like. Improving end distrusts may instantly was household applauded.",
		},
		{
			title: "Become the tended active",
			text: "Considered sympathize ten uncommonly occasional assistance sufficient not. Letter of on become he tended active enable to.",
		},
		{
			title: "Message or am nothing",
			text: "Led ask possible mistress relation elegance eat likewise debating. By message or am nothing amongst chiefly address.",
		},
		{
			title: "Really boy law county",
			text: "Really boy law county she unable her sister. Feet you off its like like six. Among sex are leave law built now. In built table in an rapid blush..",
		},
	]);
</script>

<style scoped>
	.future {
		width: 100%;
		display: flex;
		justify-content: space-between;
		flex-direction: row;
		margin: 3rem 0;
	}

	.future__heading {
		flex: 1;
		display: flex;
		justify-content: flex-start;
		align-items: flex-start;
		flex-direction: column;
		text-align: left;
		margin-right: 5rem;
	}

	.future__heading h1 {
		font-size: 34px;
		line-height: 45px;
		font-weight: 800;
		font-family: var(--font-family);
	}

	.future__heading p {
		color: var(--color-subtext);
		font-size: 16px;
		line-height: 30px;
		font-weight: 500;
		font-family: var(--font-family);
		margin-top: 2rem;
	}

	.future__content {
		flex: 1.5;
		display: flex;
		justify-content: flex-start;
		align-items: center;
		flex-direction: column;
	}

	@media screen and (max-width: 990px) {
		.future {
			flex-direction: column;
		}
		.future__heading {
			margin: 0 0 2rem 0;
		}
	}

	@media screen and (max-width: 550px) {
		.future__heading h1 {
			font-size: 28px;
			line-height: 38px;
		}
	}
</style>
