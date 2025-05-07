<template>
  <section class="space-y-20">
    <!-- Hero Section -->
    <div class="text-center bg-gradient-to-r from-indigo-500 to-blue-600 text-white py-20 rounded-lg shadow-md">
      <h1 class="text-5xl font-bold mb-4">Selamat Datang di MyMbrongSite</h1>
      <p class="text-xl">Belajar membangun aplikasi modern dengan MyMbrong</p>
      <router-link to="/about">
        <button class="mt-6 bg-white text-blue-600 font-semibold px-6 py-2 rounded-full hover:bg-gray-200 transition duration-300">
          Tentang Kami ->
        </button>
      </router-link>
    </div>

    <!-- Fitur -->
    <div class="grid md:grid-cols-3 gap-6">
      <div class="bg-white p-6 rounded-lg shadow text-center">
        <h3 class="text-2xl font-bold mb-2">⚡ Cepat</h3>
        <p>Aplikasi dibangun dengan Vite untuk performa maksimal.</p>
      </div>
      <div class="bg-white p-6 rounded-lg shadow text-center">
        <h3 class="text-2xl font-bold mb-2">🎨 Stylish</h3>
        <p>Gunakan Mbrong App Untuk Belajar Membuat wbesite yang Rapih dan Modern.</p>
      </div>
      <div class="bg-white p-6 rounded-lg shadow text-center">
        <h3 class="text-2xl font-bold mb-2">🧩 Modular</h3>
        <p>Kembangkan Diri Dengan Belajar Langsung dari Mbrong App.</p>
      </div>
    </div>

    <!-- Testimoni -->
    <div class="bg-gray-100 p-10 rounded-lg">
      <h2 class="text-3xl font-bold text-center mb-8">Apa Kata Mereka 💬</h2>
      <div class="grid md:grid-cols-2 gap-6">
        <div class="bg-white p-6 rounded shadow">
          <p class="mb-4 italic">"Mbrong membuat saya semangat belajar Frontend"</p>
          <p class="text-right font-semibold">– Ana, Pelajar</p>
        </div>
        <div class="bg-white p-6 rounded shadow">
          <p class="mb-4 italic">"Struktur halamannya mudah diatur dan tampilannya langsung keren."</p>
          <p class="text-right font-semibold">– Budi, Developer Pemula</p>
        </div>
      </div>
    </div>

    <!-- Call To Action -->
    <div class="text-center py-16">
      <h2 class="text-3xl font-bold mb-4">Siap untuk belajar lebih dalam?</h2>
      <router-link to="/about">
        <button class="bg-blue-600 text-white px-6 py-3 rounded-full hover:bg-blue-700 transition">
          Mulai Sekarang 🚀
        </button>
      </router-link>
    </div>
  </section>
</template>
