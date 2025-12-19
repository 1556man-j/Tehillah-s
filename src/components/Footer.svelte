<script>
	import Divider from '$lib/assets/dvide-line.svg';
	import FooterBg from '$lib/assets/footer-bg.svg';
	import ProductMockup from '$lib/assets/Product-Mockup.png';
	import FooterLogo from '$lib/assets/footer-logo.svg';

	import Instagram from '$lib/assets/insta.svg';
	import Twitter from '$lib/assets/twiter.svg';
	import Facebook from '$lib/assets/facebook.svg';
</script>

<footer class="relative -top-30 lg:-top-60 max-h-90">
	<img src={Divider} alt="divider" class="w-full h-auto absolute z-10 -top-10 lg:-top-20 left-0" />
	<img
		src={FooterBg}
		alt="footer-bg"
		class="w-[120%] h-auto absolute z-0 left-0 -top-7 lg:-top-10"
	/>
	<section class="bg-[#F3E7D4] px-5 relative lg:top-30 overflow-hidden pb-40 lg:pb-60" >
		<div class="flex flex-col lg:flex-row max-w-[1300px] mx-auto  bg-[#F3E7D4] items-center">
			<!-- =====product mockup============ -->
			<div
				class="max-w-[813px] xl:w-[599px] 2xl:max-w-[700px] xl:h-[759px] 2xl:h-[890px] h-[704px] relative z-20 top-0 lg:top-10 xl:top-40 mx-auto lg:ml-0 overflow-x-hidden"
			>
				<img src={ProductMockup} alt="Tehillah’s Garri Ijebu" class="mx-auto w-full -rotate-10" />
			</div>

			<div
				class="max-w-[392px] sm:max-w-[550px] flex flex-col gap-10 -mt-30 lg:mt-0 relative lg:top-40 z-99"
			>
				<h1 class="AmsiProCond-Ultra text-[55px] leading-none text-[#5C4033] uppercase">
					A seat at <br /><span class="text-[#985C37]">Tehillah’s Table.</span>
				</h1>
				<p class="AmsiPro-SemiBold text-lg leading-snug">
					Be the first to know when new batches drop, where to find us, and what we’re crafting
					next.
				</p>
				<form class="flex items-center bg-white rounded-full pl-3 pr-1 py-2 justify-between">
					<input
						type="email"
						placeholder="Enter your email address"
						class="w-full lg:w-[350px] h-[50px] border-0 px-5 text-[#5C4033] text-lg outline-none placeholder:text-[#5C4033] focus:outline-none focus:ring-0 focus:border-transparent"
					/>
					<button
						type="submit"
						class="w-[157px] lg:w-[150px] h-[50px] bg-[#5C4033] text-[#F3E7D4] rounded-full AmsiPro-Bold text-[16px]"
						>Get Listed</button
					>
				</form>
				<div class="flex gap-3">
					{#each [Instagram, Twitter, Facebook] as icon}
						<div class="rounded-full bg-white p-3 hover:scale-110 transition">
							<img src={icon} alt="social" class="w-8 h-8 cursor-pointer" />
						</div>
					{/each}
				</div>
			</div>
		</div>
		<div class="absolute -bottom-32 2xl:-bottom-5 xl:-bottom-17 lg:-bottom-20">
			<img src={FooterLogo} alt="footer-logo" class="w-full h-[325px] mx-auto mb-0" />
		</div>
	</section>
</footer>
