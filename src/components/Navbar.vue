<template>
  <nav class="bg-white/5 backdrop-blur-2xl fixed w-full z-50 border-b border-white/10 shadow-2xl transition-all duration-300">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between h-20 items-center">
        <img :src="logoTran" alt="Zarrah Logo" class="h-14 w-auto object-contain" />
        <div class="hidden md:flex space-x-10">
          <a href="#home"
            class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide relative group">Home
            <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-yellow-400 to-yellow-600 group-hover:w-full transition-all duration-300"></span>
          </a>
          <a href="#services"
            class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide relative group">Services
            <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-yellow-400 to-yellow-600 group-hover:w-full transition-all duration-300"></span>
          </a>
          <a href="#about"
            class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide relative group">About
            <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-yellow-400 to-yellow-600 group-hover:w-full transition-all duration-300"></span>
          </a>
          <a href="#contact"
            class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide relative group">Contact
            <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-yellow-400 to-yellow-600 group-hover:w-full transition-all duration-300"></span>
          </a>
        </div>
        <button class="md:hidden text-white p-2 rounded-lg hover:bg-white/10 transition-all duration-300">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24"
            stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
          </svg>
        </button>
      </div>
    </div>
  </nav>
</template>

<script>
import logoTran from '@/assets/logo-tran.png'

export default {
  name: 'Navbar',
  data() {
    return {
      logoTran
    }
  }
}
</script>

<style scoped>
/* Navigation animations */
a {
  position: relative;
}
</style>
