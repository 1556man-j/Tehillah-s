<script>
	import StoryImage1 from '$lib/assets/A_woman_peeling_cassava 1.png';
	import StoryImage2 from '$lib/assets/mom.jpg';
	import StoryImage3 from '$lib/assets/steptodown.com227463 1 (1).png';
	import Combo from './Combo.svelte';
	import Introduction from './Introduction.svelte';
	import Reviews from './Reviews.svelte';
</script>

<main id="story" class="lg:mt-40 xl:mt-30 mt-50">
	<!-- ===================story h2 text =================-->
	<section>
		<div>
			<h2
				class="text-[#5C4033] text-[38px] lg:text-[62px] 2xl:text-[72px] font-black
				AmsiProCond-Ultra leading-none text-center mx-auto lg:max-w-[994px] max-w-[592px] px-5 "
			>
				At Tehillah’s Table, we honour the flavours we grew up with and share them the way <span
					class="text-[#985C37]">they were passed down to us.</span
				>
			</h2>
		</div>
	</section>

	<section class="mt-20 lg:mt-30 mb-10 overflow-x-hidden">
		<div class="grid grid-cols-1 lg:grid-cols-2">
			<div class="relative lg:h-[688.1px] 2xl:h-[900px] h-[1000px] flex justify-center items-center">
				<div class=" w-full h-full relative">
					<div
						class="md:w-[311px] md:h-[495px] xl:w-[311px] xl:h-[495px] lg:w-[254.04px] lg:h-[404.34px] 2xl:w-[400px] 2xl:h-[640px] w-[254.04px] h-[404.34px] border-13 border-white rounded-xl overflow-hidden -rotate-[9.45deg] absolute lg:-left-12  left-[10%] md:left-[30%] top-10 lg:top-1/2 lg:-translate-y-1/2 z-0"
					>
						<img
							src={StoryImage3}
							alt="Story-img1"
							class="w-full h-full mx-auto rounded-xl object-cover"
						/>
					</div>
					<div
						class="md:w-[311px] md:h-[495px] xl:w-[311px] xl:h-[495px] 2xl:w-[400px] 2xl:h-[640px] lg:w-[254.04px] lg:h-[404.34px] w-[254.04px] h-[404.34px] border-13 border-white rounded-xl overflow-hidden -rotate-[2.59deg] absolute lg:top-1/4 top-1/4 lg:left-[94.97px] xl:left-[195px] 2xl:left-[220px] md:left-[45%] md:top-1/3 left-[35%] z-10"
					>
						<img src={StoryImage1} alt="Story-img1" class="w-full h-full mx-auto rounded-xl" />
					</div>
					<div
						class="md:w-[311px] md:h-[495px] xl:w-[311px] xl:h-[495px] 2xl:w-[400px] 2xl:h-[640px] lg:w-[254.04px] lg:h-[404.34px] w-[254.04px] h-[404.34px] border-13 border-white rounded-xl overflow-hidden rotate-[7.1deg] absolute lg:left-[253.61px] xl:left-[353.61px] 2xl:left-[420px] left-[15%] md:left-[30%] lg:top-1/2 bottom-[10%] md:-bottom-[10%] lg:-translate-y-1/2 z-20"
					>
						<img
							src={StoryImage2}
							alt="Story-img1"
							class="w-full h-full mx-auto object-cover object-bottom-center"
						/>
					</div>
				</div>
			</div>
			<div class="flex flex-col justify-center mx-auto max-w-[486px] 2xl:max-w-[700px] gap-5 relative px-5  xl:w-full">
				<h3 class="text-[#CE9C7D] text-[16px] font-bold md:mt-40 lg:mt-0 uppercase 2xl:text-[20px]">Our Story</h3>
				<h2 class="text-[27px] font-black leading-none 2xl:text-[38px]">
					Every journey starts somewhere. Ours begins with Garri Ijebu.
				</h2>
				<p class="text-[#5C4033] text-[20px] AmsiPro-SemiBold font-normal 2xl:text-[24px] leading-snug">
					It is made from cassava grown in Ikenne and nearby towns, then peeled, fermented, roasted,
					and sieved in small batches. Local women guide each step with care, keeping the craft
					alive. The taste is clean, crisp, and familiar, carrying the quiet comfort of home.
				</p>
			</div>
		</div>
	</section>
  <Introduction/>
  <Combo/>
  <Reviews/>
</main>
