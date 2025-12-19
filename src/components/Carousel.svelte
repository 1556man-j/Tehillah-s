<script>
  let currentIndex = 0;

  const testimonials = [
    {
      id: 1,
      name: "Adaeze U.",
      role: "CEO, TechCorp",
      content: "This product has transformed the way we work. The team's dedication to excellence is evident in every feature.",
      image: "https://i.pravatar.cc/150?img=1"
    },
    {
      id: 2,
      name: "Tunde A.",
      role: "Designer, Creative Studio",
      content: "Outstanding quality and attention to detail. I couldn't be happier with the results we've achieved.",
      image: "https://i.pravatar.cc/150?img=2"
    },
    {
      id: 3,
      name: "Rachael O.",
      role: "Founder, StartupXYZ",
      content: "The best decision we made this year. Highly recommended for anyone looking to scale their business.",
      image: "https://i.pravatar.cc/150?img=3"
    },
    {
      id: 4,
      name: "James Wilson",
      role: "Marketing Director",
      content: "Exceptional service and support. The impact on our ROI has been remarkable and consistent.",
      image: "https://i.pravatar.cc/150?img=4"
    },
    {
      id: 5,
      name: "Lisa Anderson",
      role: "Product Manager",
      content: "Intuitive, powerful, and reliable. Everything we needed and more. A game-changer for our team.",
      image: "https://i.pravatar.cc/150?img=5"
    }
  ];

  function nextSlide() {
    currentIndex = (currentIndex + 1) % testimonials.length;
  }

  function prevSlide() {
    currentIndex = (currentIndex - 1 + testimonials.length) % testimonials.length;
  }
</script>

