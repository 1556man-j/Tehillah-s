<script>
  import CassavaLeaf from '$lib/assets/Cassava-Leaf.svg';
  import Layer1 from '$lib/assets/Layer_1.svg';
	import Carousel from './Carousel.svelte';
  import Vector3 from '$lib/assets/Vector3.svg';

</script>

<main class="bg-white pt-30 relative z-0 pb-30">
  <div class="absolute top-0 right-0 w-full z-0 hidden lg:block 2xl::max-w-[525px] lg:max-w-[370px] overflow-hidden" >
    <img src={Layer1} alt="Decorative Layer" class="w-full h-full overflow-hidden" />
  </div>
  <div class="absolute -top-10 left-0 w-[369.78px] z-0 hidden lg:block ">
    <img src={CassavaLeaf} alt="Cassava Leaf" class="w-full h-full" />
  </div>
	<section class="relative z-10">
		<h1
			class="AmsiProCond-Ultra text-5xl sm:text-[68px] lg:text-[84px] 2xl:text-[100px] text-center text-[#5C4033] leading-none mt-30 px-5 uppercase"
		>
			Don’t just take<br /><span class="text-[#985C37]">our word for it</span>
		</h1>
	</section>
  <Carousel/>
</main>
