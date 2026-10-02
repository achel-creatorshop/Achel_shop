  <!-- Search Bar -->
  <div class="relative w-full md:w-1/2">
    <input type="text" id="search-input" onkeyup="filterProducts()" placeholder="Shakisha mudasobwa, telephone, headphones..." class="w-full pl-10 pr-4 py-2 rounded-lg text-gray-900 bg-white focus:outline-none focus:ring-2 focus:ring-blue-500">
    <i class="fa-solid fa-magnifying-glass absolute left-3 top-3 text-gray-400"></i>
  </div>

  <!-- Cart Desktop Button -->
  <button onclick="toggleCart()" class="hidden md:flex items-center gap-2 bg-blue-600 hover:bg-blue-700 px-4 py-2 rounded-lg font-medium transition">
    <i class="fa-solid fa-cart-shopping"></i>
    <span>Icyangombwa</span>
    <span id="cart-count" class="bg-white text-blue-600 font-bold text-xs px-2 py-0.5 rounded-full">0</span>
  </button>
</div>


<!-- Category Filter -->
<div class="flex flex-wrap justify-center gap-2 mb-8">
  <button onclick="filterCategory(this, 'All')" class="cat-btn active bg-blue-600 text-white px-4 py-2 rounded-full font-medium text-sm transition hover:bg-blue-700">Byose</button>
  <button onclick="filterCategory(this, 'Laptops')" class="cat-btn bg-white text-gray-700 hover:bg-gray-100 border px-4 py-2 rounded-full font-medium text-sm transition">Mudasobwa (Laptops)</button>
  <button onclick="filterCategory(this, 'Phones')" class="cat-btn bg-white text-gray-700 hover:bg-gray-100 border px-4 py-2 rounded-full font-medium text-sm transition">Telefone (Smartphones)</button>
  <button onclick="filterCategory(this, 'Audio')" class="cat-btn bg-white text-gray-700 hover:bg-gray-100 border px-4 py-2 rounded-full font-medium text-sm transition">Audio & Headphones</button>
  <button onclick="filterCategory(this, 'Wearables')" class="cat-btn bg-white text-gray-700 hover:bg-gray-100 border px-4 py-2 rounded-full font-medium text-sm transition">Smartwatches</button>
</div>

<!-- Products Grid -->
<div id="product-grid" class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
  <!-- Dynamically generated via JS -->
</div>


<div id="cart-items" class="p-4 flex-grow overflow-y-auto space-y-4">
  <p class="text-gray-500 text-center py-8">Nta kintu kirazamo.</p>
</div>

<div class="p-4 border-t bg-gray-50">
  <div class="flex justify-between items-center text-lg font-bold mb-4">
    <span>Ayo Kwishyura:</span>
    <span id="cart-total" class="text-blue-600">0 RWF</span>
  </div>
  <button onclick="checkout()" class="w-full bg-green-600 hover:bg-green-700 text-white font-bold py-3 rounded-lg shadow transition">
    Emeza no Kwishyura
  </button>
</div>
