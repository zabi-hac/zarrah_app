<template>
   <div class="min-h-screen bg-gradient-to-br from-black via-gray-950 to-black text-white"
      style="font-family: 'Segoe UI', 'Helvetica Neue', system-ui, -apple-system, sans-serif;">
      <!-- Animated background gradient -->
      <div class="fixed inset-0 -z-10 overflow-hidden">
         <div
            class="absolute top-0 right-0 w-[600px] h-[600px] bg-gradient-to-br from-yellow-500/30 to-yellow-600/20 rounded-full blur-3xl animate-pulse animate-float"
            style="animation-duration: 6s;">
         </div>
         <div
            class="absolute bottom-0 left-0 w-[600px] h-[600px] bg-gradient-to-tr from-yellow-600/30 to-yellow-700/20 rounded-full blur-3xl animate-pulse"
            style="animation-delay: 1s;">
         </div>
         <div
            class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[400px] h-[400px] bg-gradient-to-r from-yellow-500/10 to-yellow-600/10 rounded-full blur-3xl animate-float"
            style="animation-delay: 0.5s; animation-duration: 8s;">
         </div>
      </div>
      <!-- Navigation -->
      <nav
         class="bg-white/5 backdrop-blur-2xl fixed w-full z-50 border-b border-white/10 shadow-2xl transition-all duration-300">
         <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-20 items-center">
               <img :src="logoTran" alt="Zarrah Logo" class="h-14 w-auto object-contain" />
               <div class="hidden md:flex space-x-10">
                  <a href="#home"
                     class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide relative group">Home
                     <span
                        class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-yellow-400 to-yellow-600 group-hover:w-full transition-all duration-300"></span>
                  </a>
                  <a href="#services"
                     class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide relative group">Services
                     <span
                        class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-yellow-400 to-yellow-600 group-hover:w-full transition-all duration-300"></span>
                  </a>
                  <a href="#about"
                     class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide relative group">About
                     <span
                        class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-yellow-400 to-yellow-600 group-hover:w-full transition-all duration-300"></span>
                  </a>
                  <a href="#contact"
                     class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide relative group">Contact
                     <span
                        class="absolute bottom-0 left-0 w-0 h-0.5 bg-gradient-to-r from-yellow-400 to-yellow-600 group-hover:w-full transition-all duration-300"></span>
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
      <!-- Main Content -->
      <main class="relative z-10">
         <slot></slot>
      </main>
      <!-- Footer -->
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
   </div>
</template>
<script>
import logoTran from '@/assets/logo-tran.png'

export default {
   name: 'DefaultLayout',
   data() {
      return {
         logoTran
      }
   }
}
</script>
<style scoped>
/* Scrollbar */
::-webkit-scrollbar {
   width: 10px;
}

::-webkit-scrollbar-track {
   background: #0a0a0a;
}

::-webkit-scrollbar-thumb {
   background: linear-gradient(180deg, #fbbf24, #d97706);
   border-radius: 10px;
   border: 2px solid #0a0a0a;
}

::-webkit-scrollbar-thumb:hover {
   background: linear-gradient(180deg, #fcd34d, #f59e0b);
}

/* Smooth scroll */
html {
   scroll-behavior: smooth;
}

/* Selection color */
::selection {
   background-color: #fbbf24;
   color: #000;
}

::-moz-selection {
   background-color: #fbbf24;
   color: #000;
}
</style>
<style>
/* Ghostrider Glow Effect */
@keyframes ghostrider-glow {
  0%, 100% {
    filter: drop-shadow(0 0 10px rgba(251, 191, 36, 0.4)) drop-shadow(0 0 20px rgba(251, 191, 36, 0.2));
    text-shadow: 0 0 10px rgba(251, 191, 36, 0.3);
  }
  50% {
    filter: drop-shadow(0 0 25px rgba(251, 191, 36, 0.8)) drop-shadow(0 0 40px rgba(251, 191, 36, 0.5)) drop-shadow(0 0 60px rgba(251, 191, 36, 0.3));
    text-shadow: 0 0 20px rgba(251, 191, 36, 0.6);
  }
}

.animate-ghostrider-glow {
  animation: ghostrider-glow 2s ease-in-out infinite;
}

/* Global Animations */
@keyframes fade-in {
   from {
      opacity: 0;
   }

   to {
      opacity: 1;
   }
}

@keyframes fade-in-up {
   from {
      opacity: 0;
      transform: translateY(30px);
   }

   to {
      opacity: 1;
      transform: translateY(0);
   }
}

@keyframes float {

   0%,
   100% {
      transform: translateY(0px);
   }

   50% {
      transform: translateY(-15px);
   }
}

@keyframes gradient-shift {

   0%,
   100% {
      background-position: 0% 50%;
   }

   50% {
      background-position: 100% 50%;
   }
}

@keyframes pulse-glow {

   0%,
   100% {
      box-shadow: 0 0 20px rgba(251, 191, 36, 0.3);
   }

   50% {
      box-shadow: 0 0 40px rgba(251, 191, 36, 0.6);
   }
}

@keyframes slide-in-left {
   from {
      opacity: 0;
      transform: translateX(-50px);
   }

   to {
      opacity: 1;
      transform: translateX(0);
   }
}

@keyframes slide-in-right {
   from {
      opacity: 0;
      transform: translateX(50px);
   }

   to {
      opacity: 1;
      transform: translateX(0);
   }
}

.animate-fade-in {
   animation: fade-in 1s ease-out forwards;
}

.animate-fade-in-up {
   animation: fade-in-up 1s ease-out forwards;
   opacity: 0;
}

.animate-float {
   animation: float 3s ease-in-out infinite;
}

.animate-gradient-shift {
   animation: gradient-shift 4s ease-in-out infinite;
   background-size: 200% 200%;
}

.animate-pulse-glow {
   animation: pulse-glow 2s ease-in-out infinite;
}

.animate-slide-in-left {
   animation: slide-in-left 0.8s ease-out forwards;
   opacity: 0;
}

.animate-slide-in-right {
   animation: slide-in-right 0.8s ease-out forwards;
   opacity: 0;
}
</style>
