<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SignAble AI – Communication Without Barriers</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
            mono: ['JetBrains Mono', 'monospace'],
          },
          colors: {
            slateDark: '#090d16',
            panelDark: '#111827',
            accentCyan: '#06b6d4',
            accentEmerald: '#10b981',
          }
        }
      }
    }
  </script>
  <style>
    body {
      background-color: #090d16;
      color: #f8fafc;
    }
    .grid-bg {
      background-image: radial-gradient(rgba(6, 182, 212, 0.15) 1px, transparent 1px);
      background-size: 28px 28px;
    }
    @keyframes pulse-ring {
      0% { transform: scale(0.95); opacity: 0.7; }
      70% { transform: scale(1.15); opacity: 0; }
      100% { transform: scale(0.95); opacity: 0; }
    }
    .animate-pulse-ring {
      animation: pulse-ring 2s infinite;
    }
    @keyframes wave {
      0%, 100% { height: 6px; }
      50% { height: 22px; }
    }
    .wave-bar {
      animation: wave 0.9s ease-in-out infinite;
    }
    .wave-bar:nth-child(2) { animation-delay: 0.15s; }
    .wave-bar:nth-child(3) { animation-delay: 0.3s; }
    .wave-bar:nth-child(4) { animation-delay: 0.45s; }
    .wave-bar:nth-child(5) { animation-delay: 0.6s; }
  </style>
