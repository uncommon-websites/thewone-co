<script lang="ts">
    export let category: string;
    export let title: string;
    export let description: string;
    export let buttonText: string;
    export let imageContent: any = null; // Could be a component or HTML
    
    // We will use a slot for the image content to allow flexibility
</script>

<section class="px-4 max-w-7xl mx-auto mb-32">
    <div class="mb-4 text-sm font-medium text-gray-500 uppercase tracking-wide">{category}</div>
    
    <div class="flex flex-col md:flex-row justify-between items-start gap-12 mb-16">
        <div class="max-w-2xl">
            <h2 class="text-4xl md:text-5xl font-bold mb-6 tracking-tight leading-[1.1]">{title}</h2>
            <p class="text-gray-600 text-lg leading-relaxed max-w-xl">
                {description}
            </p>
        </div>
        
        <button class="bg-black text-white pl-6 pr-2 py-2 rounded-full font-medium flex items-center gap-4 hover:bg-gray-800 transition-colors whitespace-nowrap">
            <div class="flex flex-col items-start text-left">
                <span class="text-sm font-bold">Learn about {category}</span>
                <span class="text-[10px] text-gray-400 opacity-80">{buttonText}</span>
            </div>
            <span class="w-8 h-8 bg-white/20 rounded-full flex items-center justify-center">
                <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                    <path d="M5 12h14M12 5l7 7-7 7"/>
                </svg>
            </span>
        </button>
    </div>

    <!-- Feature Visual Container -->
    <div class="w-full bg-[#F0F4F8] rounded-[24px] overflow-hidden shadow-sm border border-gray-100 p-8 md:p-12">
        <slot />
    </div>
</section>
