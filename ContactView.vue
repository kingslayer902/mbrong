<template>
    <section class="space-y-20">
      <!-- Hero -->
      <div class="text-center bg-gradient-to-r from-green-500 to-teal-500 text-white py-20 rounded-lg shadow-md">
        <h1 class="text-5xl font-bold mb-4">Hubungi Kami 📞</h1>
        <p class="text-xl">Kami senang mendengar dari Anda! Silakan isi formulir di bawah atau kirim pesan langsung.</p>
      </div>
  
      <!-- Form Kontak -->
      <div class="bg-white p-8 rounded-lg shadow max-w-3xl mx-auto">
        <form @submit.prevent="submitForm" class="space-y-6">
          <div>
            <label class="block font-semibold mb-1">Nama</label>
            <input type="text" class="w-full border border-gray-300 rounded px-4 py-2 focus:outline-none focus:ring-2 focus:ring-green-500" />
          </div>
          <div>
            <label class="block font-semibold mb-1">Email</label>
            <input type="email" class="w-full border border-gray-300 rounded px-4 py-2 focus:outline-none focus:ring-2 focus:ring-green-500" />
          </div>
          <div>
            <label class="block font-semibold mb-1">Pesan</label>
            <textarea class="w-full border border-gray-300 rounded px-4 py-2 h-32 resize-none focus:outline-none focus:ring-2 focus:ring-green-500"></textarea>
          </div>
          <button type="submit" class="bg-green-600 text-white px-6 py-2 rounded-full hover:bg-green-700 transition">
            Kirim Pesan 🚀
          </button>
        </form>
      </div>
  
      <!-- Lokasi & Sosial Media -->
      <div class="text-center space-y-6">
        <h2 class="text-2xl font-bold">📍 Lokasi Kami</h2>
        <p>Jl. Vue Developer No. 77, Bandung</p>
        <iframe
          class="mx-auto rounded shadow"
          width="100%"
          height="300"
          src="https://maps.google.com/maps?q=jakarta&output=embed"
          allowfullscreen
        ></iframe>
  
        <div class="flex justify-center space-x-4 mt-4">
          <a href="#" class="text-blue-600 hover:underline">Facebook</a>
          <a href="#" class="text-pink-500 hover:underline">Instagram</a>
          <a href="#" class="text-blue-400 hover:underline">Twitter</a>
        </div>
      </div>
  
      <!-- CTA -->
      <div class="text-center py-16">
        <h2 class="text-3xl font-bold mb-4">Ingin kembali ke halaman utama?</h2>
        <router-link to="/">
          <button class="bg-gray-700 text-white px-6 py-3 rounded-full hover:bg-gray-800 transition">
            ← Kembali ke Home
          </button>
        </router-link>
      </div>
    </section>
  </template>
  
  <script setup>
  function submitForm() {
    alert("Pesan berhasil dikirim! (ini simulasi)");
  }
  </script>
  