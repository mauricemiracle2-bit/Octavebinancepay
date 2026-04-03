<!DOCTYPE html>  
<html lang="en" class="scroll-smooth">  
<head>  
  <meta charset="UTF-8">  
  <meta name="viewport" content="width=device-width, initial-scale=1.0">  
  <title>Octave - Instant Payments</title>  
  <script src="https://cdn.tailwindcss.com"></script>  
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">  
  <style>  
    body { font-family: 'Inter', system-ui, sans-serif; }  
    .hero-bg {  
      background: linear-gradient(135deg, #0A2540 0%, #1E3A8A 100%);  
    }  
    .modal {  
      animation: fadeIn 0.3s ease;  
    }  
    @keyframes fadeIn {  
      from { opacity: 0; transform: scale(0.95); }  
      to { opacity: 1; transform: scale(1); }  
    }  
  </style>  
</head>  
<body class="bg-zinc-950 text-white">  
  
  <!-- Navbar -->  
  <nav class="fixed top-0 w-full bg-zinc-950/80 backdrop-blur-md z-50 border-b border-zinc-800">  
    <div class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">  
      <div class="flex items-center gap-3">  
        <div class="w-9 h-9 bg-indigo-600 rounded-2xl flex items-center justify-center text-2xl font-bold">♪</div>  
        <h1 class="text-2xl font-bold tracking-tight">Octave</h1>  
      </div>  
      <div class="hidden md:flex gap-8">  
        <a href="#" class="hover:text-indigo-400 transition">Services</a>  
        <a href="#" class="hover:text-indigo-400 transition">How it Works</a>  
        <a href="#" class="hover:text-indigo-400 transition">Pricing</a>  
      </div>  
      <div class="flex gap-3">  
        <button onclick="showLoginModal()" class="px-6 py-2.5 rounded-2xl border border-zinc-700 hover:border-zinc-500 transition">Login</button>  
        <button onclick="showRegisterModal()" class="px-6 py-2.5 bg-indigo-600 hover:bg-indigo-500 rounded-2xl font-semibold transition">Get Started</button>  
      </div>  
    </div>  
  </nav>  
  
  <!-- Hero -->  
  <section class="hero-bg min-h-screen pt-24 flex items-center">  
    <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-2 gap-12 items-center">  
      <div class="space-y-8">  
        <div class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-md px-4 py-2 rounded-full text-sm">  
          <div class="w-2 h-2 bg-green-400 rounded-full animate-pulse"></div>  
          Now Available in Nigeria & Ghana  
        </div>  
          
        <h1 class="text-6xl md:text-7xl font-bold leading-tight tracking-tighter">  
          Get your account ready and trade better.  
        </h1>  
          
        <p class="text-xl text-zinc-400 max-w-lg">  
          Buy & sell airtime, data, pay bills cheaper, send money instantly, and earn daily with Octave.  
        </p>  
          
        <div class="flex gap-4">  
          <button onclick="showRegisterModal()" class="px-8 py-4 bg-indigo-600 hover:bg-indigo-500 text-lg font-semibold rounded-3xl flex items-center gap-3 transition">  
            Get Started Free  
            <i class="fas fa-arrow-right"></i>  
          </button>  
          <button onclick="watchDemo()" class="px-8 py-4 border border-white/30 hover:bg-white/10 rounded-3xl flex items-center gap-3 transition">  
            <i class="fas fa-play"></i> Watch Demo  
          </button>  
        </div>  
          
        <div class="flex items-center gap-8 text-sm">  
          <div class="flex -space-x-4">  
            <div class="w-8 h-8 bg-zinc-700 rounded-full border-2 border-zinc-900 flex items-center justify-center text-xs">🇳🇬</div>  
            <div class="w-8 h-8 bg-zinc-700 rounded-full border-2 border-zinc-900 flex items-center justify-center text-xs">🇬🇭</div>  
          </div>  
          <div>Trusted by <span class="font-semibold text-green-400">50,000+</span> users</div>  
        </div>  
      </div>  
  
      <!-- Phone Mockup -->  
      <div class="relative hidden md:block">  
        <div class="bg-black rounded-[3rem] p-3 shadow-2xl mx-auto max-w-[280px] border border-zinc-700">  
          <div class="bg-zinc-900 rounded-[2.5rem] overflow-hidden h-[560px] relative">  
            <div class="absolute top-0 left-0 right-0 h-12 bg-black flex items-center justify-center">  
              <div class="w-28 h-4 bg-zinc-800 rounded-full"></div>  
            </div>  
            <div class="pt-14 px-6 text-center">  
              <div class="text-indigo-400 text-3xl font-bold mb-2">₦12,450</div>  
              <div class="text-sm text-zinc-400">Available Balance</div>  
              <div class="mt-8 space-y-4">  
                <button class="w-full py-4 bg-indigo-600 rounded-2xl font-medium">Buy Airtime & Data</button>  
                <button class="w-full py-4 bg-zinc-800 rounded-2xl font-medium">Send Money</button>  
                <button class="w-full py-4 bg-zinc-800 rounded-2xl font-medium">Pay Bills</button>  
              </div>  
            </div>  
          </div>  
        </div>  
      </div>  
    </div>  
  </section>  
  
  <!-- Features -->  
  <section class="py-20 bg-zinc-900">  
    <div class="max-w-7xl mx-auto px-6">  
      <h2 class="text-4xl font-bold text-center mb-12">Everything you need in one app</h2>  
      <div class="grid md:grid-cols-3 gap-6">  
        <div class="bg-zinc-800/50 p-8 rounded-3xl card-hover">  
          <i class="fas fa-mobile-alt text-4xl text-indigo-400 mb-6"></i>  
          <h3 class="text-2xl font-semibold mb-3">Airtime & Data</h3>  
          <p class="text-zinc-400">Cheapest rates for all networks. Instant delivery.</p>  
        </div>  
        <div class="bg-zinc-800/50 p-8 rounded-3xl card-hover">  
          <i class="fas fa-exchange-alt text-4xl text-indigo-400 mb-6"></i>  
          <h3 class="text-2xl font-semibold mb-3">Instant Transfers</h3>  
          <p class="text-zinc-400">Send money to any bank account in seconds.</p>  
        </div>  
        <div class="bg-zinc-800/50 p-8 rounded-3xl card-hover">  
          <i class="fas fa-receipt text-4xl text-indigo-400 mb-6"></i>  
          <h3 class="text-2xl font-semibold mb-3">Bill Payments</h3>  
          <p class="text-zinc-400">Electricity, Cable, Internet at discounted rates.</p>  
        </div>  
      </div>  
    </div>  
  </section>  
  
  <!-- CTA -->  
  <section class="py-20 bg-gradient-to-b from-transparent via-indigo-950 to-transparent text-center">  
    <div class="max-w-lg mx-auto px-6">  
      <h2 class="text-5xl font-bold mb-6">Ready to start earning?</h2>  
      <button onclick="showRegisterModal()" class="w-full md:w-auto px-12 py-5 text-xl bg-white text-black font-semibold rounded-3xl hover:scale-105 transition">  
        Create Free Account →  
      </button>  
    </div>  
  </section>  
  
  <!-- Login & Register Modals (same beautiful ones) -->  
  <div id="loginModal" class="hidden fixed inset-0 bg-black/70 flex items-center justify-center z-[100]">  
    <div class="modal bg-zinc-900 w-full max-w-md mx-4 rounded-3xl p-8">  
      <div class="flex justify-between items-center mb-6">  
        <h2 class="text-3xl font-bold">Welcome back</h2>  
        <button onclick="hideLoginModal()" class="text-3xl text-zinc-400 hover:text-white">×</button>  
      </div>  
      <input type="text" placeholder="Phone number or Email" class="w-full bg-zinc-800 border border-zinc-700 rounded-2xl px-5 py-4 mb-4 focus:outline-none focus:border-indigo-500">  
      <input type="password" placeholder="Password" class="w-full bg-zinc-800 border border-zinc-700 rounded-2xl px-5 py-4 mb-6 focus:outline-none focus:border-indigo-500">  
      <button onclick="fakeLogin()" class="w-full py-4 bg-indigo-600 hover:bg-indigo-500 rounded-2xl font-semibold text-lg">Login</button>  
      <div class="text-center mt-8 text-zinc-400">  
        Don't have an account?   
        <button onclick="switchToRegister()" class="text-indigo-400 hover:underline">Sign up</button>  
      </div>  
    </div>  
  </div>  
  
  <div id="registerModal" class="hidden fixed inset-0 bg-black/70 flex items-center justify-center z-[100]">  
    <div class="modal bg-zinc-900 w-full max-w-md mx-4 rounded-3xl p-8">  
      <div class="flex justify-between items-center mb-6">  
        <h2 class="text-3xl font-bold">Create Account</h2>  
        <button onclick="hideRegisterModal()" class="text-3xl text-zinc-400 hover:text-white">×</button>  
      </div>  
      <input type="text" placeholder="Full Name" class="w-full bg-zinc-800 border border-zinc-700 rounded-2xl px-5 py-4 mb-4">  
      <input type="tel" placeholder="Phone Number" class="w-full bg-zinc-800 border border-zinc-700 rounded-2xl px-5 py-4 mb-4">  
      <input type="email" placeholder="Email (optional)" class="w-full bg-zinc-800 border border-zinc-700 rounded-2xl px-5 py-4 mb-6">  
      <input type="password" placeholder="Create Password" class="w-full bg-zinc-800 border border-zinc-700 rounded-2xl px-5 py-4 mb-4">  
      <button onclick="fakeRegister()" class="w-full py-4 bg-indigo-600 hover:bg-indigo-500 rounded-2xl font-semibold text-lg">Create Free Account</button>  
      <div class="text-center mt-8 text-zinc-400">  
        Already have an account?   
        <button onclick="switchToLogin()" class="text-indigo-400 hover:underline">Login</button>  
      </div>  
    </div>  
  </div>  
  
  <script>  
    function showLoginModal() { document.getElementById('loginModal').classList.remove('hidden'); }  
    function hideLoginModal() { document.getElementById('loginModal').classList.add('hidden'); }  
    function showRegisterModal() { document.getElementById('registerModal').classList.remove('hidden'); }  
    function hideRegisterModal() { document.getElementById('registerModal').classList.add('hidden'); }  
    function switchToRegister() { hideLoginModal(); setTimeout(showRegisterModal, 300); }  
    function switchToLogin() { hideRegisterModal(); setTimeout(showLoginModal, 300); }  
    function fakeLogin() { alert("🎉 Logged in successfully!"); hideLoginModal(); }  
    function fakeRegister() { alert("🎉 Account created successfully! Welcome to Octave."); hideRegisterModal(); }  
    function watchDemo() { alert("🎥 Demo video would play here"); }  
  
    // Close modals when clicking outside  
    document.getElementById('loginModal').addEventListener('click', e => { if (e.target === this) hideLoginModal(); });  
    document.getElementById('registerModal').addEventListener('click', e => { if (e.target === this) hideRegisterModal(); });  
  </script>  
</body>  
</html>  
