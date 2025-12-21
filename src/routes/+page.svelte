<script>
  import { onMount } from 'svelte';

  const images = [
    "/generated/image-luxury-minimalist-watch-with-leather-str-1766338611879-0.webp",
    "/generated/image-modern-wireless-earbuds-in-charging-case-1766338614852-1.webp",
    "/generated/image-elegant-gold-jewelry-necklace-with-penda-1766338617166-2.webp",
    "/generated/image-stylish-minimalist-backpack-in-neutral-c-1766338619677-3.webp",
    "/generated/image-modern-led-desk-lamp-with-sleek-design-p-1766338622204-4.webp"
  ];

  let showCookieBanner = $state(true);
</script>

<div class="font-sans text-[#111] antialiased bg-white selection:bg-black selection:text-white">
  <!-- Header -->
  <header class="fixed top-0 left-0 w-full z-50 flex justify-between items-center px-6 py-5 bg-white/90 backdrop-blur-sm border-b border-gray-100">
    <div class="flex items-center gap-2">
      <div class="w-8 h-8 text-primary-600">
        <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M12.2566 21.954C17.929 21.954 22.5274 17.484 22.5274 11.9699C22.5274 6.45586 17.929 1.98584 12.2566 1.98584C6.58422 1.98584 1.98584 6.45586 1.98584 11.9699C1.98584 17.484 6.58422 21.954 12.2566 21.954ZM15.4608 6.63684C15.6167 6.09831 15.0791 5.77985 14.5881 6.1199L7.73395 10.8665C7.20146 11.2352 7.28522 11.9699 7.85977 11.9699H9.66465V11.9563H13.1823L10.3161 12.9394L9.05251 17.303C8.89655 17.8415 9.43412 18.16 9.92517 17.8199L16.7793 13.0734C17.3118 12.7046 17.228 11.9699 16.6535 11.9699H13.9165L15.4608 6.63684Z"
            fill="currentColor"
          />
        </svg>
      </div>
      <span class="text-xl font-semibold tracking-tight">Dropmagic</span>
    </div>
    <nav class="hidden md:flex items-center gap-8 text-sm font-medium">
      <a href="#platform" class="hover:opacity-70 transition-opacity">Platform</a>
      <a href="#pricing" class="hover:opacity-70 transition-opacity">Pricing</a>
      <a href="#academy" class="hover:opacity-70 transition-opacity">Academy</a>
      <a href="#blog" class="hover:opacity-70 transition-opacity">Blog</a>
      <a href="#affiliate" class="flex items-center gap-1.5 hover:opacity-70 transition-opacity">
        <span class="bg-primary-600 text-white text-[10px] font-bold px-1.5 py-0.5 rounded-sm">20%</span>
        Affiliate
      </a>
      <a href="#trial" class="bg-primary-600 text-white px-5 py-2 rounded-sm hover:bg-primary-700 transition-colors">
        Start Free Trial
      </a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="pt-40 pb-20 px-6 max-w-[1400px] mx-auto">
    <div class="max-w-4xl mb-24">
      <div class="inline-flex items-center gap-2 bg-primary-50 text-primary-700 px-4 py-2 rounded-full text-sm font-medium mb-6">
        <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 20 20">
          <path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/>
        </svg>
        500,000+ stores generated • 2M+ TikTok views
      </div>
      <h1 class="text-6xl md:text-7xl font-semibold tracking-tight leading-[1.1] mb-8">
        Generate Shopify stores<br>in <span class="text-primary-600">10 minutes</span>
      </h1>
      <div class="flex flex-col md:flex-row justify-between items-start md:items-end gap-8">
        <p class="text-lg md:text-xl max-w-md leading-relaxed text-gray-700">
          AI-powered store builder for dropshippers. Automated product scraping, conversion-optimized design, and instant deployment.
        </p>
        <div class="flex flex-col sm:flex-row gap-3">
          <button class="bg-primary-600 text-white px-8 py-3.5 text-sm font-semibold rounded-sm hover:bg-primary-700 transition-colors shadow-sm">
            Start Free Trial
          </button>
          <button class="bg-white text-gray-900 border border-gray-200 px-8 py-3.5 text-sm font-semibold rounded-sm hover:bg-gray-50 transition-colors">
            Watch Demo
          </button>
        </div>
      </div>
    </div>

    <!-- Hero Images Grid -->
    <div class="grid grid-cols-2 md:grid-cols-5 gap-4">
      {#each images as src, i}
        <div class="aspect-[3/4] overflow-hidden bg-gray-100 rounded-sm shadow-sm">
          <img {src} alt="Dropshipping product example {i + 1}" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
        </div>
      {/each}
    </div>
  </section>

  <!-- Floating Images Section -->
  <section class="py-32 px-6 max-w-[1400px] mx-auto relative min-h-[800px]">
    <div class="absolute inset-0 flex items-center justify-center pointer-events-none z-10">
      <h2 class="text-2xl md:text-3xl font-semibold text-center max-w-2xl leading-snug bg-white/90 backdrop-blur-sm p-6 rounded-xl shadow-sm">
        57+ conversion-optimized sections.<br>Built for dropshipping success.
      </h2>
    </div>

    <!-- Scattered Images with 'Add to cart' -->
    <div class="relative w-full h-full min-h-[800px]">
      <!-- Image 1: Earbuds (Left) -->
      <div class="absolute top-20 left-[10%] w-64 aspect-[3/4]">
        <img src={images[1]} alt="Wireless earbuds" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <div class="w-3 h-3 bg-primary-600 rounded-full mx-auto mb-2 animate-pulse"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-md whitespace-nowrap hover:bg-white transition-colors font-medium">Add to cart</button>
        </div>
      </div>

      <!-- Image 2: Backpack (Center Top) -->
      <div class="absolute top-0 left-[45%] w-56 aspect-[3/4]">
        <img src={images[3]} alt="Minimalist backpack" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/3 left-1/3">
             <div class="w-3 h-3 bg-primary-600 rounded-full mb-2 animate-pulse"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-md whitespace-nowrap hover:bg-white transition-colors font-medium">Add to cart</button>
        </div>
      </div>

       <!-- Image 3: Lamp (Right Top) -->
      <div class="absolute top-40 right-[5%] w-64 aspect-[3/4]">
        <img src={images[4]} alt="LED desk lamp" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute bottom-1/3 right-1/4">
             <div class="w-3 h-3 bg-primary-600 rounded-full mb-2 animate-pulse ml-auto"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-md whitespace-nowrap hover:bg-white transition-colors font-medium">Add to cart</button>
        </div>
      </div>

      <!-- Image 4: Watch (Left Bottom) -->
      <div class="absolute bottom-20 left-[5%] w-56 aspect-[3/4]">
        <img src={images[0]} alt="Luxury watch" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-md whitespace-nowrap hover:bg-white transition-colors font-medium">Add to cart</button>
        </div>
      </div>

      <!-- Image 5: Jewelry (Center Bottom) -->
      <div class="absolute bottom-0 left-[35%] w-48 aspect-[3/4]">
        <img src={images[2]} alt="Gold necklace" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-md whitespace-nowrap hover:bg-white transition-colors font-medium">Add to cart</button>
        </div>
      </div>
    </div>
  </section>

  <!-- Dark Section 1: Speed & Automation -->
  <section class="bg-[#111] text-white py-32 px-6">
    <div class="max-w-[1400px] mx-auto">
      <div class="flex flex-col md:flex-row justify-between items-start mb-20 gap-8">
        <h2 class="text-4xl md:text-5xl font-semibold tracking-tight max-w-xl">
          Launch while competitors<br>are still designing
        </h2>
        <p class="text-gray-400 text-lg max-w-md leading-relaxed">
          Generate a complete, conversion-optimized Shopify store in 10 minutes. AI handles design, copywriting, and product imports automatically.
        </p>
      </div>

      <!-- Interactive Box -->
      <div class="w-full aspect-video bg-[#1a1a1a] rounded-sm mb-16 flex items-center justify-center relative overflow-hidden group border border-white/5">
        <div class="text-4xl md:text-6xl font-light tracking-tight text-white/90">
          <span class="text-primary-400">dropmagic.ai/</span>mystorename<span class="animate-pulse">|</span>
        </div>
        <!-- Subtle grid or gradient could go here -->
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-12 border-t border-white/10 pt-12">
        <div>
          <h3 class="text-lg font-semibold mb-3">10-minute setup</h3>
          <p class="text-gray-400 leading-relaxed">From product idea to live store faster than any competitor.</p>
        </div>
        <div>
          <h3 class="text-lg font-semibold mb-3">AI-powered automation</h3>
          <p class="text-gray-400 leading-relaxed">Automated branding, copywriting, and design generation.</p>
        </div>
        <div>
          <h3 class="text-lg font-semibold mb-3">Mobile-first design</h3>
          <p class="text-gray-400 leading-relaxed">Every section optimized for mobile conversions automatically.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Dark Section 2: Product Import -->
  <section class="bg-[#111] text-white py-32 px-6 border-t border-white/5">
    <div class="max-w-[1400px] mx-auto">
      <div class="flex flex-col md:flex-row justify-between items-start mb-20 gap-8">
        <h2 class="text-4xl md:text-5xl font-semibold tracking-tight">
          One-click product<br>import from AliExpress
        </h2>
        <p class="text-gray-400 text-lg max-w-md leading-relaxed">
          Automatically scrape product titles, images, descriptions, and reviews. AI generates native-sounding copy in English, French, or Spanish.
        </p>
      </div>

      <!-- Interactive Box -->
      <div class="w-full aspect-[2/1] bg-[#1a1a1a] rounded-sm flex items-center justify-center border border-white/5 relative overflow-hidden">
         <div class="absolute inset-0 bg-gradient-to-br from-primary-900/20 to-transparent"></div>
         <div class="text-3xl md:text-5xl font-light tracking-tight text-white/90 relative z-10">
          <span class="text-primary-400">Import from</span> aliexpress.com<span class="animate-pulse">|</span>
        </div>
      </div>
    </div>
  </section>

  <!-- Light Gray Section -->
  <section class="bg-[#f5f5f5] py-24 px-6">
    <div class="max-w-[1400px] mx-auto grid grid-cols-1 md:grid-cols-3 gap-12">
      <div>
        <h3 class="text-lg font-semibold mb-3 text-[#111]">57+ conversion sections</h3>
        <p class="text-gray-600 leading-relaxed">Pre-built, tested sections that drive sales. Fresh sections added monthly.</p>
      </div>
      <div>
        <h3 class="text-lg font-semibold mb-3 text-[#111]">Unlimited AI copywriting</h3>
        <p class="text-gray-600 leading-relaxed">Generate product descriptions, headlines, and marketing copy instantly.</p>
      </div>
      <div>
        <h3 class="text-lg font-semibold mb-3 text-[#111]">Multilingual support</h3>
        <p class="text-gray-600 leading-relaxed">Native-sounding translations in English, French, and Spanish.</p>
      </div>
    </div>
  </section>

  <!-- Built for Dropshippers -->
  <section class="bg-[#f0f0f0] py-32 px-6">
    <div class="max-w-[1400px] mx-auto">
      <div class="mb-16">
        <h2 class="text-4xl md:text-5xl font-semibold tracking-tight mb-6 text-[#111]">
          Everything dropshippers need
        </h2>
        <p class="text-gray-600 text-lg max-w-2xl leading-relaxed">
          From product import to store launch, Dropmagic automates every step. Focus on marketing while AI handles design, copy, and technical setup.
        </p>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-start">
        <!-- Visual -->
        <div class="bg-gradient-to-br from-primary-950 to-[#111] aspect-video rounded-xl flex items-center justify-center relative overflow-hidden perspective-1000 border border-primary-900/20">
           <!-- Abstract Wireframe Animation -->
           <div class="relative w-64 h-40 flex items-center justify-center transform-style-3d">
              {#each [0, 1, 2, 3, 4] as i}
                <div 
                  class="absolute w-32 h-48 border border-primary-400/30 bg-primary-500/5 backdrop-blur-sm rounded-sm transition-transform duration-500"
                  style="
                    transform: translateX({(i - 2) * 40}px) translateZ({Math.abs(i - 2) * -20}px) rotateY({(i - 2) * 10}deg);
                    z-index: {10 - Math.abs(i - 2)};
                  "
                ></div>
              {/each}
              <!-- Central Highlight -->
              <div class="absolute w-32 h-48 border border-primary-400/60 shadow-[0_0_20px_rgba(139,92,246,0.3)] rounded-sm z-20"></div>
           </div>
        </div>

        <!-- List -->
        <div class="space-y-12 pt-4">
          <div class="group cursor-pointer">
            <h3 class="text-xl font-semibold mb-3 text-[#111]">AI branding generator</h3>
            <p class="text-gray-600 leading-relaxed">Automatic color palettes, font pairings, and brand identity generation for professional-looking stores.</p>
          </div>
          <div class="group cursor-pointer opacity-40 hover:opacity-100 transition-opacity">
            <h3 class="text-xl font-semibold mb-3 text-[#111]">Automated product scraping</h3>
            <p class="text-gray-600 leading-relaxed">Import products with titles, images, descriptions, and reviews from AliExpress in one click.</p>
          </div>
          <div class="group cursor-pointer opacity-40 hover:opacity-100 transition-opacity">
            <h3 class="text-xl font-semibold mb-3 text-[#111]">Conversion optimization</h3>
            <p class="text-gray-600 leading-relaxed">Every section tested for maximum conversions. Mobile-first design that drives sales.</p>
          </div>

          <div class="flex gap-4 pt-8">
             <button class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center text-gray-400 hover:border-primary-600 hover:text-primary-600 transition-colors">←</button>
             <button class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center text-gray-400 hover:border-primary-600 hover:text-primary-600 transition-colors">→</button>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Fast to Launch -->
  <section class="bg-white py-32 px-6">
    <div class="max-w-[1400px] mx-auto">
      <h2 class="text-4xl md:text-5xl font-semibold tracking-tight mb-20 text-[#111]">
        Start free, scale fast
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-12">
        <!-- Card 1 -->
        <div>
          <div class="w-14 h-14 bg-primary-600 text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-7 h-7">
              <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 13.5l10.5-11.25L12 10.5h8.25L9.75 21.75 12 13.5H3.75z" />
            </svg>
          </div>
          <h3 class="text-lg font-semibold mb-3 text-[#111]">10-minute store creation</h3>
          <p class="text-gray-600 leading-relaxed">From product idea to live Shopify store in just 10 minutes. No design or coding skills required.</p>
        </div>

        <!-- Card 2 -->
        <div>
          <div class="w-14 h-14 bg-primary-600 text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-7 h-7">
              <path stroke-linecap="round" stroke-linejoin="round" d="M12 21a9.004 9.004 0 008.716-6.747M12 21a9.004 9.004 0 01-8.716-6.747M12 21c2.485 0 4.5-4.03 4.5-9S14.485 3 12 3m0 18c-2.485 0-4.5-4.03-4.5-9S9.515 3 12 3m0 0a8.997 8.997 0 017.843 4.582M12 3a8.997 8.997 0 00-7.843 4.582m15.686 0A11.953 11.953 0 0112 10.5c-2.998 0-5.74-1.1-7.843-2.918m15.686 0A8.959 8.959 0 0121 12c0 .778-.099 1.533-.284 2.253m0 0A17.919 17.919 0 0112 16.5c-3.162 0-6.133-.815-8.716-2.247m0 0A9.015 9.015 0 013 12c0-1.605.42-3.113 1.157-4.418" />
            </svg>
          </div>
          <h3 class="text-lg font-semibold mb-3 text-[#111]">Free .store domain</h3>
          <p class="text-gray-600 leading-relaxed">Every store includes a free .store domain. Professional branding from day one.</p>
        </div>

        <!-- Card 3 -->
        <div>
          <div class="w-14 h-14 bg-primary-600 text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-7 h-7">
              <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 16.875h3.375m0 0h3.375m-3.375 0V13.5m0 3.375v3.375M6 10.5h2.25a2.25 2.25 0 002.25-2.25V6a2.25 2.25 0 00-2.25-2.25H6A2.25 2.25 0 003.75 6v2.25A2.25 2.25 0 006 10.5zm0 9.75h2.25A2.25 2.25 0 0010.5 18v-2.25a2.25 2.25 0 00-2.25-2.25H6a2.25 2.25 0 00-2.25 2.25V18A2.25 2.25 0 006 20.25zm9.75-9.75H18a2.25 2.25 0 002.25-2.25V6A2.25 2.25 0 0018 3.75h-2.25A2.25 2.25 0 0013.5 6v2.25a2.25 2.25 0 002.25 2.25z" />
            </svg>
          </div>
          <h3 class="text-lg font-semibold mb-3 text-[#111]">Seamless Shopify integration</h3>
          <p class="text-gray-600 leading-relaxed">Direct integration with Shopify, DSers, and Kaching Bundle. Start selling immediately.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Pricing Section -->
  <section id="pricing" class="bg-gradient-to-b from-gray-50 to-white py-32 px-6">
    <div class="max-w-[1400px] mx-auto">
      <div class="text-center mb-16">
        <h2 class="text-4xl md:text-5xl font-semibold tracking-tight mb-6 text-[#111]">
          Simple, transparent pricing
        </h2>
        <p class="text-gray-600 text-lg max-w-2xl mx-auto">
          Start free and upgrade when you're ready. No hidden fees, cancel anytime.
        </p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-8 max-w-5xl mx-auto">
        <!-- Free Plan -->
        <div class="bg-white border-2 border-gray-200 rounded-xl p-8 hover:shadow-lg transition-shadow">
          <div class="mb-6">
            <h3 class="text-2xl font-semibold mb-2">Free</h3>
            <div class="flex items-baseline gap-2 mb-4">
              <span class="text-5xl font-bold">$0</span>
              <span class="text-gray-500">/month</span>
            </div>
            <p class="text-gray-600">Perfect for getting started</p>
          </div>
          
          <ul class="space-y-4 mb-8">
            <li class="flex items-start gap-3">
              <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
              </svg>
              <span class="text-gray-700">Unlimited store creation</span>
            </li>
            <li class="flex items-start gap-3">
              <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
              </svg>
              <span class="text-gray-700">57+ conversion sections</span>
            </li>
            <li class="flex items-start gap-3">
              <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
              </svg>
              <span class="text-gray-700">Monthly section updates</span>
            </li>
            <li class="flex items-start gap-3">
              <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
              </svg>
              <span class="text-gray-700">Basic customization</span>
            </li>
          </ul>

          <button class="w-full bg-gray-100 text-gray-900 px-6 py-3 rounded-sm font-semibold hover:bg-gray-200 transition-colors">
            Start Free
          </button>
        </div>

        <!-- PRO Plan -->
        <div class="bg-gradient-to-br from-primary-600 to-primary-700 text-white rounded-xl p-8 relative overflow-hidden shadow-xl">
          <div class="absolute top-4 right-4">
            <span class="bg-white/20 backdrop-blur-sm text-white text-xs font-bold px-3 py-1 rounded-full">POPULAR</span>
          </div>
          
          <div class="mb-6">
            <h3 class="text-2xl font-semibold mb-2">PRO</h3>
            <div class="flex items-baseline gap-2 mb-4">
              <span class="text-5xl font-bold">$79</span>
              <span class="text-primary-100">/month</span>
            </div>
            <p class="text-primary-100">Everything you need to scale</p>
          </div>
          
          <ul class="space-y-4 mb-8">
            <li class="flex items-start gap-3">
              <svg class="w-5 h-5 text-white mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
              </svg>
              <span class="text-white font-medium">Everything in Free, plus:</span>
            </li>
            <li class="flex items-start gap-3">
              <svg class="w-5 h-5 text-white mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
              </svg>
              <span class="text-white">Unlimited AI copywriting</span>
            </li>
            <li class="flex items-start gap-3">
              <svg class="w-5 h-5 text-white mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
              </svg>
              <span class="text-white">AI image generation</span>
            </li>
            <li class="flex items-start gap-3">
              <svg class="w-5 h-5 text-white mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
              </svg>
              <span class="text-white">One-click product import</span>
            </li>
            <li class="flex items-start gap-3">
              <svg class="w-5 h-5 text-white mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
              </svg>
              <span class="text-white">Free .store domain</span>
            </li>
            <li class="flex items-start gap-3">
              <svg class="w-5 h-5 text-white mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
              </svg>
              <span class="text-white">Priority support</span>
            </li>
          </ul>

          <button class="w-full bg-white text-primary-600 px-6 py-3 rounded-sm font-semibold hover:bg-primary-50 transition-colors">
            Start PRO Trial
          </button>
        </div>
      </div>

      <p class="text-center text-gray-500 text-sm mt-8">
        No credit card required • Cancel anytime • Products remain accessible after cancellation
      </p>
    </div>
  </section>

  <!-- CTA Banner -->
  <section class="px-6 py-12">
    <div class="max-w-[1400px] mx-auto border border-primary-200 rounded-xl p-8 md:p-12 flex flex-col md:flex-row justify-between items-center gap-8 bg-gradient-to-br from-primary-50 to-white shadow-sm">
      <div class="flex items-center gap-6">
        <div class="flex gap-1 h-8">
           <div class="w-2 bg-primary-600 h-full rounded-full"></div>
           <div class="w-2 bg-primary-600 h-full rounded-full"></div>
           <div class="w-2 bg-primary-600 h-full rounded-full"></div>
           <div class="w-2 bg-primary-300 h-full rounded-full"></div>
        </div>
        <div>
          <h2 class="text-2xl md:text-3xl font-semibold tracking-tight mb-1">Ready to launch your store?</h2>
          <p class="text-gray-600 text-sm">Start free at $0/month. No credit card required.</p>
        </div>
      </div>
      <button class="bg-primary-600 text-white px-8 py-3.5 text-sm font-semibold rounded-sm hover:bg-primary-700 transition-colors whitespace-nowrap shadow-sm">
        Start Free Trial
      </button>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-white pt-20 pb-10 px-6 border-t border-gray-100">
    <div class="max-w-[1400px] mx-auto">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-12 md:gap-24 mb-20">
        <div class="col-span-1 md:col-span-2">
          <div class="flex items-center gap-2 mb-3">
            <div class="w-8 h-8 text-primary-600">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M12.2566 21.954C17.929 21.954 22.5274 17.484 22.5274 11.9699C22.5274 6.45586 17.929 1.98584 12.2566 1.98584C6.58422 1.98584 1.98584 6.45586 1.98584 11.9699C1.98584 17.484 6.58422 21.954 12.2566 21.954ZM15.4608 6.63684C15.6167 6.09831 15.0791 5.77985 14.5881 6.1199L7.73395 10.8665C7.20146 11.2352 7.28522 11.9699 7.85977 11.9699H9.66465V11.9563H13.1823L10.3161 12.9394L9.05251 17.303C8.89655 17.8415 9.43412 18.16 9.92517 17.8199L16.7793 13.0734C17.3118 12.7046 17.228 11.9699 16.6535 11.9699H13.9165L15.4608 6.63684Z"
                  fill="currentColor"
                />
              </svg>
            </div>
            <h3 class="text-xl font-semibold">Dropmagic</h3>
          </div>
          <p class="text-gray-500 text-base mb-4">Generate Shopify stores in minutes</p>
          <p class="text-gray-400 text-sm max-w-md">AI-powered store builder for dropshippers. 500,000+ stores generated.</p>
        </div>

        <div>
          <h4 class="text-sm font-semibold mb-4 text-gray-900">Product</h4>
          <ul class="space-y-3 text-sm">
            <li><a href="#platform" class="text-gray-600 hover:text-primary-600 transition-colors">Platform</a></li>
            <li><a href="#pricing" class="text-gray-600 hover:text-primary-600 transition-colors">Pricing</a></li>
            <li><a href="#academy" class="text-gray-600 hover:text-primary-600 transition-colors">Academy</a></li>
            <li><a href="#inspiration" class="text-gray-600 hover:text-primary-600 transition-colors">Inspiration Gallery</a></li>
          </ul>
        </div>

        <div>
          <h4 class="text-sm font-semibold mb-4 text-gray-900">Company</h4>
          <ul class="space-y-3 text-sm">
            <li><a href="#blog" class="text-gray-600 hover:text-primary-600 transition-colors">Blog</a></li>
            <li><a href="#affiliate" class="text-gray-600 hover:text-primary-600 transition-colors">Affiliate Program</a></li>
            <li><a href="mailto:support@dropmagic.ai" class="text-gray-600 hover:text-primary-600 transition-colors">Support</a></li>
            <li><a href="https://tiktok.com/@dropmagic" class="text-gray-600 hover:text-primary-600 transition-colors">TikTok</a></li>
          </ul>
        </div>
      </div>

      <div class="flex flex-col md:flex-row justify-between items-center text-xs text-gray-400 gap-4 pt-8 border-t border-gray-100">
        <div class="flex gap-6">
          <span>© 2025 Dropmagic. All rights reserved.</span>
        </div>
        <div class="flex gap-6">
          <a href="#terms" class="hover:text-gray-600 transition-colors">Terms of Service</a>
          <a href="#privacy" class="hover:text-gray-600 transition-colors">Privacy Policy</a>
        </div>
      </div>
    </div>
  </footer>

  <!-- Cookie Banner -->
  {#if showCookieBanner}
    <div class="fixed bottom-6 right-6 max-w-sm bg-white border border-gray-200 shadow-xl p-6 rounded-lg z-50 text-sm text-gray-600">
      <p class="mb-4 leading-relaxed">
        We use cookies to improve your experience. See our <a href="#privacy" class="underline text-primary-600 hover:text-primary-700">Privacy Policy</a> for details.
      </p>
      <button onclick={() => showCookieBanner = false} class="bg-primary-600 text-white px-5 py-2 rounded-sm font-medium hover:bg-primary-700 transition-colors w-full">
        Accept
      </button>
    </div>
  {/if}
</div>

<style>
  :global(body) {
    font-family: 'Inter', sans-serif;
  }
  .perspective-1000 {
    perspective: 1000px;
  }
  .transform-style-3d {
    transform-style: preserve-3d;
  }
</style>

