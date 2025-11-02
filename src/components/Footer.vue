<template>
  <footer class="bg-white/5 backdrop-blur-xl py-10 border-t border-white/10 relative z-10">
    <div
      class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row items-center justify-between space-y-4 md:space-y-0">
      <img :src="logoTran" alt="Zarrah Logo" class="h-12 w-auto object-contain" />
      <p class="text-white/70 text-sm font-medium">&copy; 2025 Zarrah. All rights reserved.</p>
      <div class="flex space-x-6">
        <social-icon name="Facebook" />
        <social-icon name="Instagram" />
        <social-icon name="Twitter" />
      </div>
    </div>
  </footer>
</template>

<script>
import logoTran from '@/assets/logo-tran.png'

export default {
  name: 'Footer',
  data() {
    return {
      logoTran
    }
  }
}
</script>
