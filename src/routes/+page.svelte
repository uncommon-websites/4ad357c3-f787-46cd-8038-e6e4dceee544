<script lang="ts">
  import Logo from '$lib/components/Logo.svelte';

  // SVGs
  const arrowUpIcon = `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-white"><path d="m5 12 7-7 7 7"/><path d="M12 19V5"/></svg>`;
  const playIcon = `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><polygon points="5 3 19 12 5 21 5 3"/></svg>`;
  const sparkleIcon = `<svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-gray-800"><path d="M12 2L14.4 9.6L22 12L14.4 14.4L12 22L9.6 14.4L2 12L9.6 9.6L12 2Z" fill="#333"/><path d="M19 17L20 20L23 21L20 22L19 25L18 22L15 21L18 20L19 17Z" fill="#333"/><path d="M5 5L6 8L9 9L6 10L5 13L4 10L1 9L4 8L5 5Z" fill="#333"/></svg>`;
</script>

<style>
  .custom-gradient-bg {
    background: linear-gradient(to bottom, #abcfe9 0%, #eef6fb 50%, #f5f7f9 100%);
  }
</style>

<div class="w-full bg-white font-sans">
  <!-- Hero Section -->
  <section class="pt-16 md:pt-24 pb-12">
    <div class="max-w-4xl mx-auto px-4 text-center mb-16">
      <h1 class="text-[42px] md:text-[64px] leading-[1.1] font-normal text-[#1a1a1a] tracking-tight mb-6 pt-8">
        Institutional intelligence.<br />
        Native to private markets.
      </h1>
      <p style="color: #334155" class="text-[19px] md:text-[21px] leading-relaxed max-w-2xl mx-auto font-light">
        Horison unifies documents, data, and firm knowledge into a single<br class="hidden md:block" />
        real-time workspace for investment teams.
      </p>
    </div>

    <!-- Hero Visual / Gradient Area -->
    <div class="mx-4 md:mx-6 lg:mx-8 rounded-t-[40px] md:rounded-t-[60px] custom-gradient-bg h-[600px] md:h-[700px] relative overflow-hidden pt-20">
      
      <!-- Cards Container -->
      <div class="flex flex-col items-center gap-5 px-4">
          
          <!-- Card 1: AI Agent Chat -->
          <div class="bg-white rounded-[32px] p-8 md:p-10 shadow-[0_4px_20px_rgba(0,0,0,0.03)] w-full max-w-[580px] relative z-20">
              <div class="flex items-center gap-2 mb-4">
                  {@html sparkleIcon}
                  <span class="text-gray-500 text-lg font-normal">Investment Intelligence</span>
              </div>
              <div class="text-[28px] md:text-[32px] leading-tight text-[#1a1a1a] font-normal">
                  I've analyzed the CIM. Revenue quality is high with 85% recurring fees and strong retention. <span class="inline-block align-bottom">📊</span>
              </div>
          </div>

          <!-- Card 2: Room Preview -->
          <div class="bg-white rounded-[32px] p-3 pr-8 shadow-[0_4px_20px_rgba(0,0,0,0.03)] w-full max-w-[580px] flex items-center gap-6 relative z-10">
              <!-- Image Placeholder -->
              <div class="w-[140px] h-[160px] shrink-0 rounded-[24px] overflow-hidden relative bg-gray-200">
                  <img src="/generated/image-a-high-end-modern-investment-firm-office-1771438794528-0.webp" alt="Data Room Analysis" class="w-full h-full object-cover opacity-80 mix-blend-multiply">
                  <div class="absolute inset-0 bg-gradient-to-r from-gray-300/50 to-transparent"></div>
              </div>
              
              <!-- Content -->
              <div class="flex flex-col justify-center h-full py-2">
                  <div class="text-[28px] text-[#1a1a1a] font-normal mb-1">
                      Due Diligence <span style="color: #334155" class="opacity-60">Report</span>
                  </div>
                  <!-- Small dot indicator -->
                  <div style="background-color: #1e40af" class="w-1.5 h-1.5 rounded-full mt-2"></div>
              </div>
          </div>

      </div>

      <!-- Fade at bottom to blend -->
      <div class="absolute bottom-0 left-0 w-full h-20 bg-gradient-to-t from-white to-transparent pointer-events-none"></div>
    </div>
  </section>

  <!-- Logos Section -->
  <section class="py-20 border-b border-gray-50">
    <div class="max-w-[1200px] mx-auto px-6">
      <p class="text-center text-sm font-medium text-gray-400 mb-12 uppercase tracking-widest">Trusted by leading private market investors</p>
      <div class="grid grid-cols-2 md:grid-cols-4 gap-y-12 gap-x-8 items-center justify-items-center opacity-40 grayscale hover:grayscale-0 transition-all duration-500">
        <div class="h-8 flex items-center"><span class="font-bold text-xl tracking-tight">Blackstone</span></div>
        <div class="h-8 flex items-center"><span class="font-serif text-2xl">KKR</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Carlyle</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl tracking-tighter">Apollo</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl italic">TPG</span></div>
        <div class="h-8 flex items-center"><span class="font-medium text-xl uppercase tracking-tighter">Warburg Pincus</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">BainCapital</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl tracking-widest">SEQUOIA</span></div>
      </div>
    </div>
  </section>

  <!-- Feature Section 1 -->
  <section class="py-24 px-6">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex flex-col md:flex-row gap-16 items-start">
        <!-- Visual -->
        <div class="w-full md:w-1/2 bg-gray-50 rounded-[32px] aspect-square relative overflow-hidden group">
          <img src="/generated/image-a-high-end-modern-investment-firm-office-1771438794528-0.webp" alt="Investment Intelligence" class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" />
          <div class="absolute inset-0 bg-black/5"></div>
        </div>

        <!-- Content -->
        <div class="w-full md:w-1/2 pt-8">
          <div class="flex justify-between items-start mb-6">
            <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-gray-900 max-w-md">
              Unify your firm's knowledge
            </h2>
            <span class="bg-[#1e40af] text-white px-3 py-1.5 rounded-full text-xs font-medium">Intelligence</span>
          </div>
          
          <p class="text-gray-600 text-lg mb-12 leading-relaxed">
            Break down silos between documents, data, and institutional memory. Horison creates a single source of truth for your entire investment team.
          </p>

          <div class="space-y-10">
            <!-- Feature 1 -->
            <div class="flex gap-4">
              <div class="mt-1 text-[#1e40af]">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/><polyline points="10 9 9 9 8 9"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Unified Document Intelligence</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Instantly query across CIMs, data rooms, and internal notes with AI that understands the nuances of private equity.
                </p>
              </div>
            </div>

            <!-- Feature 2 -->
            <div class="flex gap-4">
              <div class="mt-1 text-[#1e40af]">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Real-time Data Integration</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Connect your live market data feeds and internal databases directly into your workspace for up-to-the-minute analysis.
                </p>
              </div>
            </div>

            <!-- Feature 3 -->
            <div class="flex gap-4">
              <div class="mt-1 text-[#1e40af]">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Institutional Memory</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Capture and compound knowledge from every deal, meeting, and research note automatically, building a lasting competitive advantage.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonial Section -->
  <section class="py-12 px-6">
    <div class="max-w-[1200px] mx-auto">
      <div class="bg-gray-50 rounded-[32px] p-12 md:p-16 relative">
        <div class="mb-8 font-bold text-lg text-[#1e40af]">Peak Capital</div>
        <blockquote class="text-2xl md:text-3xl font-medium leading-tight text-gray-900 mb-12 max-w-4xl">
          "Horison has fundamentally changed how we approach due diligence. What used to take our associates days now takes minutes, with higher confidence in the output."
        </blockquote>
        <div class="flex items-center justify-between flex-wrap gap-6">
          <div class="flex items-center gap-4">
            <img src="/generated/image-portrait-of-a-confident-female-investmen-1771438801707-3.webp" alt="Sarah Chen" class="w-12 h-12 rounded-full object-cover" />
            <div>
              <div class="font-medium text-gray-900">Sarah Chen</div>
              <div class="text-sm text-gray-500">Managing Director, Peak Capital</div>
            </div>
          </div>
          <a href="#" class="inline-flex items-center gap-2 bg-[#1e40af] hover:opacity-90 text-white px-5 py-2.5 rounded-full text-sm font-medium transition-colors">
            Read Case Study
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m9 18 6-6-6-6"/></svg>
          </a>
        </div>
      </div>
    </div>
  </section>

  <!-- Feature Section 2 (Automation) -->
  <section class="py-24 px-6 bg-gray-50">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex flex-col md:flex-row-reverse gap-16 items-start">
        <!-- Visual -->
        <div class="w-full md:w-1/2 bg-white rounded-[32px] aspect-square relative flex items-center justify-center p-8 shadow-sm overflow-hidden group">
            <img src="/generated/image-close-up-of-a-tablet-screen-showing-an-a-1771438797163-1.webp" alt="Due Diligence Automation" class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" />
        </div>

        <!-- Content -->
        <div class="w-full md:w-1/2 pt-8">
          <div class="flex justify-between items-start mb-6">
            <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-gray-900 max-w-md">
              Move from data to decision, faster
            </h2>
            <span class="bg-[#1e40af] text-white px-3 py-1.5 rounded-full text-xs font-medium">Automation</span>
          </div>
          
          <p class="text-gray-600 text-lg mb-12 leading-relaxed">
            Automate the manual grind of due diligence without sacrificing depth. Horison surfaces the insights that matter most.
          </p>

          <div class="space-y-10">
            <!-- Feature 1 -->
            <div class="flex gap-4">
              <div class="mt-1 text-[#1e40af]">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"/><path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Automated CIM Analysis</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Extract key metrics, financial highlights, and potential risks from Confidential Information Memorandums in seconds.
                </p>
              </div>
            </div>

            <!-- Feature 2 -->
            <div class="flex gap-4">
              <div class="mt-1 text-[#1e40af]">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Risk Identification</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Surface red flags and inconsistencies hidden deep in unstructured data rooms and legal documents.
                </p>
              </div>
            </div>

            <!-- Feature 3 -->
            <div class="flex gap-4">
              <div class="mt-1 text-[#1e40af]">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"/><line x1="3" y1="9" x2="21" y2="9"/><line x1="9" y1="21" x2="9" y2="9"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Seamless Stack Integration</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Horison works where you work, integrating with Excel, your CRM, and existing data providers for a unified workflow.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Feature Section 3 (Scale) -->
  <section class="py-24 px-6 bg-white">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex flex-col md:flex-row gap-16 items-start">
        <!-- Visual -->
        <div class="w-full md:w-1/2 bg-gray-100 rounded-[32px] aspect-square relative flex items-center justify-center shadow-inner overflow-hidden group">
           <img src="/generated/image-a-diverse-team-of-investment-professiona-1771438799468-2.webp" alt="Scale with Horison" class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" />
        </div>

        <!-- Content -->
        <div class="w-full md:w-1/2 pt-8">
          <div class="flex justify-between items-start mb-6">
            <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-gray-900 max-w-md">
              Scale your expertise
            </h2>
            <span class="bg-[#1e40af] text-white px-3 py-1.5 rounded-full text-xs font-medium">Platform</span>
          </div>
          
          <p class="text-gray-600 text-lg mb-12 leading-relaxed">
            A multi-fund intelligence platform that grows with your assets under management, compounding your firm's edge over time.
          </p>

          <div class="space-y-4">
            <!-- Feature 1 (Active) -->
            <div class="bg-gray-50 p-6 rounded-xl border border-gray-100">
              <h3 class="font-medium text-gray-900 mb-2 text-sm">Cross-fund Insights</h3>
              <p class="text-gray-600 text-xs leading-relaxed">
                Identify patterns, synergies, and opportunities across your entire portfolio and fund history with global search and analysis.
              </p>
            </div>

            <!-- Feature 2 -->
            <div class="p-6 rounded-xl border border-gray-100 hover:bg-gray-50 transition-colors cursor-pointer">
              <h3 class="font-medium text-gray-500 mb-0 text-sm">Proprietary Knowledge Moat</h3>
            </div>

            <!-- Feature 3 -->
            <div class="p-6 rounded-xl border border-gray-100 hover:bg-gray-50 transition-colors cursor-pointer">
              <h3 class="font-medium text-gray-500 mb-0 text-sm">Enterprise-grade Security</h3>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Security Section -->
  <section class="py-24 px-6 bg-[#1A1A1A] text-white">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex flex-col md:flex-row gap-16 items-start">
        <!-- Visual (Left) -->
        <div class="w-full md:w-1/2 bg-[#111111] rounded-[32px] aspect-square relative flex items-center justify-center p-8 border border-white/10 overflow-hidden">
           <img src="/generated/image-a-busy-trading-floor-or-investment-firm--1771438803805-4.webp" alt="Security and Compliance" class="w-full h-full object-cover opacity-30" />
           <div class="absolute inset-0 flex items-center justify-center">
             <div class="text-center">
               <div class="bg-[#1e40af] text-white px-6 py-3 rounded-full font-medium shadow-xl">
                 Enterprise Grade Security
               </div>
             </div>
           </div>
        </div>

        <!-- Content (Right) -->
        <div class="w-full md:w-1/2 pt-8">
          <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-white mb-6">
            Trusted by the most rigorous firms
          </h2>
          
          <p class="text-gray-400 text-lg mb-12 leading-relaxed">
            Horison is built with the highest commitment to data privacy, security, and institutional-grade compliance. Your proprietary data never leaves your secure environment.
          </p>

          <div class="divide-y divide-white/10 border-t border-b border-white/10">
            {#each ['Data Isolation', 'SOC2 Type II Compliant', 'Granular Access Control', 'Full Audit Logging', 'End-to-End Encryption'] as item, i}
              <div class="py-4">
                <div class="flex justify-between items-center cursor-pointer group">
                  <h3 class="font-medium text-gray-300 group-hover:text-white transition-colors text-sm">{item}</h3>
                  {#if i === 0}
                  <p class="mt-2 text-gray-500 text-xs max-w-md">Your firm's data is logically isolated and never used to train models for other customers.</p>
                  {/if}
                </div>
              </div>
            {/each}
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Results Section -->
  <section class="py-24 px-6">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex justify-between items-end mb-16">
        <div class="max-w-xl">
          <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-gray-900 mb-6">
            Higher confidence. Faster decisions.
          </h2>
          <p class="text-gray-600 text-lg leading-relaxed">
            Investment teams using Horison see immediate improvements in workflow efficiency and knowledge retention.
          </p>
        </div>
        <span class="bg-[#1e40af] text-white px-3 py-1.5 rounded-full text-xs font-medium mb-2">Impact</span>
      </div>

      <div class="grid md:grid-cols-3 gap-8">
        <!-- Card 1 -->
        <div class="group">
          <div class="bg-gray-50 p-10 rounded-2xl mb-6">
            <div class="text-5xl font-bold text-[#1e40af] mb-2">30%</div>
            <div class="text-gray-600 font-medium">Faster Due Diligence</div>
          </div>
          <p class="text-gray-600 leading-snug">
            Reduce the time spent on manual document review and data extraction by nearly a third.
          </p>
        </div>

        <!-- Card 2 -->
        <div class="group">
          <div class="bg-gray-50 p-10 rounded-2xl mb-6">
            <div class="text-5xl font-bold text-[#1e40af] mb-2">90%</div>
            <div class="text-gray-600 font-medium">Reduction in Manual Entry</div>
          </div>
          <p class="text-gray-600 leading-snug">
            Automate the flow of data from documents directly into your models and CRM.
          </p>
        </div>

        <!-- Card 3 -->
        <div class="group">
          <div class="bg-gray-50 p-10 rounded-2xl mb-6">
            <div class="text-5xl font-bold text-[#1e40af] mb-2">100%</div>
            <div class="text-gray-600 font-medium">Knowledge Retention</div>
          </div>
          <p class="text-gray-600 leading-snug">
            Never lose institutional memory when team members move on. Every insight is captured.
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- CTA Section -->
  <section class="py-32 px-6 text-center bg-gray-50">
    <div class="max-w-[1200px] mx-auto">
      <h2 class="text-4xl md:text-5xl font-medium text-gray-900 mb-6 tracking-tight">
        Ready to unify your investment intelligence?
      </h2>
      <p class="text-gray-600 text-lg max-w-2xl mx-auto mb-10">
        Join the leading private market firms building their institutional knowledge moat with Horison.
      </p>
      <div class="flex flex-col sm:flex-row gap-4 justify-center">
        <a href="#" class="inline-block bg-[#1e40af] hover:opacity-90 text-white px-8 py-4 rounded-full font-medium transition-colors">
          Book a Demo
        </a>
        <a href="#" class="inline-block bg-white border border-gray-200 hover:bg-gray-50 text-gray-900 px-8 py-4 rounded-full font-medium transition-colors">
          Contact Sales
        </a>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-white pt-20 pb-10 px-6 border-t border-gray-100">
    <div class="max-w-[1200px] mx-auto">
      <div class="grid grid-cols-2 md:grid-cols-6 gap-12 mb-20">
        <div class="col-span-2">
          <a href="/" class="flex items-center gap-2 mb-6">
            <Logo className="w-7 h-7 text-[#1e40af]" />
            <span class="text-[#1e40af] font-semibold text-lg tracking-widest">HORISON</span>
          </a>
          <p class="text-gray-500 text-sm max-w-xs">
            The AI-native workspace for private market investment teams.
          </p>
        </div>
        
        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Product</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">Intelligence</a></li>
            <li><a href="#" class="hover:text-gray-900">Automation</a></li>
            <li><a href="#" class="hover:text-gray-900">Integrations</a></li>
            <li><a href="#" class="hover:text-gray-900">Security</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Solutions</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">Private Equity</a></li>
            <li><a href="#" class="hover:text-gray-900">Venture Capital</a></li>
            <li><a href="#" class="hover:text-gray-900">Real Estate</a></li>
            <li><a href="#" class="hover:text-gray-900">Private Credit</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Resources</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">Case Stories</a></li>
            <li><a href="#" class="hover:text-gray-900">Blog</a></li>
            <li><a href="#" class="hover:text-gray-900">Documentation</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Company</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">About</a></li>
            <li><a href="#" class="hover:text-gray-900">Careers</a></li>
            <li><a href="#" class="hover:text-gray-900">Contact</a></li>
          </ul>
        </div>
      </div>

      <div class="flex flex-col md:flex-row justify-between items-center pt-8 border-t border-gray-100">
        <div class="flex flex-col md:flex-row items-center gap-6 mb-4 md:mb-0">
          <div class="text-xs text-gray-500">
            © 2025 Horison AI. All rights reserved.
            <a href="#" class="ml-4 hover:text-gray-900">Privacy Policy</a>
            <a href="#" class="ml-4 hover:text-gray-900">Terms of Service</a>
          </div>
        </div>

        <div class="flex items-center gap-4 text-gray-400">
          <a href="#" class="hover:text-gray-900"><svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg></a>
          <a href="#" class="hover:text-gray-900"><svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg></a>
        </div>
      </div>
    </div>
  </footer>
</div>