</head>
<body class="antialiased selection:bg-cyan-500 selection:text-slate-950">

  <!-- Navbar -->
  <header class="sticky top-0 z-50 backdrop-blur-md bg-slate-950/80 border-b border-slate-800/80">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
      <div class="flex items-center gap-3">
        <div class="w-9 h-9 rounded-lg bg-gradient-to-br from-cyan-400 to-emerald-500 flex items-center justify-center text-slate-950 font-extrabold text-lg shadow-lg shadow-cyan-500/20">
          SA
        </div>
        <div>
          <span class="font-bold text-lg tracking-tight text-white">SignAble <span class="text-cyan-400">AI</span></span>
          <span class="hidden sm:inline-block ml-2 text-xs font-mono px-2 py-0.5 rounded bg-cyan-500/10 text-cyan-300 border border-cyan-500/20">
            Computer Vision
          </span>
        </div>
      </div>
      <nav class="hidden md:flex items-center gap-7 text-sm font-medium text-slate-300">
        <a href="#problem-solution" class="hover:text-cyan-400 transition">Problem & Solution</a>
        <a href="#live-demo" class="hover:text-cyan-400 transition">Interactive Prototype</a>
        <a href="#architecture" class="hover:text-cyan-400 transition">How It Works</a>
        <a href="#tech-stack" class="hover:text-cyan-400 transition">Tech Stack</a>
      </nav>
      <a href="#live-demo" class="px-4 py-2 rounded-lg bg-cyan-500 hover:bg-cyan-400 text-slate-950 font-semibold text-sm transition shadow-md shadow-cyan-500/20">
        Launch Prototype
      </a>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="relative overflow-hidden grid-bg pt-16 pb-20 lg:pt-24 lg:pb-28 border-b border-slate-800/80">
    <div class="absolute -top-24 left-1/2 -translate-x-1/2 w-[650px] h-[320px] bg-cyan-500/15 blur-[120px] rounded-full pointer-events-none"></div>
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 text-center">
      <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-slate-900/90 border border-slate-700/80 text-xs font-mono text-cyan-300 mb-6">
        <span class="w-2 h-2 rounded-full bg-emerald-400 animate-ping"></span>
        DOMAIN: COMPUTER VISION • ACCESSIBILITY AI
      </div>
      <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight text-white max-w-4xl mx-auto leading-tight">
        SignAble AI – <span class="text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 via-teal-300 to-emerald-400">Communication Without Barriers</span>
      </h1>
      <p class="mt-6 text-lg sm:text-xl text-slate-300 max-w-2xl mx-auto leading-relaxed">
        Real-time hand gesture recognition using a standard webcam. Translating sign language gestures into instant text and natural Text-to-Speech audio inside a two-way conversational interface.
      </p>
      <div class="mt-9 flex flex-wrap items-center justify-center gap-4">
        <a href="#live-demo" class="px-6 py-3.5 rounded-xl bg-gradient-to-r from-cyan-500 to-emerald-500 hover:from-cyan-400 hover:to-emerald-400 text-slate-950 font-bold text-base transition shadow-lg shadow-cyan-500/25 flex items-center gap-2">
          <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M15 10l4.553-2.276A1 1 0 0121 8.618v6.764a1 1 0 01-1.447.894L15 14M5 18h8a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v8a2 2 0 002 2z"/></svg>
          Try Interactive Demo
        </a>
        <a href="#architecture" class="px-6 py-3.5 rounded-xl bg-slate-900 hover:bg-slate-800 text-white font-semibold text-base border border-slate-700 transition">
          Explore Architecture
        </a>
      </div>

      <!-- Quick Feature Pills -->
      <div class="mt-14 grid grid-cols-2 md:grid-cols-4 gap-4 max-w-4xl mx-auto text-left">
        <div class="p-4 rounded-xl bg-slate-900/70 border border-slate-800">
          <div class="text-cyan-400 font-mono text-xs mb-1">01 / VISION</div>
          <div class="font-semibold text-white text-sm">Webcam Hand Tracking</div>
        </div>
        <div class="p-4 rounded-xl bg-slate-900/70 border border-slate-800">
          <div class="text-emerald-400 font-mono text-xs mb-1">02 / TRANSLATE</div>
          <div class="font-semibold text-white text-sm">Gesture-to-Text Engine</div>
        </div>
        <div class="p-4 rounded-xl bg-slate-900/70 border border-slate-800">
          <div class="text-cyan-400 font-mono text-xs mb-1">03 / VOICE</div>
          <div class="font-semibold text-white text-sm">Instant TTS Output</div>
        </div>
        <div class="p-4 rounded-xl bg-slate-900/70 border border-slate-800">
          <div class="text-emerald-400 font-mono text-xs mb-1">04 / DIALOGUE</div>
          <div class="font-semibold text-white text-sm">Two-Way Chat UI</div>
        </div>
      </div>
    </div>
  </section>

  <!-- Problem & Solution Section -->
  <section id="problem-solution" class="py-20 border-b border-slate-800/80">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center max-w-3xl mx-auto mb-14">
        <h2 class="text-3xl font-bold text-white">Bridging the Everyday Communication Gap</h2>
        <p class="mt-3 text-slate-400">Designed to empower hearing and speech impaired individuals in clinics, classrooms, workplaces, and daily interactions.</p>
      </div>

      <div class="grid md:grid-cols-2 gap-8">
        <!-- Problem Card -->
        <div class="p-8 rounded-2xl bg-slate-900/60 border border-rose-500/20 relative overflow-hidden">
          <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-rose-500/10 text-rose-300 text-xs font-mono mb-5">
            THE CHALLENGE
          </div>
          <h3 class="text-2xl font-bold text-white mb-4">Everyday Communication Barriers</h3>
          <p class="text-slate-300 leading-relaxed mb-6">
            Hearing and speech impaired individuals face constant friction in everyday interactions because most people around them do not understand sign language.
          </p>
          <ul class="space-y-3 text-sm text-slate-300">
            <li class="flex items-start gap-3">
              <span class="text-rose-400 font-bold mt-0.5">✕</span>
              <span>Reliance on human interpreters or slow manual typing on phones during urgent conversations.</span>
            </li>
            <li class="flex items-start gap-3">
              <span class="text-rose-400 font-bold mt-0.5">✕</span>
              <span>Expensive specialized sensor gloves that are impractical for everyday public use.</span>
            </li>
            <li class="flex items-start gap-3">
              <span class="text-rose-400 font-bold mt-0.5">✕</span>
              <span>One-way tools that fail to support natural back-and-forth dialogue with listeners.</span>
            </li>
          </ul>
        </div>

        <!-- Solution Card -->
        <div class="p-8 rounded-2xl bg-slate-900/60 border border-emerald-500/30 relative overflow-hidden">
          <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-emerald-500/10 text-emerald-300 text-xs font-mono mb-5">
            OUR SOLUTION
          </div>
          <h3 class="text-2xl font-bold text-white mb-4">Accessible Vision-to-Voice Pipeline</h3>
          <p class="text-slate-300 leading-relaxed mb-6">
            SignAble AI uses any standard laptop or mobile webcam to detect hand gestures in real time and convert them into spoken words and conversational text.
          </p>
          <ul class="space-y-3 text-sm text-slate-200">
            <li class="flex items-start gap-3">
              <span class="text-emerald-400 font-bold mt-0.5">✓</span>
              <span><strong>Zero Extra Hardware:</strong> Works purely with a built-in webcam and computer vision landmarks.</span>
            </li>
            <li class="flex items-start gap-3">
              <span class="text-emerald-400 font-bold mt-0.5">✓</span>
              <span><strong>Selected Sign Gestures to Text:</strong> High-accuracy classification of essential daily phrases.</span>
            </li>
            <li class="flex items-start gap-3">
              <span class="text-emerald-400 font-bold mt-0.5">✓</span>
              <span><strong>Text-to-Speech + Two-Way Chat:</strong> Speaks the translated sign aloud while letting the other person reply cleanly on screen.</span>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Interactive Prototype Section -->
  <section id="live-demo" class="py-20 bg-slate-950/60 border-b border-slate-800/80">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex flex-col md:flex-row md:items-end justify-between mb-10 gap-4">
        <div>
          <span class="text-xs font-mono uppercase tracking-wider text-cyan-400">Interactive Prototype</span>
          <h2 class="text-3xl font-bold text-white mt-1">SignAble AI Live Studio</h2>
          <p class="text-slate-400 mt-2 max-w-2xl">
            Enable your webcam or click any gesture preset below to simulate real-time 21-point hand landmark detection, text translation, and Text-to-Speech synthesis.
          </p>
        </div>
        <div class="flex items-center gap-3">
          <button id="toggleCamBtn" onclick="toggleWebcam()" class="px-4 py-2.5 rounded-xl bg-slate-800 hover:bg-slate-700 border border-slate-600 text-sm font-semibold text-white flex items-center gap-2 transition">
            <span id="camDot" class="w-2.5 h-2.5 rounded-full bg-amber-400"></span>
            <span id="camBtnText">Enable Live Webcam</span>
          </button>
          <label class="flex items-center gap-2 px-3.5 py-2.5 rounded-xl bg-slate-900 border border-slate-800 text-sm text-slate-300 cursor-pointer select-none">
            <input id="autoSpeakToggle" type="checkbox" checked class="accent-cyan-500 w-4 h-4 rounded">
            Auto-Speak (TTS)
          </label>
        </div>
      </div>

      <!-- Main Split Studio -->
      <div class="grid lg:grid-cols-12 gap-8 items-start">
        
        <!-- Left Column: Webcam & Gesture Detection (7 cols) -->
        <div class="lg:col-span-7 space-y-6">
          <div class="rounded-2xl bg-slate-900 border border-slate-800 overflow-hidden shadow-2xl">
            <!-- Viewport Header -->
            <div class="px-4 py-3 bg-slate-950 border-b border-slate-800 flex items-center justify-between text-xs font-mono">
              <div class="flex items-center gap-2 text-slate-300">
                <span class="w-2 h-2 rounded-full bg-emerald-400"></span>
                <span id="visionModeLabel">CV SIMULATOR MODE (21 LANDMARKS)</span>
              </div>
              <div class="text-cyan-400" id="fpsCounter">30 FPS • CONFIDENCE: 98.4%</div>
            </div>

            <!-- Video / Canvas Container -->
            <div class="relative aspect-video bg-slate-950 flex items-center justify-center overflow-hidden">
              <video id="webcamVideo" autoplay playsinline muted class="hidden w-full h-full object-cover scale-x-[-1]"></video>
              <canvas id="landmarkCanvas" width="640" height="360" class="w-full h-full object-cover"></canvas>

              <!-- HUD Overlay: Detected Sign -->
              <div class="absolute bottom-4 left-4 right-4 flex flex-wrap items-center justify-between gap-3 bg-slate-950/85 backdrop-blur-md border border-slate-700/80 rounded-xl p-3.5">
                <div>
                  <div class="text-[11px] font-mono text-slate-400 uppercase">Detected Sign Gesture</div>
                  <div id="detectedGestureText" class="text-xl sm:text-2xl font-bold text-cyan-300">
                    "Hello / Namaste"
                  </div>
                </div>
                <button onclick="speakCurrentText()" class="px-4 py-2.5 rounded-lg bg-emerald-500 hover:bg-emerald-400 text-slate-950 font-bold text-sm flex items-center gap-2 transition shadow-lg shadow-emerald-500/20">
                  <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2.4" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M15.536 8.464a5 5 0 010 7.072m2.828-9.9a9 9 0 010 12.728M5.586 15H4a1 1 0 01-1-1v-4a1 1 0 011-1h1.586l4.707-4.707C10.923 3.663 12 4.109 12 5v14c0 .891-1.077 1.337-1.707.707L5.586 15z"/></svg>
                  Speak Output
                </button>
              </div>
            </div>
          </div>

          <!-- Gesture Trigger Pad -->
          <div class="p-5 rounded-2xl bg-slate-900/90 border border-slate-800">
            <div class="flex items-center justify-between mb-3">
              <h3 class="text-sm font-semibold text-white">Select / Simulate Hand Gesture</h3>
              <span class="text-xs text-slate-400">Click a gesture to detect, convert & speak</span>
            </div>
            <div id="gestureGrid" class="grid grid-cols-2 sm:grid-cols-4 gap-2.5">
              <!-- Populated by JS -->
            </div>
          </div>
        </div>

        <!-- Right Column: Basic Conversational Interface (5 cols) -->
        <div class="lg:col-span-5 rounded-2xl bg-slate-900 border border-slate-800 flex flex-col h-[610px] shadow-2xl">
          <!-- Chat Header -->
          <div class="px-5 py-4 bg-slate-950 border-b border-slate-800 flex items-center justify-between rounded-t-2xl">
            <div>
              <h3 class="font-bold text-white text-base">Two-Way Conversation</h3>
              <p class="text-xs text-slate-400">Signer (Gesture → Voice) ↔ Listener (Text Reply)</p>
            </div>
            <div class="flex items-center gap-2">
              <!-- Audio Visualizer Bars -->
              <div id="ttsWave" class="hidden items-end gap-1 h-6 px-2">
                <span class="w-1 bg-emerald-400 rounded-full wave-bar"></span>
                <span class="w-1 bg-cyan-400 rounded-full wave-bar"></span>
                <span class="w-1 bg-emerald-400 rounded-full wave-bar"></span>
                <span class="w-1 bg-cyan-400 rounded-full wave-bar"></span>
              </div>
              <button onclick="clearChat()" class="text-xs px-2.5 py-1.5 rounded-lg bg-slate-800 hover:bg-slate-700 text-slate-300 transition">
                Clear
              </button>
            </div>
          </div>

          <!-- Messages Feed -->
          <div id="chatFeed" class="flex-1 overflow-y-auto p-4 space-y-3.5">
            <!-- Initial Messages -->
          </div>

          <!-- Quick Listener Replies -->
          <div class="px-4 pt-2.5 pb-1.5 border-t border-slate-800/80 bg-slate-950/50">
            <div class="text-[11px] font-mono text-slate-400 mb-1.5">LISTENER QUICK REPLIES:</div>
            <div class="flex flex-wrap gap-1.5">
              <button onclick="sendListenerReply('Hello! How can I assist you today?')" class="text-xs px-2.5 py-1 rounded-full bg-slate-800 hover:bg-slate-700 text-slate-200 transition">
                Hello! How can I assist you?
              </button>
              <button onclick="sendListenerReply('Please wait a moment, I am getting help.')" class="text-xs px-2.5 py-1 rounded-full bg-slate-800 hover:bg-slate-700 text-slate-200 transition">
                Getting help now
              </button>
              <button onclick="sendListenerReply('Yes, I understand completely.')" class="text-xs px-2.5 py-1 rounded-full bg-slate-800 hover:bg-slate-700 text-slate-200 transition">
                Yes, I understand
              </button>
            </div>
          </div>

          <!-- Listener Text Input -->
          <form onsubmit="handleListenerSubmit(event)" class="p-3.5 bg-slate-950 border-t border-slate-800 rounded-b-2xl flex gap-2">
            <input
              id="listenerInput"
              type="text"
              placeholder="Listener: Type a reply to show on screen..."
              class="flex-1 bg-slate-900 border border-slate-700 focus:border-cyan-500 focus:outline-none rounded-xl px-3.5 py-2.5 text-sm text-white placeholder-slate-500"
            />
            <button type="submit" class="px-4 py-2.5 rounded-xl bg-cyan-500 hover:bg-cyan-400 text-slate-950 font-bold text-sm transition">
              Send
            </button>
          </form>
        </div>

      </div>
    </div>
  </section>

  <!-- System Architecture / Workflow -->
  <section id="architecture" class="py-20 border-b border-slate-800/80">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center max-w-3xl mx-auto mb-14">
        <span class="text-xs font-mono text-cyan-400 uppercase tracking-wider">Computer Vision Pipeline</span>
        <h2 class="text-3xl font-bold text-white mt-1">How SignAble AI Works</h2>
        <p class="mt-3 text-slate-400">A low-latency 4-stage pipeline converting raw webcam frames into natural speech.</p>
      </div>

      <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-6">
        <div class="p-6 rounded-2xl bg-slate-900/70 border border-slate-800">
          <div class="w-10 h-10 rounded-xl bg-cyan-500/15 text-cyan-400 font-mono font-bold flex items-center justify-center mb-4">01</div>
          <h3 class="font-bold text-white text-lg mb-2">Webcam Capture</h3>
          <p class="text-sm text-slate-400 leading-relaxed">OpenCV / WebRTC captures real-time video frames from any standard device camera without external sensors.</p>
        </div>
        <div class="p-6 rounded-2xl bg-slate-900/70 border border-slate-800">
          <div class="w-10 h-10 rounded-xl bg-emerald-500/15 text-emerald-400 font-mono font-bold flex items-center justify-center mb-4">02</div>
          <h3 class="font-bold text-white text-lg mb-2">Hand Landmark Detection</h3>
          <p class="text-sm text-slate-400 leading-relaxed">MediaPipe Hands extracts 21 3D keypoint coordinates per hand, invariant to background lighting and skin tone.</p>
        </div>
        <div class="p-6 rounded-2xl bg-slate-900/70 border border-slate-800">
          <div class="w-10 h-10 rounded-xl bg-cyan-500/15 text-cyan-400 font-mono font-bold flex items-center justify-center mb-4">03</div>
          <h3 class="font-bold text-white text-lg mb-2">Gesture Classification</h3>
          <p class="text-sm text-slate-400 leading-relaxed">A trained neural classifier maps normalized landmark vectors into selected sign vocabulary and phrases.</p>
        </div>
        <div class="p-6 rounded-2xl bg-slate-900/70 border border-slate-800">
          <div class="w-10 h-10 rounded-xl bg-emerald-500/15 text-emerald-400 font-mono font-bold flex items-center justify-center mb-4">04</div>
          <h3 class="font-bold text-white text-lg mb-2">TTS & Chat UI</h3>
          <p class="text-sm text-slate-400 leading-relaxed">Recognized text renders in the conversational thread and triggers instant Text-to-Speech voice output.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Tech Stack & Future Scope -->
  <section id="tech-stack" class="py-20">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid lg:grid-cols-2 gap-12">
        <div>
          <h3 class="text-2xl font-bold text-white mb-4">Technology Stack</h3>
          <p class="text-slate-400 text-sm mb-6">Built with lightweight, real-time computer vision and browser speech technologies.</p>
          <div class="grid grid-cols-2 gap-4">
            <div class="p-4 rounded-xl bg-slate-900 border border-slate-800">
              <div class="font-bold text-cyan-400">OpenCV & MediaPipe</div>
              <div class="text-xs text-slate-400 mt-1">Frame processing & 21-point hand skeletal tracking</div>
            </div>
            <div class="p-4 rounded-xl bg-slate-900 border border-slate-800">
              <div class="font-bold text-emerald-400">Python / TensorFlow</div>
              <div class="text-xs text-slate-400 mt-1">Sign gesture model training & coordinate classification</div>
            </div>
            <div class="p-4 rounded-xl bg-slate-900 border border-slate-800">
              <div class="font-bold text-cyan-400">Web Speech API / pyttsx3</div>
              <div class="text-xs text-slate-400 mt-1">Low-latency Text-to-Speech voice synthesis</div>
            </div>
            <div class="p-4 rounded-xl bg-slate-900 border border-slate-800">
              <div class="font-bold text-emerald-400">HTML5 / Tailwind / JS</div>
              <div class="text-xs text-slate-400 mt-1">Accessible high-contrast conversational interface</div>
            </div>
          </div>
        </div>

        <div>
          <h3 class="text-2xl font-bold text-white mb-4">Future Roadmap</h3>
          <p class="text-slate-400 text-sm mb-6">Scaling from core gestures to full continuous sign language translation.</p>
          <div class="space-y-3">
            <div class="p-4 rounded-xl bg-slate-900/70 border border-slate-800 flex items-center justify-between">
              <div>
                <div class="font-semibold text-white text-sm">Indian Sign Language (ISL) & ASL Expansion</div>
                <div class="text-xs text-slate-400">Expanding dataset to 200+ dynamic two-handed gestures</div>
              </div>
              <span class="text-xs font-mono px-2.5 py-1 rounded bg-cyan-500/10 text-cyan-300">Phase 2</span>
            </div>
            <div class="p-4 rounded-xl bg-slate-900/70 border border-slate-800 flex items-center justify-between">
              <div>
                <div class="font-semibold text-white text-sm">Speech-to-Text for Listener Replies</div>
                <div class="text-xs text-slate-400">Automatic voice transcription so listeners don't even need to type</div>
              </div>
              <span class="text-xs font-mono px-2.5 py-1 rounded bg-emerald-500/10 text-emerald-300">Phase 3</span>
            </div>
            <div class="p-4 rounded-xl bg-slate-900/70 border border-slate-800 flex items-center justify-between">
              <div>
                <div class="font-semibold text-white text-sm">Multilingual Regional Voice Output</div>
                <div class="text-xs text-slate-400">Hindi, English, and regional TTS output for local accessibility</div>
              </div>
              <span class="text-xs font-mono px-2.5 py-1 rounded bg-cyan-500/10 text-cyan-300">Phase 4</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="border-t border-slate-800/80 py-8 text-center text-sm text-slate-500">
    <div class="max-w-7xl mx-auto px-4">
      <p class="text-slate-300 font-semibold">SignAble AI – Communication Without Barriers</p>
      <p class="mt-1 text-xs">Computer Vision Accessibility Project • Hand Gesture Detection • Gesture-to-Text • Text-to-Speech</p>
    </div>
  </footer>

  <!-- Interactive Prototype Logic -->
  <script>
    const GESTURES = [
      { id: 'hello', label: 'Hello / Namaste', icon: '👋', confidence: '99.1%', spread: 1.0, curl: 0.0 },
      { id: 'thanks', label: 'Thank You', icon: '🙏', confidence: '98.4%', spread: 0.4, curl: 0.1 },
      { id: 'help', label: 'I Need Help', icon: '🆘', confidence: '97.8%', spread: 0.8, curl: 0.35 },
      { id: 'yes', label: 'Yes', icon: '👍', confidence: '99.4%', spread: 0.3, curl: 0.85 },
      { id: 'no', label: 'No', icon: '✋', confidence: '98.0%', spread: 0.65, curl: 0.2 },
      { id: 'how', label: 'How are you?', icon: '🤟', confidence: '96.9%', spread: 0.9, curl: 0.45 },
      { id: 'water', label: 'Water / Food', icon: '💧', confidence: '97.5%', spread: 0.5, curl: 0.5 },
      { id: 'please', label: 'Please', icon: '🤲', confidence: '98.2%', spread: 0.75, curl: 0.15 }
    ];

    let activeGesture = GESTURES[0];
    let webcamStream = null;
    let isWebcamOn = false;

    const canvas = document.getElementById('landmarkCanvas');
    const ctx = canvas.getContext('2d');
    const videoEl = document.getElementById('webcamVideo');

    // Render Gesture Buttons
    function initGestureGrid() {
      const grid = document.getElementById('gestureGrid');
      grid.innerHTML = GESTURES.map(g => `
        <button
          onclick="triggerGesture('${g.id}')"
          id="btn-${g.id}"
          class="gesture-btn p-3 rounded-xl border text-left transition flex items-center gap-2.5 ${
            g.id === activeGesture.id
              ? 'bg-cyan-500/15 border-cyan-400 text-white'
              : 'bg-slate-950/80 border-slate-800 hover:border-slate-600 text-slate-300'
          }"
        >
          <span class="text-xl">${g.icon}</span>
          <span class="text-xs font-semibold leading-tight">${g.label}</span>
        </button>
      `).join('');
    }

    // Trigger Gesture Detection
    function triggerGesture(id) {
      const found = GESTURES.find(g => g.id === id);
      if (!found) return;
      activeGesture = found;

      // Update UI highlights
      document.querySelectorAll('.gesture-btn').forEach(btn => {
        btn.classList.remove('bg-cyan-500/15', 'border-cyan-400', 'text-white');
        btn.classList.add('bg-slate-950/80', 'border-slate-800', 'text-slate-300');
      });
      const activeBtn = document.getElementById(`btn-${id}`);
      if (activeBtn) {
        activeBtn.classList.remove('bg-slate-950/80', 'border-slate-800', 'text-slate-300');
        activeBtn.classList.add('bg-cyan-500/15', 'border-cyan-400', 'text-white');
      }

      document.getElementById('detectedGestureText').textContent = `"${found.label}"`;
      document.getElementById('fpsCounter').textContent = `30 FPS • CONFIDENCE: ${found.confidence}`;

      addMessage('signer', found.label);

      if (document.getElementById('autoSpeakToggle').checked) {
        speakText(found.label);
      }
    }

    // Text-to-Speech Output
    function speakText(text) {
      if (!('speechSynthesis' in window)) return;
      window.speechSynthesis.cancel();
      const utterance = new SpeechSynthesisUtterance(text);
      utterance.rate = 0.98;
      utterance.pitch = 1.0;

      const wave = document.getElementById('ttsWave');
      utterance.onstart = () => {
        wave.classList.remove('hidden');
        wave.classList.add('flex');
      };
      utterance.onend = () => {
        wave.classList.add('hidden');
        wave.classList.remove('flex');
      };
      window.speechSynthesis.speak(utterance);
    }

    function speakCurrentText() {
      speakText(activeGesture.label);
    }

    // Conversational Chat Logic
    function addMessage(sender, text) {
      const feed = document.getElementById('chatFeed');
      const time = new Date().toLocaleTimeString([], { hour: '2-digit', minute: '2-digit' });
      const wrapper = document.createElement('div');

      if (sender === 'signer') {
        wrapper.className = 'flex flex-col items-start';
        wrapper.innerHTML = `
          <div class="text-[11px] font-mono text-cyan-400 mb-1">SIGNER (GESTURE → TTS) • ${time}</div>
          <div class="max-w-[85%] px-4 py-2.5 rounded-2xl rounded-tl-sm bg-cyan-500/15 border border-cyan-500/30 text-white text-sm flex items-center justify-between gap-3">
            <span>${text}</span>
            <button onclick="speakText('${text.replace(/'/g, "\\'")}')" title="Replay TTS" class="text-cyan-300 hover:text-white shrink-0">
              🔊
            </button>
          </div>
        `;
      } else {
        wrapper.className = 'flex flex-col items-end';
        wrapper.innerHTML = `
          <div class="text-[11px] font-mono text-emerald-400 mb-1">LISTENER • ${time}</div>
          <div class="max-w-[85%] px-4 py-2.5 rounded-2xl rounded-tr-sm bg-slate-800 border border-slate-700 text-slate-100 text-sm">
            ${text}
          </div>
        `;
      }

      feed.appendChild(wrapper);
      feed.scrollTop = feed.scrollHeight;
    }

    function sendListenerReply(text) {
      addMessage('listener', text);
    }

    function handleListenerSubmit(e) {
      e.preventDefault();
      const input = document.getElementById('listenerInput');
      const val = input.value.trim();
      if (!val) return;
      addMessage('listener', val);
      input.value = '';
    }

    function clearChat() {
      document.getElementById('chatFeed').innerHTML = '';
    }

    // Webcam Toggle
    async function toggleWebcam() {
      const btnText = document.getElementById('camBtnText');
      const camDot = document.getElementById('camDot');
      const modeLabel = document.getElementById('visionModeLabel');

      if (isWebcamOn) {
        if (webcamStream) {
          webcamStream.getTracks().forEach(track => track.stop());
        }
        videoEl.classList.add('hidden');
        isWebcamOn = false;
        btnText.textContent = 'Enable Live Webcam';
        camDot.className = 'w-2.5 h-2.5 rounded-full bg-amber-400';
        modeLabel.textContent = 'CV SIMULATOR MODE (21 LANDMARKS)';
        return;
      }

      try {
        webcamStream = await navigator.mediaDevices.getUserMedia({ video: true });
        videoEl.srcObject = webcamStream;
        videoEl.classList.remove('hidden');
        isWebcamOn = true;
        btnText.textContent = 'Stop Webcam';
        camDot.className = 'w-2.5 h-2.5 rounded-full bg-emerald-400 animate-ping';
        modeLabel.textContent = 'LIVE WEBCAM + LANDMARK OVERLAY';
      } catch (err) {
        alert('Camera permission denied or unavailable in this browser preview. Continuing in interactive CV Simulator mode.');
      }
    }

    // Animated 21-Point Hand Landmark Skeleton Overlay
    let tick = 0;
    function drawHandLandmarks() {
      tick += 0.04;
      ctx.clearRect(0, 0, canvas.width, canvas.height);

      if (!isWebcamOn) {
        // Dark sci-fi CV grid backdrop
        ctx.fillStyle = '#070b14';
        ctx.fillRect(0, 0, canvas.width, canvas.height);
        ctx.strokeStyle = 'rgba(6, 182, 212, 0.08)';
        ctx.lineWidth = 1;
        for (let x = 0; x < canvas.width; x += 32) {
          ctx.beginPath(); ctx.moveTo(x, 0); ctx.lineTo(x, canvas.height); ctx.stroke();
        }
        for (let y = 0; y < canvas.height; y += 32) {
          ctx.beginPath(); ctx.moveTo(0, y); ctx.lineTo(canvas.width, y); ctx.stroke();
        }
      }

      const cx = canvas.width / 2 + Math.sin(tick) * 8;
      const cy = canvas.height / 2 + 35 + Math.cos(tick * 0.8) * 6;

      // Bounding box
      ctx.strokeStyle = 'rgba(16, 185, 129, 0.65)';
      ctx.lineWidth = 2;
      ctx.setLineDash([6, 4]);
      ctx.strokeRect(cx - 105, cy - 155, 210, 215);
      ctx.setLineDash([]);

      ctx.fillStyle = '#10b981';
      ctx.font = '11px JetBrains Mono, monospace';
      ctx.fillText(`HAND_ROI [${activeGesture.id.toUpperCase()}]`, cx - 100, cy - 162);

      // Wrist point (0)
      const wrist = { x: cx, y: cy + 40 };
      const spread = activeGesture.spread;
      const curl = activeGesture.curl;

      const fingerAngles = [-0.65 * spread, -0.28 * spread, 0, 0.28 * spread, 0.58 * spread];
      const fingerLengths = [75, 105, 118, 108, 88];

      const allPoints = [wrist];

      fingerAngles.forEach((angle, fIdx) => {
        const len = fingerLengths[fIdx] * (1 - curl * 0.45);
        let prev = wrist;
        for (let j = 1; j <= 4; j++) {
          const frac = j / 4;
          const waveOffset = Math.sin(tick + fIdx) * 2.5;
          const px = wrist.x + Math.sin(angle) * (len * frac + 22) + waveOffset;
          const py = wrist.y - Math.cos(angle) * (len * frac + 22);
          const pt = { x: px, y: py };
          allPoints.push(pt);

          // Draw bone connection
          ctx.strokeStyle = '#06b6d4';
          ctx.lineWidth = 2.5;
          ctx.beginPath();
          ctx.moveTo(prev.x, prev.y);
          ctx.lineTo(pt.x, pt.y);
          ctx.stroke();

          prev = pt;
        }
      });

      // Draw 21 landmark nodes
      allPoints.forEach((pt, idx) => {
        ctx.beginPath();
        ctx.arc(pt.x, pt.y, idx === 0 ? 5.5 : 4, 0, Math.PI * 2);
        ctx.fillStyle = idx === 0 ? '#10b981' : '#f8fafc';
        ctx.fill();
        ctx.strokeStyle = '#06b6d4';
        ctx.lineWidth = 1.5;
        ctx.stroke();
      });

      requestAnimationFrame(drawHandLandmarks);
    }

    // Boot
    initGestureGrid();
    addMessage('signer', 'Hello / Namaste');
    addMessage('listener', 'Welcome! SignAble AI is ready for conversation.');
    drawHandLandmarks();
  </script>
</body>
</html>
