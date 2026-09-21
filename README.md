# ProblemHunter.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ProductHunter — We Hunt The Best, So You Don't Have To</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700;800&family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" />
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            brand: {
              emerald: '#10b981',
              accent: '#059669',
              dark: '#090d16',
              card: '#0f172a',
              border: '#1e293b'
            }
          },
          fontFamily: {
            sans: ['"Plus Jakarta Sans"', 'sans-serif'],
            display: ['Outfit', 'sans-serif']
          }
        }
      }
    }
  </script>
  <style>
    body {
      background-color: #070a12;
      color: #f8fafc;
      font-family: 'Plus Jakarta Sans', sans-serif;
    }
    .custom-scrollbar::-webkit-scrollbar { width: 6px; }
    .custom-scrollbar::-webkit-scrollbar-track { background: #0b0f19; }
    .custom-scrollbar::-webkit-scrollbar-thumb { background: #1e293b; border-radius: 9999px; }
  </style>
</head>
<body class="min-h-screen flex flex-col antialiased selection:bg-emerald-500 selection:text-black">

  <!-- TOP ANNOUNCEMENT BAR -->
  <header class="bg-gradient-to-r from-emerald-950/80 via-slate-900 to-emerald-950/80 border-b border-emerald-500/20 py-2.5 px-4 text-xs font-semibold text-center text-emerald-300">
    <div class="max-w-7xl mx-auto flex items-center justify-center gap-2">
      <span class="w-2 h-2 rounded-full bg-emerald-400 animate-pulse"></span>
      <span>Official Portal — <strong>We Hunt The Best, So You Don't Have To.</strong> Enter any 6-digit video code below!</span>
    </div>
  </header>

  <!-- NAVBAR -->
  <nav class="sticky top-0 z-40 bg-[#070a12]/90 backdrop-blur-md border-b border-slate-800/80">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between gap-4">
      
      <!-- LOGO -->
      <a href="index.html" class="flex items-center gap-3">
        <div class="w-11 h-11 rounded-xl bg-gradient-to-tr from-emerald-500 to-teal-400 flex items-center justify-center shadow-lg shadow-emerald-500/20 text-black font-black text-xl font-display">
          PH
        </div>
        <div>
          <span class="text-xl font-extrabold tracking-tight font-display text-white">Product<span class="text-emerald-400">Hunter</span></span>
          <span class="hidden sm:block text-[10px] uppercase font-bold tracking-widest text-slate-400">Curated Tech & Viral Finds</span>
        </div>
      </a>

      <!-- QUICK 6-DIGIT CODE SEARCH IN HEADER -->
      <div class="relative w-full max-w-xs sm:max-w-sm">
        <i class="fa-solid fa-hashtag absolute left-3.5 top-1/2 -translate-y-1/2 text-slate-500 text-sm"></i>
        <input 
          id="headerCodeInput"
          type="text" 
          maxlength="6"
          placeholder="Paste 6-digit code..." 
          class="w-full pl-9 pr-20 py-2 rounded-lg bg-slate-900/90 border border-slate-800 text-white placeholder-slate-500 text-xs sm:text-sm font-mono focus:outline-none focus:border-emerald-500 focus:ring-1 focus:ring-emerald-500 transition"
        />
        <button id="headerCodeBtn" class="absolute right-1.5 top-1/2 -translate-y-1/2 px-2.5 py-1 rounded bg-emerald-500 hover:bg-emerald-400 text-black text-xs font-bold transition">
          Find
        </button>
      </div>

      <!-- SOCIAL CHANNELS -->
      <div class="flex items-center gap-2 sm:gap-3">
        <a href="https://www.youtube.com/@ProblemHunterGG" target="_blank" rel="noopener noreferrer" class="px-3 py-2 rounded-lg bg-red-600/10 hover:bg-red-600/20 text-red-400 border border-red-500/20 text-xs font-bold flex items-center gap-1.5 transition">
          <i class="fa-brands fa-youtube text-sm"></i>
          <span class="hidden md:inline">YouTube</span>
        </a>
        <a href="https://www.instagram.com/problemhunteroriginal?stkn=b3UxcjN4bnQ2cW9v" target="_blank" rel="noopener noreferrer" class="px-3 py-2 rounded-lg bg-pink-600/10 hover:bg-pink-600/20 text-pink-400 border border-pink-500/20 text-xs font-bold flex items-center gap-1.5 transition">
          <i class="fa-brands fa-instagram text-sm"></i>
          <span class="hidden md:inline">Instagram</span>
        </a>
      </div>
    </div>
  </nav>

  <!-- HERO & MAIN SEARCH -->
  <section class="relative pt-12 pb-8 px-4 text-center max-w-4xl mx-auto">
    <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-slate-800/80 border border-slate-700/80 text-slate-300 text-xs font-medium mb-4">
      <span class="w-1.5 h-1.5 rounded-full bg-emerald-400"></span>
      100% Tested & Handpicked Finds
    </div>
    <h1 class="text-3xl sm:text-5xl font-black font-display tracking-tight text-white mb-3">
      We Hunt The Best, <span class="text-transparent bg-clip-text bg-gradient-to-r from-emerald-400 via-teal-300 to-cyan-400">So You Don't Have To.</span>
    </h1>
    <p class="text-slate-400 text-sm sm:text-base max-w-xl mx-auto mb-8">
      Saw a product on our YouTube or Instagram? Search by keyword or enter the exact 6-digit product code to grab the deal.
    </p>

    <!-- SEARCH & FILTER BAR -->
    <div class="relative max-w-2xl mx-auto mb-6">
      <i class="fa-solid fa-magnifying-glass absolute left-4 top-1/2 -translate-y-1/2 text-slate-400 text-lg"></i>
      <input 
        id="mainSearchInput"
        type="text" 
        placeholder="Search by product name or type 6-digit code..." 
        class="w-full pl-12 pr-12 py-3.5 rounded-xl bg-slate-900 border border-slate-800 text-white placeholder-slate-500 text-sm focus:outline-none focus:border-emerald-500 focus:ring-2 focus:ring-emerald-500/20 transition shadow-xl"
      />
      <button id="clearSearchBtn" class="hidden absolute right-4 top-1/2 -translate-y-1/2 text-slate-400 hover:text-white text-sm">
        <i class="fa-solid fa-xmark"></i>
      </button>
    </div>

    <!-- CATEGORY PILLS -->
    <div id="categoryContainer" class="flex flex-wrap items-center justify-center gap-2 text-xs">
      <button class="cat-pill active px-3.5 py-1.5 rounded-lg bg-emerald-500 text-black font-bold border border-emerald-400 transition" data-cat="all">All Drops</button>
      <button class="cat-pill px-3.5 py-1.5 rounded-lg bg-slate-900 text-slate-300 font-semibold border border-slate-800 hover:border-slate-700 transition" data-cat="Tech & Gadgets">Tech & Gadgets</button>
      <button class="cat-pill px-3.5 py-1.5 rounded-lg bg-slate-900 text-slate-300 font-semibold border border-slate-800 hover:border-slate-700 transition" data-cat="Desk Setup">Desk Setup</button>
      <button class="cat-pill px-3.5 py-1.5 rounded-lg bg-slate-900 text-slate-300 font-semibold border border-slate-800 hover:border-slate-700 transition" data-cat="Lifestyle">Lifestyle</button>
    </div>
  </section>

  <!-- PRODUCT GRID / ZERO STATE -->
  <main class="flex-1 max-w-7xl mx-auto w-full px-4 sm:px-6 lg:px-8 py-6">
    <div id="productGrid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6">
      <!-- Injected via JavaScript -->
    </div>

    <!-- EMPTY CATALOG STATE (NO PRODUCTS YET) -->
    <div id="emptyCatalogState" class="hidden text-center py-20 px-4 max-w-md mx-auto">
      <div class="w-16 h-16 rounded-2xl bg-slate-900 border border-slate-800 flex items-center justify-center mx-auto mb-4 text-emerald-400 text-2xl">
        <i class="fa-solid fa-compass"></i>
      </div>
      <h3 class="text-xl font-bold font-display text-white mb-2">Curating Fresh Drops</h3>
      <p class="text-slate-400 text-sm mb-6">
        We are currently testing and vetting new viral finds for our next reel. Stay tuned on our social channels!
      </p>
      <div class="flex items-center justify-center gap-3">
        <a href="https://www.youtube.com/@ProblemHunterGG" target="_blank" class="px-4 py-2 rounded-lg bg-slate-900 border border-slate-800 hover:border-red-500/50 text-slate-300 hover:text-white text-xs font-semibold flex items-center gap-2 transition">
          <i class="fa-brands fa-youtube text-red-500"></i> Subscribe on YouTube
        </a>
        <a href="https://www.instagram.com/problemhunteroriginal?stkn=b3UxcjN4bnQ2cW9v" target="_blank" class="px-4 py-2 rounded-lg bg-slate-900 border border-slate-800 hover:border-pink-500/50 text-slate-300 hover:text-white text-xs font-semibold flex items-center gap-2 transition">
          <i class="fa-brands fa-instagram text-pink-500"></i> Follow Instagram
        </a>
      </div>
    </div>
  </main>

  <!-- PRODUCT DETAILS & AFFILIATE REDIRECT MODAL -->
  <div id="productModal" class="fixed inset-0 z-50 bg-black/80 backdrop-blur-sm hidden flex items-center justify-center p-4">
    <div class="bg-slate-900 border border-slate-800 w-full max-w-2xl rounded-2xl overflow-hidden shadow-2xl flex flex-col max-h-[90vh]">
      
      <!-- MODAL HEADER -->
      <div class="px-6 py-4 border-b border-slate-800 flex items-center justify-between bg-slate-950/60">
        <div class="flex items-center gap-2.5">
          <span class="px-2 py-0.5 rounded bg-emerald-500/20 text-emerald-400 text-xs font-mono font-bold tracking-wider" id="modalCode">#000000</span>
          <span class="text-xs text-slate-400" id="modalCategory">Category</span>
        </div>
        <button id="modalCloseBtn" class="text-slate-400 hover:text-white text-lg transition">
          <i class="fa-solid fa-xmark"></i>
        </button>
      </div>

      <!-- MODAL BODY -->
      <div class="p-6 overflow-y-auto custom-scrollbar space-y-6">
        <div class="flex flex-col sm:flex-row gap-6 items-start">
          <img id="modalImage" src="" alt="Product Image" class="w-full sm:w-56 h-56 object-cover rounded-xl border border-slate-800 bg-slate-950 flex-shrink-0" />
          <div class="flex-1 space-y-3">
            <h2 id="modalTitle" class="text-xl font-bold font-display text-white"></h2>
            <div class="flex items-baseline gap-2">
              <span id="modalPrice" class="text-2xl font-extrabold text-emerald-400"></span>
              <span id="modalOriginalPrice" class="text-sm line-through text-slate-500"></span>
            </div>
            <p id="modalDescription" class="text-sm text-slate-300 leading-relaxed"></p>
          </div>
        </div>

        <!-- HIGHLIGHTS / SPECS -->
        <div id="modalFeaturesContainer" class="bg-slate-950/60 border border-slate-800/80 p-4 rounded-xl space-y-2">
          <h4 class="text-xs font-bold uppercase tracking-wider text-slate-400">Verified Highlights</h4>
          <ul id="modalFeaturesList" class="text-xs text-slate-300 space-y-1.5 list-disc list-inside"></ul>
        </div>

        <!-- AFFILIATE CTA BUTTON -->
        <div class="pt-2">
          <a id="modalAffiliateLink" href="#" target="_blank" rel="noopener noreferrer sponsored" class="w-full py-4 rounded-xl bg-gradient-to-r from-emerald-500 to-teal-400 hover:from-emerald-400 hover:to-teal-300 text-black font-extrabold text-base flex items-center justify-center gap-2 shadow-lg shadow-emerald-500/25 transition">
            <span>GO TO STORE & CLAIM DEAL</span>
            <i class="fa-solid fa-arrow-up-right-from-square text-sm"></i>
          </a>
        </div>

        <!-- TRANSPARENCY & AFFILIATE DISCLAIMER -->
        <div class="p-4 rounded-xl bg-slate-950 border border-slate-800 text-[11px] text-slate-400 leading-relaxed">
          <div class="flex items-center gap-2 text-slate-300 font-bold mb-1.5">
            <i class="fa-solid fa-shield-halved text-emerald-400"></i>
            <span>Transparency & Affiliate Disclaimer</span>
          </div>
          <p>
            Some links in this description are affiliate links, meaning I may earn a commission if you purchase through them, at no extra cost to you. I aim to promote products that are permissible to promote. Product availability, appearance, specifications, pricing, and quality may vary, and the product shown in the video may differ from the exact product/listing received. Product descriptions, claims, quality, fulfillment, shipping, and accuracy are the responsibility of the respective Temu or any xyz platform seller/listing. Please review the listing and seller information carefully before purchasing.
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- FOOTER -->
  <footer class="border-t border-slate-800 bg-[#06080f] py-8 mt-auto">
    <div class="max-w-7xl mx-auto px-4 text-center text-xs text-slate-500 space-y-2">
      <p class="font-bold text-slate-400 font-display">ProductHunter — We Hunt The Best, So You Don't Have To.</p>
      <p>© 2026 ProductHunter. All rights reserved. Follow our channels for daily verified drops.</p>
    </div>
  </footer>

  <script>
    // STORAGE KEY FOR SHARED CATALOG
    const STORAGE_KEY = "PRODUCT_HUNTER_DATABASE";

    // Load active products from storage or fallback to empty array
    function getStoredProducts() {
      try {
        const data = localStorage.getItem(STORAGE_KEY);
        return data ? JSON.parse(data) : [];
      } catch(e) {
        return [];
      }
    }

    let products = getStoredProducts();
    let currentCategory = 'all';
    let searchQuery = '';

    const productGrid = document.getElementById('productGrid');
    const emptyState = document.getElementById('emptyCatalogState');
    const mainSearchInput = document.getElementById('mainSearchInput');
    const headerCodeInput = document.getElementById('headerCodeInput');
    const headerCodeBtn = document.getElementById('headerCodeBtn');
    const clearSearchBtn = document.getElementById('clearSearchBtn');
    const categoryButtons = document.querySelectorAll('.cat-pill');

    // Modal elements
    const productModal = document.getElementById('productModal');
    const modalCloseBtn = document.getElementById('modalCloseBtn');
    const modalCode = document.getElementById('modalCode');
    const modalCategory = document.getElementById('modalCategory');
    const modalImage = document.getElementById('modalImage');
    const modalTitle = document.getElementById('modalTitle');
    const modalPrice = document.getElementById('modalPrice');
    const modalOriginalPrice = document.getElementById('modalOriginalPrice');
    const modalDescription = document.getElementById('modalDescription');
    const modalFeaturesList = document.getElementById('modalFeaturesList');
    const modalAffiliateLink = document.getElementById('modalAffiliateLink');

    // RENDER PRODUCTS
    function render() {
      // Re-read latest products in case of updates
      products = getStoredProducts();

      const filtered = products.filter(item => {
        const matchesCategory = currentCategory === 'all' || item.category === currentCategory;
        const q = searchQuery.toLowerCase().trim();
        const matchesQuery = !q || 
          item.code.toLowerCase().includes(q) || 
          item.title.toLowerCase().includes(q) || 
          (item.description && item.description.toLowerCase().includes(q));
        return matchesCategory && matchesQuery;
      });

      productGrid.innerHTML = '';

      if (filtered.length === 0) {
        productGrid.classList.add('hidden');
        emptyState.classList.remove('hidden');
      } else {
        productGrid.classList.remove('hidden');
        emptyState.classList.add('hidden');

        filtered.forEach(p => {
          const card = document.createElement('div');
          card.className = "bg-slate-900 border border-slate-800 rounded-2xl overflow-hidden hover:border-emerald-500/50 transition duration-300 flex flex-col group cursor-pointer shadow-lg";
          card.onclick = () => openProductModal(p.code);

          card.innerHTML = `
            <div class="relative w-full h-48 bg-slate-950 overflow-hidden">
              <img src="${p.imageUrl}" alt="${p.title}" class="w-full h-full object-cover group-hover:scale-105 transition duration-500" onerror="this.src='https://images.unsplash.com/photo-1526170375885-4d8ecf77b99f?w=600&auto=format&fit=crop&q=80'" />
              <div class="absolute top-3 left-3 bg-black/80 backdrop-blur-md px-2.5 py-1 rounded-md text-[11px] font-mono font-bold text-emerald-400 border border-emerald-500/30">
                #${p.code}
              </div>
              ${p.badge ? `<div class="absolute top-3 right-3 bg-emerald-500 text-black px-2 py-0.5 rounded text-[10px] font-extrabold uppercase tracking-wide">${p.badge}</div>` : ''}
            </div>
            <div class="p-4 flex-1 flex flex-col justify-between space-y-3">
              <div>
                <span class="text-[10px] font-bold uppercase tracking-wider text-slate-400">${p.category || 'Curated'}</span>
                <h3 class="text-sm font-bold text-white line-clamp-2 mt-1 group-hover:text-emerald-300 transition">${p.title}</h3>
              </div>
              <div class="flex items-center justify-between pt-2 border-t border-slate-800/80">
                <div>
                  <span class="text-base font-extrabold text-emerald-400">${p.price}</span>
                  ${p.originalPrice ? `<span class="text-xs line-through text-slate-500 ml-1.5">${p.originalPrice}</span>` : ''}
                </div>
                <span class="text-xs font-bold text-slate-300 group-hover:text-emerald-400 flex items-center gap-1">
                  View <i class="fa-solid fa-chevron-right text-[10px]"></i>
                </span>
              </div>
            </div>
          `;
          productGrid.appendChild(card);
        });
      }
    }

    // MODAL HANDLER
    function openProductModal(code) {
      const p = products.find(i => i.code === code);
      if (!p) return;

      modalCode.textContent = `#${p.code}`;
      modalCategory.textContent = p.category || 'Curated Deal';
      modalImage.src = p.imageUrl || '';
      modalTitle.textContent = p.title;
      modalPrice.textContent = p.price;
      modalOriginalPrice.textContent = p.originalPrice || '';
      modalDescription.textContent = p.description || 'Verified product selected by ProductHunter.';
      modalAffiliateLink.href = p.affiliateUrl || '#';

      // Features
      modalFeaturesList.innerHTML = '';
      if (Array.isArray(p.features) && p.features.length > 0) {
        p.features.forEach(f => {
          const li = document.createElement('li');
          li.textContent = f;
          modalFeaturesList.appendChild(li);
        });
        document.getElementById('modalFeaturesContainer').classList.remove('hidden');
      } else {
        document.getElementById('modalFeaturesContainer').classList.add('hidden');
      }

      productModal.classList.remove('hidden');
      history.replaceState(null, '', `?code=${p.code}`);
    }

    function closeModal() {
      productModal.classList.add('hidden');
      history.replaceState(null, '', window.location.pathname);
    }

    modalCloseBtn.onclick = closeModal;
    productModal.onclick = (e) => {
      if (e.target === productModal) closeModal();
    };

    // SEARCH INPUTS
    mainSearchInput.addEventListener('input', (e) => {
      searchQuery = e.target.value;
      clearSearchBtn.classList.toggle('hidden', !searchQuery);
      
      // Auto open if exact 6-digit code matched
      if (/^\d{6}$/.test(searchQuery.trim())) {
        const found = products.find(p => p.code === searchQuery.trim());
        if (found) openProductModal(found.code);
      }
      render();
    });

    clearSearchBtn.onclick = () => {
      mainSearchInput.value = '';
      searchQuery = '';
      clearSearchBtn.classList.add('hidden');
      render();
    };

    // HEADER CODE JUMP
    function handleHeaderCode() {
      const code = headerCodeInput.value.trim();
      if (!code) return;
      const found = products.find(p => p.code === code);
      if (found) {
        openProductModal(found.code);
        headerCodeInput.value = '';
      } else {
        alert("Product with code #" + code + " not found.");
      }
    }
    headerCodeBtn.onclick = handleHeaderCode;
    headerCodeInput.onkeydown = (e) => { if (e.key === 'Enter') handleHeaderCode(); };

    // CATEGORY FILTERS
    categoryButtons.forEach(btn => {
      btn.onclick = () => {
        categoryButtons.forEach(b => {
          b.className = "cat-pill px-3.5 py-1.5 rounded-lg bg-slate-900 text-slate-300 font-semibold border border-slate-800 hover:border-slate-700 transition";
        });
        btn.className = "cat-pill active px-3.5 py-1.5 rounded-lg bg-emerald-500 text-black font-bold border border-emerald-400 transition";
        currentCategory = btn.getAttribute('data-cat');
        render();
      };
    });

    // LISTEN FOR REAL-TIME CROSS-TAB SYNC (When admin updates products in admin.html)
    window.addEventListener('storage', (e) => {
      if (e.key === STORAGE_KEY) {
        render();
      }
    });

    // CHECK URL PARAMS ON LOAD (?code=123456)
    window.addEventListener('DOMContentLoaded', () => {
      const urlParams = new URLSearchParams(window.location.search);
      const codeParam = urlParams.get('code');
      render();
      if (codeParam) {
        openProductModal(codeParam);
      }
    });
  </script>
</body>
</html>
