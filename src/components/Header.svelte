<script>
	import Instagram from '$lib/assets/insta.svg';
	import Twitter from '$lib/assets/twiter.svg';
	import Facebook from '$lib/assets/facebook.svg';

	let mobileOpen = false;

	const links = [
		{ name: 'Our Story', href: '#story' },
		{ name: 'Craft', href: '#craft' },
		{ name: 'Shop', href: '#shop' }
	];

	// $: {
	// 	document.body.style.overflow = mobileOpen ? 'hidden' : '';
	// }
</script>

<nav class="relative z-50 ">
	<!-- ================= DESKTOP HEADER ================= -->
	<div class="hidden lg:flex items-center justify-between px-5 py-6 pb-20 lg:px-20">
		<div class="flex gap-3">
			{#each [Instagram, Twitter, Facebook] as icon}
				<div class="rounded-full bg-white p-2 hover:scale-110 transition">
					<img src={icon} alt="social" class="w-4 h-4 cursor-pointer" />
				</div>
			{/each}
		</div>

		<ul class="flex gap-4">
			{#each links as link}
				<li>
					<a
						href={link.href}
						class="bg-[#5C4033] text-[#EFE5D5] w-[131px] h-10 rounded-3xl flex items-center justify-center hover:opacity-90 transition"
					>
						{link.name}
					</a>
				</li>
			{/each}
		</ul>

		<a
			href="#contact"
			class="border-2 border-[#5C4033] text-[#5C4033] w-[180px] h-10 rounded-3xl flex items-center justify-center hover:bg-[#5C4033] hover:text-[#EFE5D5] transition"
		>
			Contact
		</a>
	</div>

	<!-- ================= MOBILE HEADER ================= -->
	<div class="flex lg:hidden items-center justify-between px-5 py-6">
		<button
			on:click={() => (mobileOpen = !mobileOpen)}
			class="text-[#5C4033]"
			aria-label="Toggle menu"
		>
			<svg xmlns="http://www.w3.org/2000/svg" class="w-7 h-7" fill="none" viewBox="0 0 24 24" stroke="currentColor">
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d={mobileOpen ? 'M6 18L18 6M6 6l12 12' : 'M4 6h16M4 12h16M4 18h16'}
				/>
			</svg>
		</button>

		<div class="flex gap-3">
			{#each [Instagram, Twitter, Facebook] as icon}
				<div class="rounded-full bg-white p-2">
					<img src={icon} alt="social" class="w-4 h-4" />
				</div>
			{/each}
		</div>
	</div>

	<!-- ================= MOBILE SLIDE MENU ================= -->
	<div class="fixed inset-0 z-40 lg:hidden pointer-events-none">
		<!-- Backdrop -->
		<!-- svelte-ignore a11y_click_events_have_key_events -->
		<!-- svelte-ignore a11y_no_static_element_interactions -->
		<div
			on:click={() => (mobileOpen = false)}
			class="absolute inset-0 bg-black/30 transition-opacity duration-300"
			class:opacity-100={mobileOpen}
			class:opacity-0={!mobileOpen}
		></div>

		<!-- Slide Panel -->
		<div
			class="absolute top-0 right-0 h-full w-[80%] max-w-sm bg-[#F3E7D4] px-6 py-10
			       transform transition-transform duration-300 ease-out pointer-events-auto"
			class:translate-x-0={mobileOpen}
			class:translate-x-full={!mobileOpen}
		>
			<ul class="space-y-6 mt-10">
				{#each links as link}
					<li>
						<a
							href={link.href}
							on:click={() => (mobileOpen = false)}
							class="block text-[#5C4033] text-xl font-medium"
						>
							{link.name}
						</a>
					</li>
				{/each}
			</ul>

			<a
				href="#contact"
				on:click={() => (mobileOpen = false)}
				class="mt-10 block border-2 border-[#5C4033] text-[#5C4033]
				       text-center py-3 rounded-3xl hover:bg-[#5C4033]
				       hover:text-[#EFE5D5] transition"
			>
				Contact
			</a>
		</div>
	</div>
</nav>
