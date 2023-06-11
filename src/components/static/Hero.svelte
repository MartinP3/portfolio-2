<script>
	import { fly, blur } from 'svelte/transition';
	import { onMount } from 'svelte';

	let visible = false;

	onMount(() => {
		visible = true;
	});
</script>

<section class="heroSection flex flex-col justify-center items-center mb-36 md:mb-16 pb-32">
	{#if visible}
		<div transition:fly={{ y: 200, duration: 700 }}>
			<div class="outerBg p-4">
				<div class="uppercase innerBg p-3 flex flex-col">
					{#if visible}
						<div transition:blur={{ delay: 400, duration: 500 }}>
							<span class="char">M</span>
							<span class="char">a</span>
							<span class="char">r</span>
							<span class="char">t</span>
							<span class="char">i</span>
							<span class="char">n</span>
						</div>
					{/if}
					{#if visible}
						<span
							transition:blur={{ delay: 400, duration: 500 }}
							class="secondText text-center -mt-10">Pedersen</span
						>
					{/if}
				</div>
			</div>
			{#if visible}
				<div
					transition:blur={{ delay: 600, duration: 700 }}
					class="my-4 text-white text-center subText"
				>
					Frontend Developer
				</div>
			{/if}
		</div>
	{/if}
</section>

<style>
	::selection {
		background-color: #1d1d1d;
		color: #de6431;
	}

	.heroSection {
		height: 100vh;
		width: 100%;
		font-family: 'Poppins', sans-serif;
		background-color: #2d1308;
		opacity: 0.8;
		background-image: radial-gradient(circle at center center, #de6431, #2d1308),
			repeating-radial-gradient(
				circle at center center,
				#de6431,
				#de6431,
				5px,
				transparent 36px,
				transparent 18px
			);
		background-blend-mode: multiply;
	}

	.outerBg {
		background-color: #933007;
	}

	.innerBg {
		background-color: #de6431;
	}

	.char {
		display: inline-block;
		color: transparent;
		font-size: 8rem;
		-webkit-text-stroke: 2px #fff;
		transition: transform 0.3s ease;
	}

	.secondText {
		font-size: 5rem;
		color: transparent;
		-webkit-text-stroke: 2px #fff;
		transition: transform 0.3s ease;
	}

	.char:hover,
	.secondText:hover {
		transform: scale(1.2);
		color: #fff;
	}

	.subText {
		font-size: 1.2rem;
		letter-spacing: 0.1rem;
	}

	@media (max-width: 600px) {
		.char {
			font-size: 7rem;
		}
	}

	@media (max-width: 542px) {
		.char {
			font-size: 6rem;
		}
		.secondText {
			font-size: 3.5rem;
		}
	}

	@media (max-width: 478px) {
		.char {
			font-size: 5rem;
		}
		.secondText {
			font-size: 3rem;
		}
	}

	@media (max-width: 412px) {
		.char {
			font-size: 4rem;
			margin-bottom: 0.8rem;
		}
		.secondText {
			font-size: 3rem;
		}
	}
</style>
