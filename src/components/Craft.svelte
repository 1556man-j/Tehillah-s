<script>
	import Vector3 from '$lib/assets/Vector3.svg';
	import HighlightCraft from '$lib/assets/Highlight-craft.svg';
	import CraftImg from '$lib/assets/craft-img.png';
</script>

<main class="bg-[#5C4033]">
	<img
		src={Vector3}
		alt="vector3"
		class="relative 2xl:bottom-0 left-0 -mt-15 lg:-mt-30 w-full h-auto z-99 lg:block rotate-180"
	/>
	<section id="craft">
		<h1
			class="AmsiProCond-Ultra text-5xl sm:text-[68px] lg:text-[84px] 2xl:text-[100px] text-center text-[#CE9C7D] leading-none mt-30 px-5"
		>
			Made By Hand,<br /><span class="text-[#F3E7D4]"> Made With Heart</span>
		</h1>
	</section>

	<section>
		<div class="flex flex-col lg:flex-row overflow-x-hidden">
			<div class="flex flex-col w-full gap-5 px-5 mt-20 xl:px-30 lg:px-20 md:px-20 sm:px-10">
				<h3 class="AmsiPro-Bold text-[16px] 2xl:text-2xl uppercase text-[#CE9C7D]">The Craft</h3>
				<h1 class="AmsiPro-Ultra text-[32px] text-[#F3E7D4] leading-snug font-black">
					Every bowl begins with real hands and real patience.
				</h1>
				<p class="text-[#F3E7D4] text-xl AmsiPro-SemiBold">
					From cassava grown in nearby villages to the slow roasting that brings out its clean,
					crisp taste, nothing here is rushed. Women who have mastered this craft sift, turn, and
					toast each batch with the same care passed down through generations.
				</p>
				<p class="AmsiPro-Bold text-xl text-[#F3E7D4]">
					This is why Tehillah’s Garri Ijebu tastes the way it does: honest, familiar, and full of
					character.
				</p>
				<button
					class="text-[#5C4033] text-[14px] bg-[#F3E7D4] w-[161px] h-[39px] flex justify-center items-center rounded-full AmsiPro-Ultra"
					>Bring Home a Bag</button
				>
				<div>
					<img
						src={HighlightCraft}
						alt="highlight-craft"
						class="relative w-full max-w-[185px] mx-auto py-10"
					/>
				</div>
			</div>
			<div class="relative min-h-120 xl:min-h-200 z-0 border w-full">
				<div class="relative -right-10 border w-full">
					<div
						class="absolute top-0 right-0 max-w-[388.65px] max-h-[430.46px] lg:max-w-[450px] lg:max-h-[500px] xl:max-w-[660px] xl:max-h-[731px] border-13 border-white rounded-4xl overflow-hidden z-10 -rotate-10"
					>
						<img
							src={CraftImg}
							alt="craft-img"
							class="w-full h-full object-contain object-center"
						/>
					</div>
					<div
						class="absolute top-0 right-0 max-w-[388.65px] max-h-[430.46px] lg:max-w-[450px] lg:max-h-[500px] xl:max-w-[660px] xl:max-h-[731px] border-13 border-white rounded-4xl overflow-hidden z-99990 shadow-2xl"
					>
						<img
							src={CraftImg}
							alt="craft-img"
							class="mx-auto w-full h-full object-contain object-center"
						/>
					</div>
				</div>
			</div>
		</div>
	</section>
</main>
