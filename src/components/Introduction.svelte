<script>
	import Highlight from '$lib/assets/Highlight2.svg';
	import Emoji from '$lib/assets/emoji.svg';
	import ProductMockup from '$lib/assets/Product-Mockup.png';
	import vectorImg from '$lib/assets/vector-img.svg';
	import BgLine from '$lib/assets/bg-line.svg';
	import Union from '$lib/assets/Union.svg';
</script>

<main class="relative">
	<!-- ===========bg lmage show starting from laptop view=========== -->
	<div>
		<img
			src={BgLine}
			alt="Background Line"
			class="absolute -top-30 left-0 h-auto z-0 hidden lg:block opacity-50 w-full"
		/>
	</div>

	<!-- =================header text=============== -->
	<section class="lg:px-20 px-5 leading-none">
		<h1 class="text-[50px] text-[#5C4033] 2xl:text-[72px] AmsiProCond-Ultra">
			Introducing<br />
			<span class="text-[#985C37]">Tehillah’s Garri Ijebu</span>
		</h1>
		<img
			src={Highlight}
			alt="Highlight"
			class="mt-5 lg:-mt-68 w-[129.19px] lg:right-[25%] 2xl:w-[150px] ml-auto relative"
		/>
	</section>
	<section class="relative lg:-top-80 overflow-x-hidden mx-auto">
		<!-- ===============first box========= -->
		<div
			class="rounded-xl bg-[#CE9C7D] relative flex flex-col gap-5 z-20 p-5 max-w-[90%] sm:max-w-[393px] sm:mx-auto mt-20 pb-12 lg:-right-90 lg:top-69 2xl:-right-99 lg:rotate-6 lg:max-w-[473px] mx-auto"
		>
			<div
				class="w-[78.1px] h-[78.1px] absolute z-20 top-0 bg-white p-2 rounded-full -translate-y-1/2 left-1/2 transform -translate-x-1/2"
			>
				<img src={Emoji} alt="emoji" class=" w-full h-full" />
			</div>
			<h2 class="AmsiPro-Ultra text-[34px] text-center text-white leading-none font-black pt-5">
				TASTE MADE WITH PATIENCE
			</h2>
			<p
				class="text-[#5C4033] text-[15px] lg:text-[18px] 2xl:text-[19px] leading-none text-center AmsiPro-SemiBold relative z-30"
			>
				From cassava peeled by steady hands to grains dried under open sky, this is food made the
				way our mothers taught us. “Dídùn ló pọ̀ sí i” — what is made with care tastes sweeter.
			</p>
			<!-- imaage laying on the text -->
			<div>
				<img
					src={vectorImg}
					alt="vector-img"
					class="absolute bottom-20 right-20 lg:right-30 2xl:right-25 2xl:w-[139.49px] lg:bottom-21 w-[122.49px] h-auto z-10"
				/>
			</div>
		</div>
		<!-- =====product mockup============ -->
		<div
			class="max-w-[395px] 2xl:max-w-[503px] 2xl:h-[700px] h-[501px] relative z-20 -top-15 lg:top-40 mx-auto overflow-x-hidden"
		>
			<img src={ProductMockup} alt="Tehillah’s Garri Ijebu" class="mx-auto w-full -rotate-10" />
		</div>

		<!-- ================cta & rating for laptop ===================-->
		<div class="relative 2xl:-top-80 -top-40 2xl:left-100 left-90 z-90">
			<div class="lg:flex items-center gap-0 max-w-[450px] mx-auto hidden">
				<div
					class="bg-[#5C4033] rounded-full p-0.5 mx-auto w-[29px] h-[29px] flex items-center justify-center"
				>
					<img src={Union} alt="Decorative Line" class="mx-auto" />
				</div>
				<button
					class="AmsiPro-Ultra font-extrabold text-12 lg:flex hidden cursor-pointer -ml-2 text-[#EFE5D5] bg-[#5C4033] w-[135px] text-center rounded-3xl h-12 items-center justify-center mx-auto "
				>
					Buy Now
				</button>
				<svg
					width="140"
					height="24"
					viewBox="0 0 140 24"
					fill="none"
					xmlns="http://www.w3.org/2000/svg"
					class="ml-10"
				>
					<!-- Star Path -->
					<defs>
						<path
							id="star"
							d="M12 2.5l2.95 6 6.63.96-4.79 4.67 1.13 6.6L12 17.77 6.08 20.73l1.13-6.6L2.42 9.46l6.63-.96L12 2.5z"
						/>

						<!-- Half fill mask -->
						<clipPath id="half">
							<rect x="0" y="0" width="12" height="24" />
						</clipPath>
					</defs>

					<!-- Full Stars -->
					<g fill="#5C4033" stroke="#5C4033" stroke-width="1">
						<use href="#star" x="0" />
						<use href="#star" x="28" />
						<use href="#star" x="56" />
						<use href="#star" x="84" />
					</g>

					<!-- Empty 5th Star Outline -->
					<use href="#star" x="112" fill="none" stroke="#5C4033" stroke-width="1" />

					<!-- Half Filled 5th Star -->
					<use href="#star" x="112" fill="#5C4033" clip-path="url(#half)" />
				</svg>
        <p class="text-[#5C4033] AmsiPro-SemiBold text-[16px] ml-2">325 Reviews</p>
			</div>
		</div>
		<!-- =============second box=========== -->
		<div
			class="rounded-xl bg-[#CE9C7D] relative flex flex-col gap-5 z-10 py-5 px-10 lg:pr-10 2xl:pr-15 max-w-[90%] sm:max-w-[393px] h-[271px] justify-center items-center 2xl:w-[473px] mx-auto -mt-15 pb-5 lg:-left-80 lg:bottom-29 2xl:bottom-50 lg:-rotate-4 lg:max-w-[473px]"
		>
			<div
				class="w-[78.1px] h-[78.1px] absolute z-20 top-0 bg-white p-2 rounded-full -translate-y-1/2 left-1/2 transform -translate-x-1/2"
			>
				<img src={Emoji} alt="emoji" class=" w-full h-full" />
			</div>
			<h2 class="AmsiPro-Ultra text-[34px] text-center text-white leading-none font-black pt-5">
				FROM ROOT <br />TO GRAIN
			</h2>
			<p
				class="text-[#5C4033] text-[15px] leading-none text-center AmsiPro-SemiBold lg:text-[18px] 2xl:text-[19px]"
			>
				Cassava pulled from earth. Hands that know what they’re doing. A taste that carries memory
				in every crunch.
			</p>
		</div>

		<!-- ===============third box======= -->
		<div
			class="rounded-xl bg-[#CE9C7D] relative flex flex-col gap-5 z-10 py-5 px-15 max-w-[90%] sm:max-w-[393px] mx-auto mt-20 pb-12 lg:relative lg:-right-85 lg:bottom-62 2xl:bottom-85 lg:-rotate-4 lg:max-w-[473px] h-[271px] items-center justify-center"
		>
			<div
				class="w-[78.1px] h-[78.1px] absolute z-20 top-0 bg-white p-2 rounded-full -translate-y-1/2 left-1/2 transform -translate-x-1/2"
			>
				<img src={Emoji} alt="emoji" class=" w-full h-full" />
			</div>
			<h2 class="AmsiPro-Ultra text-[34px] text-center text-white leading-none font-black pt-5">
				WHAT HOME <br />TASTES LIKE
			</h2>
			<p
				class="text-[#5C4033] text-[15px] lg:text-[18px] 2xl:text-[19px] leading-none text-center AmsiPro-SemiBold relative z-30"
			>
				Bright, crisp garri roasted the Ijebu way. It carries sunshine, stories, and the small joys
				that follow us everywhere.
			</p>
		</div>
	</section>
</main>
