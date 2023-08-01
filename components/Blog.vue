<template>
	<div class="container" id="blog">
		<div class="blog">
			<div class="blog__heading">
				<h1 class="gradient__text">
					A lot is happening, <br />
					We are blogging about it.
				</h1>
			</div>
			<div class="blog__content">
				<div class="blog__content-groupA">
					<Article :imgUrl="imgUrl1" :date="date1" :text="text1" />
				</div>
				<div class="blog__content-groupB">
					<div>
						<Article :imgUrl="imgUrl2" :date="date2" :text="text2" />
					</div>
					<div>
						<Article :imgUrl="imgUrl3" :date="date3" :text="text3" />
					</div>
					<div>
						<Article :imgUrl="imgUrl4" :date="date4" :text="text4" />
					</div>
					<div>
						<Article :imgUrl="imgUrl5" :date="date5" :text="text5" />
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script setup>
	import imgUrl1 from "~/assets/img/blog01.png";
	const date1 = ref("Sep 26, 2021");
	const text1 = ref(
		"GPT-3 and Open  AI is the future. Let us exlore how it is?",
	);

	import imgUrl2 from "~/assets/img/blog02.png";
	const date2 = ref("Sep 26, 2021");
	const text2 = ref(
		"GPT-3 and Open  AI is the future. Let us exlore how it is?",
	);

	import imgUrl3 from "~/assets/img/blog03.png";
	const date3 = ref("Sep 26, 2021");
	const text3 = ref(
		"GPT-3 and Open  AI is the future. Let us exlore how it is?",
	);

	import imgUrl4 from "~/assets/img/blog04.png";
	const date4 = ref("Sep 26, 2021");
	const text4 = ref(
		"GPT-3 and Open  AI is the future. Let us exlore how it is?",
	);

	import imgUrl5 from "~/assets/img/blog05.png";
	const date5 = ref("Sep 26, 2021");
	const text5 = ref(
		"GPT-3 and Open  AI is the future. Let us exlore how it is?",
	);
</script>

<style>
	.blog {
		display: flex;
		flex-direction: column;
	}

	.blog__heading {
		width: 100%;
		text-align: left;

		margin-bottom: 5rem;
	}

	.blog__heading h1 {
		font-size: 62px;
		line-height: 75px;
		font-family: var(--font-family);
		font-weight: 800;
	}

	.blog__content {
		display: flex;
		flex-direction: row;
	}

	.blog__content-groupA {
		flex: 0.75;
		margin-right: 2rem;
	}

	.blog__content-groupB {
		flex: 1;
		display: grid;
		grid-template-columns: repeat(2, 1fr);
		grid-gap: 2rem;
		/* 
*/
	}

	@media screen and (max-width: 990px) {
		.blog__content {
			flex-direction: column-reverse;
		}
		.blog__content-groupA {
			margin: 2rem 0;
		}
		.blog__content-groupA .article {
			width: 48%;
		}

		.blog__content-groupA .article__image {
			height: 250px;
		}
	}

	@media screen and (max-width: 700px) {
		.blog__content-groupB {
			grid-template-columns: repeat(1, 1fr);
		}
		.blog__content-groupA .article {
			width: 100%;
		}

		.blog__heading h1 {
			font-size: 46px;
			line-height: 52px;
		}
	}

	@media screen and (max-width: 550px) {
		.blog__heading h1 {
			font-size: 34px;
			line-height: 42px;
		}
	}
</style>
