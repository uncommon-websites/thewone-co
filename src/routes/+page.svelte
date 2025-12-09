<script lang="ts">
    import Navbar from '$lib/components/Navbar.svelte';
    import Hero from '$lib/components/Hero.svelte';
    import FeatureIntro from '$lib/components/FeatureIntro.svelte';
    import LargeFeatureBlock from '$lib/components/LargeFeatureBlock.svelte';
    import DetailedFeature from '$lib/components/DetailedFeature.svelte';
    import VisionSection from '$lib/components/VisionSection.svelte';
    import FounderLetter from '$lib/components/FounderLetter.svelte';
    import ComparisonChart from '$lib/components/ComparisonChart.svelte';
    import Footer from '$lib/components/Footer.svelte';
</script>

<div class="min-h-screen bg-[#F9F9F7] font-sans text-gray-900 selection:bg-black selection:text-white">
    <Navbar />
    
    <main>
        <Hero />
        <FeatureIntro />
        <LargeFeatureBlock />
        
        <!-- Sourcing Feature -->
        <DetailedFeature 
            category="Sourcing"
            title="Find exceptional talent others miss, magically."
            description="Wone actively finds candidates using natural language and contextual search, going beyond boolean filtering to find talent that matches your exact needs. Save weeks sourcing and get a curated list of candidates in front of you in as little as 20 seconds."
            buttonText="Save weeks sourcing talent"
        >
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden relative">
                <!-- Mockup of Sourcing UI -->
                <div class="border-b border-gray-100 p-4 flex items-center justify-between bg-white">
                    <div class="flex items-center gap-4">
                        <div class="w-8 h-8 rounded-full bg-blue-600 flex items-center justify-center text-white text-xs font-bold">W</div>
                        <div class="font-bold text-sm">Chief Technical Officer, Payments</div>
                        <div class="text-xs text-gray-400 flex items-center gap-1">
                            <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>
                            Boston, US
                        </div>
                        <div class="text-xs text-gray-400 flex items-center gap-1">
                            <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="7" width="20" height="14" rx="2" ry="2"></rect><path d="M16 21V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v16"></path></svg>
                            Contract
                        </div>
                        <div class="text-xs text-gray-400 flex items-center gap-1">
                            <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
                            $150,000 - $240,000
                        </div>
                    </div>
                    <div class="flex gap-2">
                         <div class="flex -space-x-2 mr-2">
                            <div class="w-6 h-6 rounded-full border-2 border-white bg-gray-200"></div>
                            <div class="w-6 h-6 rounded-full border-2 border-white bg-gray-300"></div>
                            <div class="w-6 h-6 rounded-full border-2 border-white bg-gray-400"></div>
                        </div>
                        <button class="text-xs border px-2 py-1 rounded">Preview</button>
                        <button class="text-xs bg-black text-white px-2 py-1 rounded">Edit</button>
                    </div>
                </div>
                
                <div class="p-6 bg-[#F8F9FB] min-h-[400px] flex gap-6">
                    <!-- Sidebar filters -->
                    <div class="w-64 space-y-6 hidden md:block">
                        <div>
                            <div class="text-xs font-bold uppercase text-gray-400 mb-2">Search</div>
                            <div class="bg-white p-2 rounded border border-gray-200 text-sm text-gray-500 flex justify-between items-center">
                                <span>Candidates</span>
                                <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>
                            </div>
                        </div>
                        <div>
                             <div class="text-xs font-bold uppercase text-gray-400 mb-2">Details</div>
                             <div class="space-y-2">
                                <div class="h-2 w-3/4 bg-gray-200 rounded"></div>
                                <div class="h-2 w-1/2 bg-gray-200 rounded"></div>
                                <div class="h-2 w-2/3 bg-gray-200 rounded"></div>
                             </div>
                        </div>
                    </div>

                    <!-- Main List -->
                    <div class="flex-1 space-y-4">
                        <div class="flex justify-between items-center">
                            <h4 class="font-bold text-sm">Excellent matches</h4>
                        </div>
                        
                        <!-- Card 1 -->
                        <div class="bg-white p-4 rounded-lg border border-gray-100 shadow-sm">
                            <div class="flex justify-between items-start mb-3">
                                <div class="flex gap-3">
                                    <div class="w-10 h-10 rounded-full bg-purple-100 overflow-hidden">
                                        <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?w=100&h=100&fit=crop" alt="" class="w-full h-full object-cover"/>
                                    </div>
                                    <div>
                                        <div class="font-bold text-sm">Lydia Nelson</div>
                                        <div class="text-xs text-gray-500">Software Engineer @ Plaid • Boston, USA</div>
                                    </div>
                                </div>
                                <div class="flex gap-2">
                                    <button class="text-xs border px-2 py-1 rounded flex items-center gap-1">
                                        <svg width="10" height="10" viewBox="0 0 24 24" fill="currentColor"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg>
                                        LinkedIn
                                    </button>
                                    <button class="text-xs bg-black text-white px-2 py-1 rounded">Invite to apply</button>
                                </div>
                            </div>
                            <div class="flex gap-2 mb-3">
                                <span class="text-[10px] font-bold text-blue-600 bg-blue-50 px-1.5 py-0.5 rounded flex items-center gap-1">
                                    <span class="w-1.5 h-1.5 rounded-full bg-blue-600"></span> Excellent match
                                </span>
                                <span class="text-[10px] font-bold text-green-600 bg-green-50 px-1.5 py-0.5 rounded flex items-center gap-1">
                                    <span class="w-1.5 h-1.5 rounded-full bg-green-600"></span> Highly likely to move
                                </span>
                            </div>
                            <div class="text-xs text-gray-600 space-y-1 mb-3">
                                <p>Lydia is a strong fit. Currently processing over $100M per year, led a team of 30 engineers, extensive experience with compliance, financial security and distributed systems.</p>
                                <p>Exceeds financial systems scaling requirements.</p>
                            </div>
                             <div class="text-xs text-gray-600">
                                <div class="font-bold flex items-center gap-1 mb-0.5">
                                    <span class="w-1.5 h-1.5 rounded-full bg-red-500"></span> Weaknesses
                                </div>
                                <p>Financial compliance experience not highlighted, but probably has it considering extensive experience with large systems.</p>
                            </div>
                        </div>

                        <!-- Card 2 -->
                        <div class="bg-white p-4 rounded-lg border border-gray-100 shadow-sm opacity-60">
                            <div class="flex justify-between items-start mb-3">
                                <div class="flex gap-3">
                                    <div class="w-10 h-10 rounded-full bg-orange-100 overflow-hidden">
                                         <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?w=100&h=100&fit=crop" alt="" class="w-full h-full object-cover"/>
                                    </div>
                                    <div>
                                        <div class="font-bold text-sm">Peter Samson</div>
                                        <div class="text-xs text-gray-500">Senior Engineer @ Stripe • New York, USA</div>
                                    </div>
                                </div>
                                <div class="flex gap-2">
                                     <button class="text-xs border px-2 py-1 rounded flex items-center gap-1">LinkedIn</button>
                                     <button class="text-xs border px-2 py-1 rounded">Invite to apply</button>
                                </div>
                            </div>
                             <div class="flex gap-2 mb-3">
                                <span class="text-[10px] font-bold text-blue-600 bg-blue-50 px-1.5 py-0.5 rounded flex items-center gap-1">
                                    <span class="w-1.5 h-1.5 rounded-full bg-blue-600"></span> Excellent match
                                </span>
                                <span class="text-[10px] font-bold text-green-600 bg-green-50 px-1.5 py-0.5 rounded flex items-center gap-1">
                                    <span class="w-1.5 h-1.5 rounded-full bg-green-600"></span> Highly likely to move
                                </span>
                            </div>
                            <div class="text-xs text-gray-600 space-y-1">
                                <p>We think Peter is likely to move since he has been at Meta for almost 2 years, following the recent team restructuring in their AR division. Peter has specialized backend infrastructure experience that hasn't been fully utilized in his current role.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </DetailedFeature>

        <!-- Evaluation Feature -->
        <DetailedFeature 
            category="Evaluation"
            title="Evaluate and qualify talent with precision, instantly."
            description="Wone's deep evaluation goes beyond resume basics to spot true role fit, even when it isn't obvious on a profile. It explains exactly why each candidate is a fit, along with any potential weaknesses. Optionally, Wone runs an automated AI video interview to qualify candidates and deliver structured assessments, so your team doesn't have to."
            buttonText="Evaluate talent in minutes"
        >
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden p-6 md:p-12 relative">
                <!-- Background decorative elements -->
                <div class="absolute top-0 right-0 w-1/3 h-full bg-gradient-to-l from-orange-50/50 to-transparent pointer-events-none"></div>
                <div class="absolute bottom-0 left-0 w-1/3 h-1/2 bg-gradient-to-t from-blue-50/50 to-transparent pointer-events-none"></div>

                <!-- Mockup of Evaluation Card -->
                <div class="flex flex-col md:flex-row gap-8 relative z-10">
                    <div class="w-24 h-24 rounded-2xl overflow-hidden shrink-0 shadow-lg">
                        <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?w=200&h=200&fit=crop" class="w-full h-full object-cover" alt="Profile"/>
                    </div>
                    <div class="flex-1">
                        <div class="flex flex-col md:flex-row justify-between items-start mb-4 gap-4">
                            <div>
                                <h3 class="font-bold text-2xl">Alexis Bauers</h3>
                                <div class="flex items-center gap-2 text-gray-500 text-sm mt-1">
                                    <span>Chief Technical Officer @ Plaid</span>
                                    <span>•</span>
                                    <span class="flex items-center gap-1"><svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg> Boston, USA</span>
                                </div>
                            </div>
                            <div class="flex gap-3">
                                <button class="px-4 py-2 border border-gray-200 rounded-lg text-sm font-medium flex items-center gap-2 hover:bg-gray-50">
                                    <svg width="14" height="14" viewBox="0 0 24 24" fill="currentColor"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg>
                                    LinkedIn
                                </button>
                                <button class="px-4 py-2 bg-white border border-gray-200 text-black rounded-lg text-sm font-medium hover:bg-gray-50">Invite to apply</button>
                            </div>
                        </div>
                        
                        <div class="flex gap-3 mb-6">
                            <span class="text-xs font-bold text-blue-600 bg-blue-50 px-2.5 py-1 rounded-md flex items-center gap-1.5">
                                <svg width="10" height="10" viewBox="0 0 24 24" fill="currentColor"><path d="M13 2L3 14h9l-1 8 10-12h-9l1-8z"/></svg> Excellent match
                            </span>
                            <span class="text-xs font-bold text-green-600 bg-green-50 px-2.5 py-1 rounded-md flex items-center gap-1.5">
                                <span class="w-2 h-2 rounded-full bg-green-600"></span> Highly likely to move
                            </span>
                        </div>
                        
                        <div class="space-y-4 text-base text-gray-700 leading-relaxed">
                            <p>Alexis brings the ability to design and scale secure systems that keep financial transactions stable under heavy load. Her experience building APIs at Plaid and real-time payment systems at Codebank shows she can strengthen infrastructure while reducing integration complexity.</p>
                            <p>Just as importantly, her track record improving release cycles, onboarding, and code quality highlights her capacity to elevate entire engineering teams, not just deliver features.</p>
                            
                            <div class="mt-6 pt-4 border-t border-gray-100">
                                <div class="font-bold flex items-center gap-2 mb-2 text-sm">
                                    <span class="w-2 h-2 rounded-full bg-black"></span> Weaknesses
                                </div>
                                <p class="text-sm text-gray-600">Experience mostly in consumer tech, may need to adapt to stricter regulations in enterprise systems.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </DetailedFeature>

        <!-- Tracking Feature -->
        <DetailedFeature 
            category="Tracking"
            title="Easily track and manage candidates through the process."
            description="Source and invite candidates to apply, then review all the candidates who did and easily move them through the stages. Set your own hiring workflow, number of steps and types of stages you want the candidates to go through. All with a simple and easy interface you don't have to learn."
            buttonText="Simple applicant tracking system"
        >
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden flex flex-col h-[500px]">
                 <!-- Mockup of Kanban/Tracking UI -->
                 <div class="border-b border-gray-100 p-6 flex justify-between items-center">
                    <div>
                        <div class="flex items-center gap-3 mb-1">
                            <div class="w-8 h-8 rounded-full bg-blue-600 flex items-center justify-center text-white text-xs font-bold">W</div>
                            <h3 class="font-bold text-lg">Chief Technical Officer, Payments</h3>
                        </div>
                        <div class="flex gap-4 text-xs text-gray-500 pl-11">
                            <span class="flex items-center gap-1"><svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg> Boston, US</span>
                            <span class="flex items-center gap-1"><svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="7" width="20" height="14" rx="2" ry="2"></rect><path d="M16 21V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v16"></path></svg> Contract</span>
                            <span class="flex items-center gap-1"><svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg> $150,000 - $240,000</span>
                        </div>
                    </div>
                    <div class="flex gap-2">
                        <button class="text-xs border px-3 py-1.5 rounded font-medium">Preview</button>
                        <button class="text-xs bg-black text-white px-3 py-1.5 rounded font-medium">Edit</button>
                    </div>
                 </div>
                 
                 <div class="flex-1 bg-[#F8F9FB] p-6 flex gap-6 overflow-hidden">
                    <!-- Column 1: Sourced -->
                    <div class="w-1/4 flex flex-col gap-3 min-w-[250px]">
                        <div class="font-bold text-sm text-gray-500 flex justify-between items-center mb-2">
                            <span>Sourced</span>
                            <span class="bg-gray-200 px-2 py-0.5 rounded-full text-[10px] font-bold text-gray-600">6</span>
                        </div>
                        
                        <!-- Card -->
                        <div class="bg-white p-4 rounded-lg border border-gray-200 shadow-sm hover:shadow-md transition-shadow cursor-pointer">
                            <div class="flex items-center gap-3 mb-3">
                                <div class="w-8 h-8 rounded-full bg-orange-100 overflow-hidden">
                                    <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?w=100&h=100&fit=crop" alt="" class="w-full h-full object-cover"/>
                                </div>
                                <div>
                                    <div class="text-sm font-bold">Peter Samson</div>
                                    <div class="text-[10px] text-gray-500">Chief Technical Officer @ Meta</div>
                                </div>
                            </div>
                            <div class="flex gap-2 mb-2">
                                <span class="text-[10px] font-bold text-blue-600 bg-blue-50 px-1.5 py-0.5 rounded">Excellent match</span>
                            </div>
                            <div class="text-[10px] text-gray-500 line-clamp-2">
                                Peter has specialized backend infrastructure experience that hasn't been fully utilized...
                            </div>
                        </div>

                         <!-- Card -->
                        <div class="bg-white p-4 rounded-lg border border-gray-200 shadow-sm hover:shadow-md transition-shadow cursor-pointer">
                            <div class="flex items-center gap-3 mb-3">
                                <div class="w-8 h-8 rounded-full bg-blue-100 overflow-hidden">
                                     <img src="https://images.unsplash.com/photo-1573497019940-1c28c88b4f3e?w=100&h=100&fit=crop" alt="" class="w-full h-full object-cover"/>
                                </div>
                                <div>
                                    <div class="text-sm font-bold">Diana Lee</div>
                                    <div class="text-[10px] text-gray-500">Chief Technical Officer @ Amazon</div>
                                </div>
                            </div>
                            <div class="flex gap-2 mb-2">
                                <span class="text-[10px] font-bold text-blue-600 bg-blue-50 px-1.5 py-0.5 rounded">Excellent match</span>
                                <span class="text-[10px] font-bold text-green-600 bg-green-50 px-1.5 py-0.5 rounded">Somewhat likely</span>
                            </div>
                            <div class="text-[10px] text-gray-500 line-clamp-2">
                                Led complex, cross-org launches with high operational rigor. Deep systems background...
                            </div>
                        </div>
                    </div>
                    
                    <!-- Column 2: Invited -->
                    <div class="w-1/4 flex flex-col gap-3 min-w-[250px]">
                        <div class="font-bold text-sm text-gray-500 flex justify-between items-center mb-2">
                            <span>Invited</span>
                            <span class="bg-gray-200 px-2 py-0.5 rounded-full text-[10px] font-bold text-gray-600">3</span>
                        </div>
                        
                         <!-- Card -->
                        <div class="bg-white p-4 rounded-lg border border-gray-200 shadow-sm hover:shadow-md transition-shadow cursor-pointer">
                            <div class="flex items-center gap-3 mb-3">
                                <div class="w-8 h-8 rounded-full bg-purple-100 overflow-hidden">
                                    <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=100&h=100&fit=crop" alt="" class="w-full h-full object-cover"/>
                                </div>
                                <div>
                                    <div class="text-sm font-bold">James Rodriguez</div>
                                    <div class="text-[10px] text-gray-500">Software Engineer @ Google</div>
                                </div>
                            </div>
                            <div class="flex gap-2 mb-2">
                                <span class="text-[10px] font-bold text-blue-600 bg-blue-50 px-1.5 py-0.5 rounded">Strong match</span>
                            </div>
                            <div class="text-[10px] text-gray-500 line-clamp-2">
                                Created financial systems at Robinhood, distributed architecture and ML pipelines...
                            </div>
                             <div class="mt-2 text-[10px] text-red-500 font-medium flex items-center gap-1">
                                <span class="w-1 h-1 rounded-full bg-red-500"></span> Gap: Led teams of 12 engineers - compared to 15 required.
                            </div>
                        </div>

                         <!-- Card -->
                        <div class="bg-white p-4 rounded-lg border border-gray-200 shadow-sm hover:shadow-md transition-shadow cursor-pointer">
                            <div class="flex items-center gap-3 mb-3">
                                <div class="w-8 h-8 rounded-full bg-green-100 overflow-hidden">
                                    <img src="https://images.unsplash.com/photo-1580489944761-15a19d654956?w=100&h=100&fit=crop" alt="" class="w-full h-full object-cover"/>
                                </div>
                                <div>
                                    <div class="text-sm font-bold">Maria Patterson</div>
                                    <div class="text-[10px] text-gray-500">Software Engineer @ Cashapp</div>
                                </div>
                            </div>
                             <div class="flex gap-2 mb-2">
                                <span class="text-[10px] font-bold text-blue-600 bg-blue-50 px-1.5 py-0.5 rounded">Strong match</span>
                            </div>
                            <div class="text-[10px] text-gray-500 line-clamp-2">
                                Built an AI infrastructure with $50M daily volume, developed extensive ML models...
                            </div>
                        </div>
                    </div>

                     <!-- Column 3: Interview -->
                    <div class="w-1/4 flex flex-col gap-3 min-w-[250px] opacity-100">
                        <div class="font-bold text-sm text-gray-500 flex justify-between items-center mb-2">
                            <span>Interview</span>
                            <span class="bg-gray-200 px-2 py-0.5 rounded-full text-[10px] font-bold text-gray-600">1</span>
                        </div>
                         <!-- Card -->
                        <div class="bg-white p-4 rounded-lg border border-gray-200 shadow-sm hover:shadow-md transition-shadow cursor-pointer border-l-4 border-l-blue-500">
                            <div class="flex items-center gap-3 mb-3">
                                <div class="w-8 h-8 rounded-full bg-pink-100 overflow-hidden">
                                     <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?w=100&h=100&fit=crop" alt="" class="w-full h-full object-cover"/>
                                </div>
                                <div>
                                    <div class="text-sm font-bold">Lydia Nelson</div>
                                    <div class="text-[10px] text-gray-500">Software Engineer @ Plaid</div>
                                </div>
                            </div>
                            <div class="flex gap-2 mb-2">
                                <span class="text-[10px] font-bold text-blue-600 bg-blue-50 px-1.5 py-0.5 rounded">Excellent match</span>
                            </div>
                            <div class="text-[10px] text-gray-500 line-clamp-2">
                                Lydia is a strong fit. Currently processing over $100M per year, led a team...
                            </div>
                             <div class="mt-2 text-[10px] text-blue-600 font-bold bg-blue-50 inline-block px-1.5 py-0.5 rounded">
                                Scheduled: Fri 27 Jan 2:00 PM
                            </div>
                        </div>
                    </div>

                    <!-- Column 4: Offer -->
                    <div class="w-1/4 flex flex-col gap-3 min-w-[250px] opacity-40">
                         <div class="font-bold text-sm text-gray-500 flex justify-between items-center mb-2">
                            <span>Offer</span>
                            <span class="bg-gray-200 px-2 py-0.5 rounded-full text-[10px] font-bold text-gray-600">0</span>
                        </div>
                        <div class="h-full border-2 border-dashed border-gray-200 rounded-lg flex items-center justify-center">
                            <span class="text-gray-400 text-xs">Drop candidates here</span>
                        </div>
                    </div>
                 </div>
            </div>
        </DetailedFeature>

        <!-- Communication Feature -->
        <DetailedFeature 
            category="Communication"
            title="Personalized outreach, communication and feedback on autopilot."
            description="Wone learns your writing style and automates the entire communication cycle. Automate interview scheduling, replies to candidate questions, status updates, and follow up, all in your authentic voice, without your constant attention."
            buttonText="Automate outreach and feedback"
        >
             <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden h-[500px] flex">
                <!-- Sidebar -->
                <div class="w-64 border-r border-gray-100 flex flex-col hidden md:flex">
                    <div class="p-4 border-b border-gray-100">
                        <div class="flex items-center gap-2 mb-4">
                            <div class="w-6 h-6 rounded bg-black text-white flex items-center justify-center text-xs font-bold">W</div>
                            <span class="font-bold text-sm">Cockbank Careers</span>
                        </div>
                        <h2 class="font-bold text-2xl mb-1">Inbox</h2>
                        <p class="text-xs text-gray-500">Manage relationships with your candidate, clients and team.</p>
                    </div>
                    
                    <div class="p-2 space-y-1">
                        <button class="w-full text-left px-3 py-2 rounded bg-gray-100 font-medium text-sm flex justify-between items-center">
                            <div class="flex items-center gap-2">
                                <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
                                New message
                            </div>
                        </button>
                         <button class="w-full text-left px-3 py-2 rounded hover:bg-gray-50 font-medium text-sm text-gray-600 flex justify-between items-center">
                            <div class="flex items-center gap-2">
                                <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2" ry="2"></rect><line x1="16" y1="2" x2="16" y2="6"></line><line x1="8" y1="2" x2="8" y2="6"></line><line x1="3" y1="10" x2="21" y2="10"></line></svg>
                                All messages
                            </div>
                        </button>
                    </div>

                    <div class="flex-1 overflow-y-auto">
                        <div class="px-4 py-2 text-xs font-bold text-gray-400 uppercase">June</div>
                        
                        <!-- Message Item Active -->
                        <div class="px-4 py-3 bg-blue-50/50 border-l-2 border-blue-500 cursor-pointer">
                            <div class="flex justify-between items-start mb-1">
                                <span class="font-bold text-sm">John, Lucy, Me</span>
                                <span class="text-[10px] text-gray-400">Fri 27 Jan</span>
                            </div>
                            <div class="text-xs font-medium text-gray-800 mb-1">Feedback for Mateo Ruiz - Support Engineer</div>
                            <div class="text-[10px] text-gray-500 line-clamp-1">Hey team, just wrapped up Mateo's final round. Solid problem-solving and good customer empathy...</div>
                            <div class="flex items-center gap-1 mt-2">
                                <div class="w-4 h-4 rounded-full bg-gray-300"></div>
                                <div class="w-4 h-4 rounded-full bg-gray-400"></div>
                                <div class="w-4 h-4 rounded-full bg-gray-500"></div>
                            </div>
                        </div>

                         <!-- Message Item -->
                        <div class="px-4 py-3 hover:bg-gray-50 cursor-pointer">
                            <div class="flex justify-between items-start mb-1">
                                <span class="font-bold text-sm">Mateo, Me</span>
                                <span class="text-[10px] text-gray-400">Fri 27 Jan</span>
                            </div>
                            <div class="text-xs font-medium text-gray-800 mb-1">Mateo Ruiz - Scheduling next steps</div>
                            <div class="text-[10px] text-gray-500 line-clamp-1">Hi Mateo, thanks for chatting with us! We'd love to move forward. Should I schedule with the HM for a quick ch...</div>
                        </div>
                    </div>
                </div>

                <!-- Main Content -->
                <div class="flex-1 flex flex-col bg-white">
                    <div class="border-b border-gray-100 p-4 flex justify-between items-center">
                        <div>
                            <div class="font-bold text-sm">Mateo Ruiz - Scheduling next steps</div>
                            <div class="text-xs text-gray-500">Mateo, Me</div>
                        </div>
                        <div class="flex gap-2">
                             <button class="p-1.5 hover:bg-gray-100 rounded text-gray-400"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="1"></circle><circle cx="19" cy="12" r="1"></circle><circle cx="5" cy="12" r="1"></circle></svg></button>
                        </div>
                    </div>
                    
                    <div class="flex-1 p-6 space-y-6 overflow-y-auto bg-white">
                        <!-- Message 1 -->
                        <div class="flex gap-4">
                            <div class="w-8 h-8 rounded-full bg-gray-200 shrink-0 overflow-hidden">
                                <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?w=100&h=100&fit=crop" alt="" class="w-full h-full object-cover"/>
                            </div>
                            <div class="space-y-1 max-w-[80%]">
                                <div class="flex items-baseline gap-2">
                                    <span class="font-bold text-sm">Mateo Ruiz</span>
                                    <span class="text-[10px] text-gray-400">Fri 27 Jan, 10:30 AM</span>
                                </div>
                                <div class="text-sm text-gray-700 bg-gray-50 p-3 rounded-r-xl rounded-bl-xl">
                                    Wow, I am so happy to hear that. I can jump on a call today, if that works.
                                </div>
                            </div>
                        </div>

                         <!-- Message 2 (Auto) -->
                        <div class="flex gap-4 flex-row-reverse">
                            <div class="w-8 h-8 rounded-full bg-black shrink-0 flex items-center justify-center text-white text-[10px] font-bold">W</div>
                            <div class="space-y-1 max-w-[80%]">
                                <div class="flex items-baseline gap-2 justify-end">
                                    <span class="font-bold text-sm">Wone (Auto-reply)</span>
                                    <span class="text-[10px] text-gray-400">Fri 27 Jan, 10:31 AM</span>
                                </div>
                                <div class="text-sm text-gray-700 bg-blue-50 border border-blue-100 p-3 rounded-l-xl rounded-br-xl">
                                    Hi Mateo, great! I've sent a calendar invite for 2 PM today. Looking forward to it.
                                </div>
                                <div class="flex justify-end items-center gap-1 text-[10px] text-gray-400">
                                    <svg width="10" height="10" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M13 2L3 14h9l-1 8 10-12h-9l1-8z"/></svg>
                                    Sent automatically by Wone
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Reply Box -->
                    <div class="p-4 border-t border-gray-100">
                        <div class="bg-gray-50 rounded-lg p-2 border border-gray-200">
                            <div class="text-gray-400 text-sm mb-8">Write a reply...</div>
                            <div class="flex justify-between items-center">
                                <div class="flex gap-2 text-gray-400">
                                    <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21.44 11.05l-9.19 9.19a6 6 0 0 1-8.49-8.49l9.19-9.19a4 4 0 0 1 5.66 5.66l-9.2 9.19a2 2 0 0 1-2.83-2.83l8.49-8.48"></path></svg>
                                    <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><circle cx="8.5" cy="8.5" r="1.5"></circle><polyline points="21 15 16 10 5 21"></polyline></svg>
                                </div>
                                <button class="bg-black text-white px-3 py-1.5 rounded text-xs font-bold">Send</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </DetailedFeature>

        <VisionSection />
        <FounderLetter />
        <ComparisonChart />
    </main>

    <Footer />
</div>


