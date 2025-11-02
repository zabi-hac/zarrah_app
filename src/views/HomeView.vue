<template>
  <div class="min-h-screen bg-gradient-to-br from-black via-gray-950 to-black text-white" style="font-family: 'Segoe UI', 'Helvetica Neue', system-ui, -apple-system, sans-serif;">
    <!-- Animated background gradient -->
    <div class="fixed inset-0 -z-10 overflow-hidden">
      <div
        class="absolute top-0 right-0 w-[600px] h-[600px] bg-gradient-to-br from-yellow-500/30 to-yellow-600/20 rounded-full blur-3xl animate-pulse">
      </div>
      <div
        class="absolute bottom-0 left-0 w-[600px] h-[600px] bg-gradient-to-tr from-yellow-600/30 to-yellow-700/20 rounded-full blur-3xl animate-pulse" style="animation-delay: 1s;">
      </div>
      <div
        class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[400px] h-[400px] bg-gradient-to-r from-yellow-500/10 to-yellow-600/10 rounded-full blur-3xl">
      </div>
    </div>
    <!-- Navigation -->
    <nav class="bg-white/5 backdrop-blur-2xl fixed w-full z-50 border-b border-white/10 shadow-2xl transition-all duration-300">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex justify-between h-20 items-center">
          <img :src="logoTran" alt="Zarrah Logo" class="h-14 w-auto object-contain" />
          <div class="hidden md:flex space-x-10">
            <a href="#home"
              class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide">Home</a>
            <a href="#services"
              class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide">Services</a>
            <a href="#about"
              class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide">About</a>
            <a href="#contact"
              class="text-white/80 hover:text-yellow-400 transition-all duration-300 font-semibold text-sm uppercase tracking-wide">Contact</a>
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
    <!-- Hero Section -->
    <section id="home" class="pt-40 pb-24 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto relative z-10">
      <div class="text-center">
        <div class="mb-10 animate-fade-in">
          <img :src="logoTran" alt="Zarrah Logo" class="h-32 md:h-48 w-auto mx-auto object-contain drop-shadow-2xl hover:scale-105 transition-transform duration-500" />
        </div>
        <h1 class="text-6xl md:text-8xl font-semibold mb-8 tracking-tight leading-tight animate-fade-in-up" style="letter-spacing: -0.02em; animation-delay: 0.2s;">
          <span
            class="bg-gradient-to-r from-yellow-200 via-yellow-400 to-yellow-200 bg-clip-text text-transparent inline-block hover:scale-105 transition-transform duration-300">Premium
            Stitching</span>
          <br />
          <span class="bg-gradient-to-r from-yellow-300 via-yellow-500 to-yellow-300 bg-clip-text text-transparent inline-block hover:scale-105 transition-transform duration-300">at
            Your Doorstep</span>
        </h1>
        <p class="text-lg md:text-xl text-white/80 mb-12 max-w-3xl mx-auto leading-relaxed animate-fade-in-up" style="font-weight: 300; letter-spacing: 0.5px; animation-delay: 0.4s;">We bring
          imported fabrics to your home, take precise measurements, create stunning custom designs, and deliver tailored
          perfection.</p>
        <div class="flex justify-center flex-wrap gap-5 animate-fade-in-up" style="animation-delay: 0.6s;">
          <a href="#services"
            class="group relative bg-gradient-to-r from-yellow-400 to-yellow-600 hover:from-yellow-300 hover:to-yellow-500 text-black font-semibold py-4 px-12 rounded-full shadow-2xl hover:shadow-yellow-500/60 transform hover:-translate-y-2 hover:scale-105 transition-all duration-300 overflow-hidden">
            <span class="relative z-10">Our Services</span>
            <div class="absolute inset-0 bg-gradient-to-r from-yellow-300 to-yellow-500 opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
          </a>
          <a href="#contact"
            class="group relative bg-white/10 hover:bg-white/20 border-2 border-white/30 hover:border-yellow-400/50 text-white font-semibold py-4 px-12 rounded-full shadow-lg backdrop-blur-md transform hover:-translate-y-2 hover:scale-105 transition-all duration-300">Book
            a Consultation</a>
        </div>
      </div>
    </section>
    <!-- Services Section -->
    <section id="services" class="py-24 bg-gradient-to-b from-transparent via-gray-950/30 to-transparent relative z-10">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <h2 class="text-5xl md:text-6xl font-semibold text-center mb-20 tracking-tight" style="letter-spacing: -0.02em;">
          <span class="bg-gradient-to-r from-yellow-200 via-yellow-400 to-yellow-200 bg-clip-text text-transparent">Our Complete
            Service Process</span>
        </h2>
        <div class="grid md:grid-cols-3 gap-8">
          <div class="group relative">
            <div
              class="absolute inset-0 bg-gradient-to-r from-yellow-500/20 to-yellow-600/20 rounded-3xl blur-xl opacity-0 group-hover:opacity-100 transition-all duration-500">
            </div>
            <div
              class="relative bg-white/10 backdrop-blur-xl p-8 rounded-3xl border border-white/20 hover:border-white/40 transition-all duration-300 shadow-2xl group-hover:shadow-yellow-500/20 transform group-hover:-translate-y-2">
              <div class="text-yellow-400 mb-6 group-hover:text-yellow-300 transition-all duration-300 transform group-hover:scale-110">
                <UserIcon class="h-16 w-16 mx-auto" />
              </div>
              <h3 class="text-2xl font-medium text-white mb-4 text-center group-hover:text-yellow-300 transition-colors duration-300" style="letter-spacing: 0.5px;">Home Visit & Measurement</h3>
              <p class="text-white/70 leading-relaxed text-center" style="font-size: 0.95rem; font-weight: 300; letter-spacing: 0.3px;">We visit your home or preferred location
                to take precise measurements and understand your style preferences for the perfect fit.</p>
            </div>
          </div>
          <div class="group relative">
            <div
              class="absolute inset-0 bg-gradient-to-r from-yellow-500/20 to-yellow-600/20 rounded-3xl blur-xl opacity-0 group-hover:opacity-100 transition-all duration-500">
            </div>
            <div
              class="relative bg-white/10 backdrop-blur-xl p-8 rounded-3xl border border-white/20 hover:border-white/40 transition-all duration-300 shadow-2xl group-hover:shadow-yellow-500/20 transform group-hover:-translate-y-2">
              <div class="text-yellow-400 mb-6 group-hover:text-yellow-300 transition-all duration-300 transform group-hover:scale-110">
                <PencilSquareIcon class="h-16 w-16 mx-auto" />
              </div>
              <h3 class="text-2xl font-medium text-white mb-4 text-center group-hover:text-yellow-300 transition-colors duration-300" style="letter-spacing: 0.5px;">Premium Fabric Selection</h3>
              <p class="text-white/70 leading-relaxed text-center" style="font-size: 0.95rem; font-weight: 300; letter-spacing: 0.3px;">Choose from our curated collection of
                imported fabrics and work with our designers to create your unique custom design.</p>
            </div>
          </div>
          <div class="group relative">
            <div
              class="absolute inset-0 bg-gradient-to-r from-yellow-500/20 to-yellow-600/20 rounded-3xl blur-xl opacity-0 group-hover:opacity-100 transition-all duration-500">
            </div>
            <div
              class="relative bg-white/10 backdrop-blur-xl p-8 rounded-3xl border border-white/20 hover:border-white/40 transition-all duration-300 shadow-2xl group-hover:shadow-yellow-500/20 transform group-hover:-translate-y-2">
              <div class="text-yellow-400 mb-6 group-hover:text-yellow-300 transition-all duration-300 transform group-hover:scale-110">
                <GlobeAltIcon class="h-16 w-16 mx-auto" />
              </div>
              <h3 class="text-2xl font-medium text-white mb-4 text-center group-hover:text-yellow-300 transition-colors duration-300" style="letter-spacing: 0.5px;">Expert Stitching & Delivery</h3>
              <p class="text-white/70 leading-relaxed text-center" style="font-size: 0.95rem; font-weight: 300; letter-spacing: 0.3px;">Our master tailors craft your garment with
                precision, then deliver it directly to your doorstep with care and excellence.</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- About Section -->
    <section id="about" class="py-24 relative z-10">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="md:flex items-center gap-12">
          <div class="md:w-1/2 mb-10 md:mb-0">
            <h2 class="text-5xl md:text-6xl font-semibold mb-8 tracking-tight" style="letter-spacing: -0.02em;">
              <span class="bg-gradient-to-r from-yellow-200 via-yellow-400 to-yellow-200 bg-clip-text text-transparent">Your
                Style,</span>
              <br />
              <span class="bg-gradient-to-r from-yellow-300 via-yellow-500 to-yellow-300 bg-clip-text text-transparent">Our
                Expertise</span>
            </h2>
            <p class="text-white/70 mb-6 leading-relaxed text-base" style="font-weight: 300; letter-spacing: 0.3px;">At Zarrah, we revolutionize tailoring by
              bringing premium imported fabrics and expert craftsmanship directly to your doorstep. We understand that
              perfect fit and stunning design require personal attention and precision.</p>
            <p class="text-white/70 mb-8 leading-relaxed text-base" style="font-weight: 300; letter-spacing: 0.3px;">From the moment we visit your home to take
              measurements, through selecting the finest imported fabrics, to the final delivery of your custom-stitched
              masterpiece—we ensure every step reflects our commitment to excellence and your unique style.</p>
            <a href="#contact"
              class="inline-block bg-gradient-to-r from-yellow-400 to-yellow-600 hover:from-yellow-300 hover:to-yellow-500 text-black font-semibold py-4 px-12 rounded-full shadow-2xl hover:shadow-yellow-500/60 transform hover:-translate-y-2 hover:scale-105 transition-all duration-300">Book
              Your Appointment</a>
          </div>
          <div class="md:w-1/2">
            <div class="group relative">
              <div
                class="absolute inset-0 bg-gradient-to-r from-yellow-500/30 to-yellow-600/30 rounded-3xl blur-3xl opacity-0 group-hover:opacity-100 transition-all duration-700">
              </div>
              <div
                class="relative bg-gradient-to-br from-white/10 to-white/5 backdrop-blur-2xl border border-white/20 hover:border-yellow-400/40 rounded-3xl p-8 shadow-2xl group-hover:shadow-yellow-500/40 transition-all duration-500 transform group-hover:scale-105">
                <div
                  class="aspect-w-16 aspect-h-9 bg-gradient-to-br from-yellow-600/30 to-yellow-700/30 rounded-2xl overflow-hidden flex items-center justify-center h-96">
                  <span class="text-white/60 text-lg font-semibold">Tailoring Workspace</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Contact Section -->
    <section id="contact" class="py-24 bg-gradient-to-b from-transparent via-gray-950/30 to-transparent relative z-10">
      <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
        <h2 class="text-5xl md:text-6xl font-semibold text-center mb-16 tracking-tight" style="letter-spacing: -0.02em;">
          <span class="bg-gradient-to-r from-yellow-200 via-yellow-400 to-yellow-200 bg-clip-text text-transparent">Get In Touch</span>
        </h2>
        <div class="bg-gradient-to-br from-white/10 to-white/5 backdrop-blur-2xl border border-white/20 hover:border-yellow-400/30 rounded-3xl p-10 shadow-2xl transition-all duration-500">
          <form class="space-y-6">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
              <input-field label="Name" id="name" placeholder="Your name" />
              <input-field label="Email" id="email" placeholder="your.email@example.com" type="email" />
            </div>
            <select-field label="Service" id="service"
              :options="['Custom Stitching', 'Alterations', 'Design Consultation', 'Other']" />
            <textarea-field label="Message" id="message" placeholder="Tell us about your project..." rows="4" />
            <div class="text-center">
              <button type="submit"
                class="bg-gradient-to-r from-yellow-400 to-yellow-600 hover:from-yellow-300 hover:to-yellow-500 text-black font-semibold py-4 px-12 rounded-full shadow-2xl hover:shadow-yellow-500/60 transform hover:-translate-y-2 hover:scale-105 transition-all duration-300">Send
                Message</button>
            </div>
          </form>
          <!-- Contact Info -->
          <div class="mt-12 pt-8 border-t border-white/20">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
              <contact-card icon="MapPinIcon" title="Visit Us" info="123 Tailor Street<br>Fashion District" />
              <contact-card icon="EnvelopeIcon" title="Email Us" info="info@zarrah.com<br>bookings@zarrah.com" />
              <contact-card icon="PhoneIcon" title="Call Us" info="+1 (555) 123-4567<br>+1 (555) 987-6543" />
            </div>
          </div>
        </div>
      </div>
    </section>
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
import { UserIcon, PencilSquareIcon, GlobeAltIcon, MapPinIcon, EnvelopeIcon, PhoneIcon } from '@heroicons/vue/24/outline'
import logoTran from '@/assets/logo-tran.png'

export default {
  name: 'HomeView',
  data() {
    return {
      logoTran
    }
  },
  components: {
    UserIcon,
    PencilSquareIcon,
    GlobeAltIcon,
    MapPinIcon,
    EnvelopeIcon,
    PhoneIcon
  }
}
</script>
<style>
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

/* Custom Animations */
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

.animate-fade-in {
  animation: fade-in 1s ease-out forwards;
}

.animate-fade-in-up {
  animation: fade-in-up 1s ease-out forwards;
  opacity: 0;
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
