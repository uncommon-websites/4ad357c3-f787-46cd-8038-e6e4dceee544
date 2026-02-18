<script lang="ts">
  import Logo from './Logo.svelte';
</script>

<nav class="fixed top-0 left-0 right-0 z-50 bg-white/90 backdrop-blur-sm transition-all duration-300 border-b border-gray-100/50">
  <!-- Announcement Bar -->
  <div class="w-full py-2 text-center bg-[#f7f7f7] border-b border-transparent hidden md:block">
    <a href="#" class="text-[11px] md:text-xs text-gray-500 hover:text-gray-700 underline decoration-1 underline-offset-2 font-medium tracking-wide">
      Watch Horison Summit on-demand.
    </a>
  </div>

  <div class="max-w-[1400px] mx-auto px-6 h-20 flex items-center justify-between">
    <!-- Logo -->
    <div class="flex-shrink-0">
      <a href="/" class="flex items-center gap-2">
        <Logo className="w-7 h-7 text-[#1e40af]" />
        <span class="text-[#1e40af] font-semibold text-lg tracking-widest">HORISON</span>
      </a>
    </div>

    <!-- Navigation -->
    <div class="hidden md:flex items-center gap-10 text-[15px] font-normal text-gray-600">
      <a href="#" class="hover:text-gray-900 transition-colors">Product</a>
      <a href="#" class="hover:text-gray-900 transition-colors">Industries</a>
      <a href="#" class="hover:text-gray-900 transition-colors">Customers</a>
      <a href="#" class="hover:text-gray-900 transition-colors">Company</a>
    </div>

    <!-- Actions -->
    <div class="flex items-center gap-6 text-[15px] font-medium">
      <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors hidden sm:block font-normal">Sign in</a>
      <a href="#" style="background-color: #1e40af" class="hover:opacity-90 text-white px-5 py-2.5 rounded-full transition-colors">
        Book Demo
      </a>
    </div>
  </div>
</nav>
