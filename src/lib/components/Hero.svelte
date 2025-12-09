<script lang="ts">
	// Using placeholders for the hero images
	const images = [
		"https://images.unsplash.com/photo-1534528741775-53994a69daeb?w=400&h=500&fit=crop",
		"https://images.unsplash.com/photo-1517841905240-472988babdf9?w=400&h=500&fit=crop",
		"https://images.unsplash.com/photo-1506794778202-cad84cf45f1d?w=400&h=500&fit=crop",
		"https://images.unsplash.com/photo-1531123897727-8f129e1688ce?w=400&h=500&fit=crop"
	];
</script>

<section class="flex flex-col items-center pt-20 pb-32 px-4 text-center max-w-7xl mx-auto">
	<h1 class="text-5xl md:text-6xl font-bold tracking-tight text-gray-900 max-w-4xl mb-6 leading-[1.1]">
		Recruiting system that helps you hire better talent faster.
	</h1>
	<p class="text-lg text-gray-600 max-w-2xl mb-10">
		Source and evaluate extraordinary talent, automatically.<br class="hidden md:block" />
		Cut weeks off your hiring process.
	</p>

	<button class="bg-black text-white px-6 py-3 rounded-full font-medium flex items-center gap-2 hover:bg-gray-800 transition-colors cursor-pointer">
		<span class="w-5 h-5 bg-white rounded-full flex items-center justify-center">
            <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="black" stroke-width="3" stroke-linecap="round" stroke-linejoin="round">
                <path d="M5 12h14M12 5l7 7-7 7"/>
            </svg>
        </span>
		Get early access
	</button>

	<!-- Hero Images -->
	<div class="mt-20 flex justify-center items-center relative w-full h-[300px] md:h-[400px]">
		{#each images as src, i}
			<div 
				class="absolute w-48 md:w-64 aspect-[3/4] rounded-2xl overflow-hidden shadow-xl border-4 border-white transition-transform duration-500 ease-out hover:z-10 hover:scale-105"
				style="
					transform: translateX({(i - 1.5) * 120}px) rotate({(i - 1.5) * 4}deg) translateY({Math.abs(i - 1.5) * 10}px);
					z-index: {i};
				"
			>
				<img {src} alt="Candidate" class="w-full h-full object-cover" />
			</div>
		{/each}
	</div>
</section>
