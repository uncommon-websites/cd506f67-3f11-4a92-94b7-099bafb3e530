<script>
  let activeTab = 'Global Transfers';
  const tabs = ['Accounts', 'Global Transfers', 'Debit Cards', 'Business Banking', 'Wealth Management', 'Treasury'];
</script>

<section class="pt-32 pb-20 px-6 max-w-7xl mx-auto">
  <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 mb-16">
    <div>
      <h1 class="text-5xl md:text-6xl font-medium tracking-tight text-black leading-[1.1] mb-8">
        Operate globally <br /> with ease
      </h1>
    </div>
    <div class="flex flex-col justify-end items-start lg:pl-12">
      <p class="text-xl text-gray-600 mb-6 max-w-md leading-relaxed">
        Receive fiat payments, convert to stablecoins, and pay suppliers worldwide. Banking infrastructure built for businesses and individuals with global cash flows.
      </p>
      <a href="#" class="group inline-flex items-center text-black font-medium hover:opacity-70 transition-opacity">
        Open an Account
        <span class="ml-1 group-hover:translate-x-1 transition-transform">→</span>
      </a>
    </div>
  </div>

  <!-- Interactive Visual Section -->
  <div class="rounded-3xl overflow-hidden bg-gray-50 border border-gray-200 shadow-sm">
    <!-- Tabs -->
    <div class="flex overflow-x-auto scrollbar-hide border-b border-gray-200 bg-white/50 backdrop-blur-sm">
      {#each tabs as tab}
        <button 
          class="px-5 py-4 text-sm font-medium whitespace-nowrap transition-colors relative {activeTab === tab ? 'text-black' : 'text-gray-500 hover:text-gray-800'}"
          on:click={() => activeTab = tab}
        >
          {tab}
          {#if activeTab === tab}
            <div class="absolute bottom-0 left-0 right-0 h-0.5 bg-black"></div>
          {/if}
        </button>
      {/each}
    </div>

    <!-- Content Area -->
    <div class="relative h-[500px] bg-gradient-to-br from-gray-900 to-gray-800 overflow-hidden group">
      <!-- Background Pattern -->
      <div class="absolute inset-0 opacity-10" 
           style="background-image: linear-gradient(rgba(255,255,255,0.1) 1px, transparent 1px), linear-gradient(90deg, rgba(255,255,255,0.1) 1px, transparent 1px); background-size: 40px 40px;">
      </div>
      
      <!-- Floating Banking Card -->
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-80 bg-white/95 backdrop-blur-md border border-gray-200 rounded-2xl p-6 shadow-2xl">
        <div class="flex justify-between items-center mb-6">
          <span class="text-xs font-medium text-gray-500">Recent Activity</span>
          <span class="text-xs font-medium text-gray-900">USD Balance</span>
        </div>
        
        <div class="mb-6">
          <div class="text-3xl font-semibold text-gray-900 mb-1">$124,850.00</div>
          <div class="text-xs text-green-600">+$2,450.00 this month</div>
        </div>
        
        <!-- Transaction 1 -->
        <div class="flex items-center gap-3 mb-4 pb-4 border-b border-gray-100">
          <div class="w-10 h-10 rounded-full bg-gray-100 flex items-center justify-center text-gray-700 shrink-0">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 12V7H5a2 2 0 0 1 0-4h14v4"></path><path d="M3 5v14a2 2 0 0 0 2 2h16v-5"></path><line x1="18" y1="12" x2="18" y2="12"></line></svg>
          </div>
          <div class="flex-1 min-w-0">
            <div class="flex justify-between items-baseline">
              <h3 class="text-sm font-medium text-gray-900 truncate">International Wire</h3>
              <span class="text-sm font-medium text-gray-900">$50,000.00</span>
            </div>
            <div class="flex justify-between items-baseline">
              <p class="text-xs text-gray-500">To: London Office</p>
              <p class="text-xs text-green-600">No fees</p>
            </div>
          </div>
        </div>

        <!-- Transaction 2 -->
        <div class="flex items-center gap-3">
          <div class="w-10 h-10 rounded-full bg-gray-100 flex items-center justify-center text-gray-700 shrink-0">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="1" y="4" width="22" height="16" rx="2" ry="2"></rect><line x1="1" y1="10" x2="23" y2="10"></line></svg>
          </div>
          <div class="flex-1 min-w-0">
            <div class="flex justify-between items-baseline">
              <h3 class="text-sm font-medium text-gray-900 truncate">Card Payment</h3>
              <span class="text-sm font-medium text-gray-900">$2,450.00</span>
            </div>
            <div class="flex justify-between items-baseline">
              <p class="text-xs text-gray-500">Business Expenses</p>
              <p class="text-xs text-gray-400">Instant</p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Feature Highlights -->
    <div class="bg-white p-6 border-t border-gray-200">
      <div class="grid grid-cols-3 gap-6 text-center">
        <div>
          <div class="text-2xl font-semibold text-gray-900 mb-1">$0</div>
          <div class="text-xs text-gray-500">Wire Transfer Fees</div>
        </div>
        <div>
          <div class="text-2xl font-semibold text-gray-900 mb-1">24/7</div>
          <div class="text-xs text-gray-500">Global Access</div>
        </div>
        <div>
          <div class="text-2xl font-semibold text-gray-900 mb-1">Instant</div>
          <div class="text-xs text-gray-500">Settlement</div>
        </div>
      </div>
    </div>
  </div>
</section>
