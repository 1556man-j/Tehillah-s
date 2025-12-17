<script>
	import HeroImg from '$lib/assets/hero-img.svg';
	import ProductMockup from '$lib/assets/Product-Mockup.png';
	import WhiteBg from '$lib/assets/white.svg';
	import WhiteBgMobile from '$lib/assets/white-mobile.svg';
	import Union from '$lib/assets/Union.svg';
	import Highlight from '$lib/assets/Highlight1.svg';
	import Highlight3 from '$lib/assets/Highlight3.svg';
</script>

<main>
	<section
		class="flex flex-col justify-center py-5 max-w-[390px] lg:max-w-[585.99px] 2xl:max-w-[800px] mx-auto"
	>
		<image src={HeroImg} alt="Hero Image" class="w-full h-auto px-5" />

		<!--============================= cta for desktop================================== -->
		<button
			class="AmsiPro-Ultra hidden lg:flex cursor-pointer text-[#EFE5D5] font-normal bg-[#5C4033] w-[161px] 2xl:w-[180px] 2xl:h-12 2xl:text-[16px] text-center rounded-3xl h-10 items-center justify-center text-[12px] mx-auto mt-10"
		>
			Discover Our Story
		</button>
		<div class="flex lg:hidden items-center gap-0 max-w-44 mx-auto">
			<!-- ================cta for mobile ===================-->
			<div
				class="bg-[#5C4033] rounded-full p-0.5 mx-auto w-[29px] h-[29px] mt-10 flex items-center justify-center"
			>
				<img src={Union} alt="Decorative Line" class="mx-auto" />
			</div>
			<button
				class="AmsiPro-Ultra font-extrabold text-12 lg:hidden cursor-pointer text-[#EFE5D5] bg-[#5C4033] w-[135px] text-center rounded-3xl h-12 items-center justify-center flex mx-auto mt-10"
			>
				Buy Now
			</button>
		</div>
	</section>

	<section class="py-5">
		<div
			class="mx-auto max-w-[1500px] grid grid-cols-1 lg:grid-cols-2 justify-center gap-12 lg:gap-24 lg:px-20 relative"
		>
			<div class="absolute hidden lg:block">
				<img
					src={Highlight}
					alt="Highlight"
					class="mt-5 lg:-mt-40 w-[267.68px] lg:right-[25%] 2xl:w-[350px]"
				/>
			</div>

			<!-- ================= IMAGE SIDE ================= -->
			<div class="relative flex w-full">
				<!-- ================Background Shape============= -->
				<!-- for desktop -->
				<img
					src={WhiteBg}
					alt=""
					class="absolute top-10 left-1 z-10 max-w-[6000px] hidden lg:block w-full 2xl:w-[800px] 2xl:-left-30"
				/>
				<!-- for mobile -->
				<img
					src={WhiteBgMobile}
					alt=""
					class="absolute top-10 left-0 z-10 w-full sm:h-[480.52px] h-[430px] block lg:hidden"
				/>
				<!-- Product Image -->
				<img
					src={ProductMockup}
					alt="Tehillah’s Garri Ijebu"
					class="relative z-20 w-[330.10px] sm:w-[400px] xl:w-[454.12px] xl:h-[575.62px] 2xl:w-[900px] 2xl:h-[700px] left-1/2 transform -translate-x-1/2"
				/>

				<!-- Badge 1 -->
				<div
					class="absolute z-30 lg:top-[35px] lg:left-[75px] -bottom-25 left-[20%] sm:-bottom-15 md:left-[33%] 2xl:left-[1%] sm:left-[30%] w-[90px] h-[90px] lg:w-[114px] lg:h-[114px] 2xl:w-[130px] 2xl:h-[130px]
				rounded-full bg-[#985C37] flex flex-col items-center justify-center text-white leading-none"
				>
					<h2 class="text-[28px] lg:text-[37px] font-extrabold AmsiProCond-Ultra">100%</h2>
					<p class="text-[14px] lg:text-[18px] AmsiPro-SemiBold">Organic</p>
				</div>

				<!-- Badge 2 -->
				<div
					class="absolute z-30 lg:top-[155px] lg:left-[7px] -bottom-27 sm:-bottom-20 left-[45%] sm:left-[45%] 2xl:-left-[15%] w-[90px] h-[90px] lg:w-[114px] lg:h-[114px] 2xl:w-[130px] 2xl:h-[130px]
				rounded-full bg-[#985C37] flex flex-col items-center justify-center text-white leading-none"
				>
					<h2 class="text-[28px] lg:text-[37px] font-extrabold AmsiProCond-Ultra">Gluten</h2>
					<p class="text-[14px] lg:text-[18px] AmsiPro-SemiBold">Free</p>
				</div>

				<!-- Badge 3 -->
				<div
					class="absolute z-30 lg:top-[305px] lg:left-[-35px] -bottom-15 sm:-bottom-9 left-[67%] sm:left-[58%] md:left-[56%] 2xl:-left-[20%] w-[90px] h-[90px] lg:w-[114px] lg:h-[114px] 2xl:w-[130px] 2xl:h-[130px]
				rounded-full bg-[#985C37] flex flex-col items-center justify-center text-white leading-none"
				>
					<h2 class="text-[28px] lg:text-[37px] font-extrabold AmsiProCond-Ultra">NO</h2>
					<p class="text-[14px] lg:text-[18px] AmsiPro-SemiBold">GMO's</p>
				</div>
			</div>

			<div class="lg:hidden block mx-auto pt-10">
				<img
					src={Highlight3}
					alt="Highlight"
					class="mt-5  w-[267.68px]  hiddden lg:block"
				/>
			</div>

			<!-- ================= TEXT SIDE ================= -->
			<div
				class="w-full flex flex-col gap-6 text-center mt-10 md:max-w-[486px] 2xl:max-w-[700px] mx-auto px-5 pt-0 lg:pt-0"
			>
				<h1
					class="uppercase text-[#5C4033] text-[62px] 2xl:text-[72px] font-black
				AmsiProCond-Ultra leading-none"
				>
					Welcome to <br />
					<span class="text-[#985C37]">Tehillah’s Table</span>
				</h1>

				<p
					class="text-[#5C4033] text-[20px] 2xl:text-[24px] leading-snug
				AmsiPro-SemiBold font-extralight"
				>
					Here, we celebrate the beauty of everyday food crafted with care and rooted in the places
					and people that shape it. Sit with us and enjoy a taste of home, made with honesty, pride,
					and heart.
				</p>
			</div>
		</div>
	</section>
</main>
