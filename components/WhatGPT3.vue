<template>
	<div class="container" id="wgpt3">
		<div class="whatgpt3__container">
			<div class="whatgpt3__feature">
				<Feature :title="featureTitle1" :text="featureText1" />
			</div>
			<div class="whatgpt3__heading">
				<h1 class="gradient__text">
					The possibilities are beyond your imagination
				</h1>
				<p>Explore the library</p>
			</div>

			<div className="whatgpt3__content">
				<Feature :title="featureTitle2" :text="featureText2" />
				<Feature :title="featureTitle3" :text="featureText3" />
				<Feature :title="featureTitle4" :text="featureText4" />
			</div>
		</div>
	</div>
</template>

<script setup>
	const featureTitle1 = ref("What is GPT-3");
	const featureText1 = ref(
		"We so opinion friends me message as delight. Whole front do of plate heard oh ought. His defective nor convinced residence own. Connection has put impossible own apartments boisterous. At jointure ladyship an insisted so humanity he. Friendly bachelor entrance to on by.",
	);
	const featureTitle2 = ref("Chatbots");
	const featureText2 = ref(
		"We so opinion friends me message as delight. Whole front do of plate heard oh ought.",
	);

	const featureTitle3 = ref("Knowledgebase");
	const featureText3 = ref(
		"At jointure ladyship an insisted so humanity he. Friendly bachelor entrance to on by. As put impossible own apartments",
	);
	const featureTitle4 = ref("Education");
	const featureText4 = ref(
		"At jointure ladyship an insisted so humanity he. Friendly bachelor entrance to on by. As put impossible own apartments",
	);
</script>

<style>
	.whatgpt3__container {
		display: flex;
		flex-direction: column;

		padding: 2rem;
		background: var(--color-footer);

		/* ff 3.6+ */
		background: -moz-radial-gradient(
			circle at 30% -100%,
			#042c54 25%,
			rgba(4, 44, 84, 1) 85%,
			rgba(27, 120, 222, 1) 100%
		);

		/* safari 5.1+,chrome 10+ */
		background: -webkit-radial-gradient(
			circle at 30% -100%,
			#042c54 25%,
			rgba(4, 44, 84, 1) 85%,
			rgba(27, 120, 222, 1) 100%
		);

		/* opera 11.10+ */
		background: -o-radial-gradient(
			circle at 30% -100%,
			#042c54 25%,
			rgba(4, 44, 84, 1) 85%,
			rgba(27, 120, 222, 1) 100%
		);

		/* ie 10+ */
		background: -ms-radial-gradient(
			circle at 30% -100%,
			#042c54 25%,
			rgba(4, 44, 84, 1) 85%,
			rgba(27, 120, 222, 1) 100%
		);

		/* global 92%+ browsers support */
		background: radial-gradient(
			circle at 30% -100%,
			#042c54 25%,
			rgba(4, 44, 84, 1) 85%,
			rgba(27, 120, 222, 1) 100%
		);

		filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
		margin: 2rem 0rem;
	}

	.whatgpt3__feature {
		display: flex;
	}

	.whatgpt3__feature .feature__container-feature {
		margin: 0;
	}

	.whatgpt3__feature .feature__container_feature-title {
		max-width: 700px;
	}

	.whatgpt3__heading {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;

		margin: 4rem 0rem 2rem;
	}
	.whatgpt3__heading h1 {
		font-size: 30px;
		font-family: var(--font-family);
		font-style: normal;
		font-weight: 800;
		line-height: 45px;

		max-width: 510px;
	}

	.whatgpt3__heading p {
		font-family: var(--font-family);
		font-weight: 500;
		font-size: 16px;
		line-height: 30px;
		color: var(--color-subtext);
		cursor: pointer;
	}

	.whatgpt3__content {
		display: flex;
		flex-wrap: wrap;
		flex-direction: row;

		margin-top: 2rem;
	}
	.whatgpt3__content .feature__container-feature {
		flex: 1;
		margin: 1rem;
		min-width: 210px;
		display: unset;
		flex-direction: column;
	}

	.whatgpt3__content .feature__container_feature-text {
		margin-top: 0.5rem;
	}

	@media screen and (max-width: 850px) {
		.whatgpt3__heading {
			flex-direction: column;
			align-items: flex-start;
			margin-bottom: 0rem;
		}
		.whatgpt3__heading p {
			margin-top: 1rem;
		}
	}

	@media screen and (max-width: 650px) {
		.whatgpt3__feature .feature__container-feature {
			flex-direction: column;
		}

		.whatgpt3__feature .feature__container_feature-text {
			margin-top: 0.5rem;
		}

		.whatgpt3__heading h1 {
			font-size: 28px;
			line-height: 40px;
		}
	}

	@media screen and (max-width: 350px) {
		.whatgpt3__content .feature__container-feature {
			margin: 1rem 0;
			min-width: 100%;
		}
	}
</style>
