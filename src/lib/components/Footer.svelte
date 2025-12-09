<script lang="ts">
    import Logo from './Logo.svelte';
</script>

<footer class="bg-[#0A1A2F] text-white pt-32 pb-12 px-4 relative overflow-hidden">
    <!-- Starry background effect (simplified) -->
    <div class="absolute inset-0 opacity-30" style="background-image: radial-gradient(white 1px, transparent 1px); background-size: 50px 50px;"></div>
    
    <div class="max-w-7xl mx-auto relative z-10 flex flex-col items-center text-center">
        <h2 class="text-5xl md:text-6xl font-bold mb-4 tracking-tight">
            Hire better. Faster.<br/>Take your time back.
        </h2>
        <p class="text-blue-200/80 text-lg mb-10">
            Make hiring easier than ever.
        </p>
        
        <button class="bg-white text-black px-6 py-3 rounded-full font-medium flex items-center gap-2 hover:bg-gray-100 transition-colors mb-32">
            <span class="w-5 h-5 bg-black rounded-full flex items-center justify-center">
                <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="3" stroke-linecap="round" stroke-linejoin="round">
                    <path d="M5 12h14M12 5l7 7-7 7"/>
                </svg>
            </span>
            Get early access
        </button>

        <div class="w-full grid grid-cols-2 md:grid-cols-4 gap-8 text-left border-t border-white/10 pt-12">
            <div class="col-span-2 md:col-span-1">
                <div class="mb-6">
                    <Logo color="white" />
                </div>
                <p class="text-sm text-gray-400 mb-4">
                    Your own, personal recruiter.<br/>Completely automated.
                </p>
                <a href="#" class="text-sm font-bold hover:text-blue-300 transition-colors">Follow us on LinkedIn</a>
            </div>
            
            <div class="md:col-start-3">
                <h4 class="font-bold mb-4">Features</h4>
                <ul class="space-y-2 text-sm text-gray-400">
                    <li><a href="#" class="hover:text-white transition-colors">Overview</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Sourcing</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Evaluation</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Tracking</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Communication</a></li>
                </ul>
            </div>

            <div>
                <h4 class="font-bold mb-4">Product</h4>
                <ul class="space-y-2 text-sm text-gray-400">
                    <li><a href="#" class="hover:text-white transition-colors">Pricing</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Early access</a></li>
                </ul>
            </div>
        </div>
    </div>
</footer>