<div class="w-full max-w-7xl mx-auto px-4 py-12">
  <!-- Navigation Arrows -->
  <div class="flex justify-end items-center gap-4 mb-8">
    <button
      on:click={prevSlide}
      class="p-3 border-2 border-[#5C4033] hover:bg-[#5C4033] hover:text-white transition-colors rounded-full"
      aria-label="Previous testimonial"
    >
      <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
        <path d="m15 18-6-6 6-6"/>
      </svg>
    </button>
    <button
      on:click={nextSlide}
      class="p-3 border-2 border-[#5C4033] hover:bg-[#5C4033] hover:text-white transition-colors rounded-full"
      aria-label="Next testimonial"
    >
      <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
        <path d="m9 18 6-6-6-6"/>
      </svg>
    </button>
  </div>

  <!-- Testimonials Container -->
  <div class="relative overflow-hidden">
    <!-- Mobile View - Single testimonial with side borders visible -->
    <div class="md:hidden">
      <div class="flex items-center justify-center gap-2">
        <!-- Left border indicator -->
        <div class="w-4 flex-shrink-0 h-64 border-l-2 border-[#5C4033]" />

        <!-- Active testimonial -->
        <div class="flex-1 p-8 border-2 rounded-lg transition-all duration-300 bg-[#5C4033] text-white border-[#5C4033]">
          <div class="flex flex-col items-center text-center">
            <img
              src={testimonials[currentIndex].image}
              alt={testimonials[currentIndex].name}
              class="w-16 h-16 rounded-full mb-4 object-cover"
            />
            <p class="text-lg mb-6 italic text-white">
              "{testimonials[currentIndex].content}"
            </p>
            <h3 class="font-bold text-xl text-white">
              {testimonials[currentIndex].name}
            </h3>
            <p class="text-sm text-gray-200">
              {testimonials[currentIndex].role}
            </p>
          </div>
        </div>

        <!-- Right border indicator -->
        <div class="w-4 flex-shrink-0 h-64 border-r-2 border-[#5C4033]" />
      </div>
    </div>

    <!-- Desktop View (md) - Two testimonials with left side partially visible -->
    <div class="hidden md:block lg:hidden">
      <div class="flex items-center justify-start gap-6 overflow-hidden">
        <!-- Left partial testimonial -->
        <div
          class="w-24 flex-shrink-0 p-8 border-2 border-[#5C4033] rounded-lg opacity-50 transition-all duration-500 overflow-hidden"
          style="clip-path: inset(0 0 0 75%)"
        >
          <div class="flex flex-col items-center text-center whitespace-nowrap">
            <img
              src={testimonials[(currentIndex - 1 + testimonials.length) % testimonials.length].image}
              alt={testimonials[(currentIndex - 1 + testimonials.length) % testimonials.length].name}
              class="w-20 h-20 rounded-full mb-4 object-cover"
            />
          </div>
        </div>

        <!-- Active center testimonial -->
        <div class="flex-1 p-8 border-2 rounded-lg transition-all duration-500 bg-[#5C4033] text-white border-[#5C4033]">
          <div class="flex flex-col items-center text-center">
            <img
              src={testimonials[currentIndex].image}
              alt={testimonials[currentIndex].name}
              class="w-20 h-20 rounded-full mb-4 object-cover"
            />
            <p class="text-lg mb-6 italic text-white">
              "{testimonials[currentIndex].content}"
            </p>
            <h3 class="font-bold text-xl text-white">
              {testimonials[currentIndex].name}
            </h3>
            <p class="text-sm text-gray-200">
              {testimonials[currentIndex].role}
            </p>
          </div>
        </div>
      </div>
    </div>

    <!-- Large Desktop View (lg+) - Three testimonials -->
    <div class="hidden lg:block">
      <div class="flex items-center justify-center gap-6 overflow-hidden">
        <!-- Left testimonial (clipped) -->
        <div
          class="w-full p-8 border-2 rounded-lg transition-all duration-500 border-[#5C4033] opacity-60 scale-95 -mr-4"
          style="clip-path: inset(0 1% 0 0)"
        >
          <div class="flex flex-col items-center text-center">
            <img
              src={testimonials[(currentIndex - 1 + testimonials.length) % testimonials.length].image}
              alt={testimonials[(currentIndex - 1 + testimonials.length) % testimonials.length].name}
              class="w-20 h-20 rounded-full mb-4 object-cover"
            />
            <p class="text-lg mb-6 italic text-gray-700">
              "{testimonials[(currentIndex - 1 + testimonials.length) % testimonials.length].content}"
            </p>
            <h3 class="font-bold text-xl text-gray-900">
              {testimonials[(currentIndex - 1 + testimonials.length) % testimonials.length].name}
            </h3>
            <p class="text-sm text-gray-600">
              {testimonials[(currentIndex - 1 + testimonials.length) % testimonials.length].role}
            </p>
          </div>
        </div>

        <!-- Center testimonial (active) -->
        <div class="w-full p-8 border-2 rounded-lg transition-all duration-500 bg-[#5C4033] text-white border-[#5C4033] scale-105">
          <div class="flex flex-col items-center text-center">
            <img
              src={testimonials[currentIndex].image}
              alt={testimonials[currentIndex].name}
              class="w-20 h-20 rounded-full mb-4 object-cover"
            />
            <p class="text-lg mb-6 italic text-white">
              "{testimonials[currentIndex].content}"
            </p>
            <h3 class="font-bold text-xl text-white">
              {testimonials[currentIndex].name}
            </h3>
            <p class="text-sm text-gray-200">
              {testimonials[currentIndex].role}
            </p>
          </div>
        </div>

        <!-- Right testimonial (clipped) -->
        <div
          class="w-full p-8 border-2 rounded-lg transition-all duration-500 border-[#5C4033] opacity-60 scale-95 -ml-4"
          style="clip-path: inset(0 0 0 1%)"
        >
          <div class="flex flex-col items-center text-center">
            <img
              src={testimonials[(currentIndex + 1) % testimonials.length].image}
              alt={testimonials[(currentIndex + 1) % testimonials.length].name}
              class="w-20 h-20 rounded-full mb-4 object-cover"
            />
            <p class="text-lg mb-6 italic text-gray-700">
              "{testimonials[(currentIndex + 1) % testimonials.length].content}"
            </p>
            <h3 class="font-bold text-xl text-gray-900">
              {testimonials[(currentIndex + 1) % testimonials.length].name}
            </h3>
            <p class="text-sm text-gray-600">
              {testimonials[(currentIndex + 1) % testimonials.length].role}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Pagination Dots -->
  <div class="flex justify-center gap-2 mt-8">
    {#each testimonials as _, idx}
      <button
        on:click={() => currentIndex = idx}
        class="w-2 h-2 rounded-full transition-all {idx === currentIndex ? 'bg-[#5C4033] w-8' : 'bg-gray-300'}"
        aria-label="Go to testimonial {idx + 1}"
      />
    {/each}
  </div>
</div>