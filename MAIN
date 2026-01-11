<html lang="en" class="h-full">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>NCAE Practice Test - National Career Assessment Examination</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script src="/_sdk/element_sdk.js"></script>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&amp;display=swap" rel="stylesheet">
  <style>
    body {
      box-sizing: border-box;
    }
    * {
      font-family: 'Poppins', sans-serif;
    }
    .question-card {
      animation: slideIn 0.4s ease-out;
    }
    @keyframes slideIn {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
    .progress-fill {
      transition: width 0.5s ease-out;
    }
    .option-btn {
      transition: all 0.2s ease;
    }
    .option-btn:hover:not(.selected):not(.correct):not(.incorrect) {
      transform: translateX(8px);
      border-color: #10b981;
    }
    .result-card {
      animation: popIn 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    }
    @keyframes popIn {
      from {
        opacity: 0;
        transform: scale(0.8);
      }
      to {
        opacity: 1;
        transform: scale(1);
      }
    }
    .category-tag {
      animation: fadeIn 0.3s ease-out;
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
    .pulse-animation {
      animation: pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
    }
    @keyframes pulse {
      0%, 100% {
        opacity: 1;
      }
      50% {
        opacity: .5;
      }
    }
    .timer-warning {
      animation: timerPulse 1s ease-in-out infinite;
    }
    @keyframes timerPulse {
      0%, 100% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.05);
      }
    }
  </style>
  <style>@view-transition { navigation: auto; }</style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
 </head>
 <body class="h-full">
  <div id="app-wrapper" class="h-full w-full overflow-auto" style="background: linear-gradient(135deg, #065f46 0%, #047857 25%, #10b981 50%, #047857 75%, #065f46 100%);"><!-- Login Screen -->
   <div id="login-screen" class="min-h-full flex items-center justify-center p-6 relative">
    <div class="max-w-md w-full">
     <div class="bg-white/95 backdrop-blur-lg rounded-3xl p-8 md:p-10 border border-white/40 shadow-2xl">
      <div class="text-center mb-8">
       <div class="inline-flex items-center justify-center w-20 h-20 rounded-full mb-4 border-4 border-white shadow-xl" style="background: linear-gradient(135deg, #fbbf24, #f59e0b);">
        <svg class="w-12 h-12 text-white" fill="currentColor" viewbox="0 0 24 24"><path d="M12 3L1 9L5 11.18V17.18L12 21L19 17.18V11.18L21 10.09V17H23V9L12 3ZM18.82 9L12 12.72L5.18 9L12 5.28L18.82 9ZM17 15.99L12 18.72L7 15.99V12.27L12 15L17 12.27V15.99Z" />
        </svg>
       </div>
       <h2 class="text-3xl font-bold text-gray-800 mb-2">NCAE Practice Test</h2>
       <p class="text-gray-600">Sign in with your DepEd account</p>
      </div>
      <form id="login-form" class="space-y-5">
       <div><label for="username" class="block text-sm font-semibold text-gray-700 mb-2">Username (LRN)</label> <input type="text" id="username" placeholder="lrn@r7-2.deped.gov.ph" class="w-full px-4 py-3 rounded-xl border-2 border-gray-300 focus:border-emerald-500 focus:outline-none transition-colors text-gray-800" required>
       </div>
       <div><label for="password" class="block text-sm font-semibold text-gray-700 mb-2">Password</label> <input type="password" id="password" placeholder="Enter your password" class="w-full px-4 py-3 rounded-xl border-2 border-gray-300 focus:border-emerald-500 focus:outline-none transition-colors text-gray-800" required>
       </div>
       <div id="login-error" class="hidden bg-red-50 border-2 border-red-200 rounded-xl p-3 text-red-700 text-sm flex items-center gap-2">
        <svg class="w-5 h-5 flex-shrink-0" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4m0 4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
        </svg><span>Invalid username or password. Please try again.</span>
       </div><button type="submit" id="login-btn" class="w-full px-8 py-4 rounded-xl font-bold text-white text-lg transition-all hover:scale-105 shadow-lg" style="background: linear-gradient(135deg, #fbbf24, #f59e0b);"> Sign In </button>
      </form>
      <div class="mt-6 p-4 bg-blue-50 rounded-xl border border-blue-200">
       <p class="text-xs text-gray-600 text-center"><strong class="text-blue-700">Demo Credentials:</strong><br>
         Username: lrn@r7-2.deped.gov.ph<br>
         Password: G02@0012</p>
      </div>
     </div>
    </div>
    <footer class="fixed top-6 right-6 text-white/90 text-xs font-medium text-right">
     <p>NCAE Practice Test developed by</p>
     <p class="font-semibold">Joel P. Rodriguez, LPT, MAVED</p>
    </footer>
   </div><!-- Start Screen -->
   <div id="start-screen" class="min-h-full flex items-center justify-center p-6 hidden">
    <div class="max-w-4xl w-full text-center">
     <div class="mb-8">
      <div class="inline-flex items-center justify-center w-28 h-28 rounded-full mb-6 border-4 border-white shadow-2xl" style="background: linear-gradient(135deg, #fbbf24, #f59e0b);">
       <svg class="w-16 h-16 text-white" fill="currentColor" viewbox="0 0 24 24"><path d="M12 3L1 9L5 11.18V17.18L12 21L19 17.18V11.18L21 10.09V17H23V9L12 3ZM18.82 9L12 12.72L5.18 9L12 5.28L18.82 9ZM17 15.99L12 18.72L7 15.99V12.27L12 15L17 12.27V15.99Z" />
       </svg>
      </div>
      <h1 id="main-title" class="text-5xl md:text-6xl font-bold text-white mb-4 drop-shadow-lg">NCAE Practice Test</h1>
      <p id="subtitle" class="text-xl text-emerald-100 mb-8">National Career Assessment Examination</p>
     </div>
     <div class="grid grid-cols-2 md:grid-cols-4 gap-4 mb-10">
      <div class="bg-white/10 backdrop-blur-sm rounded-xl p-5 border border-white/20">
       <div class="text-4xl font-bold text-amber-300">
        70
       </div>
       <div class="text-emerald-100 text-sm">
        Questions
       </div>
      </div>
      <div class="bg-white/10 backdrop-blur-sm rounded-xl p-5 border border-white/20">
       <div class="text-4xl font-bold text-amber-300">
        7
       </div>
       <div class="text-emerald-100 text-sm">
        Categories
       </div>
      </div>
      <div class="bg-white/10 backdrop-blur-sm rounded-xl p-5 border border-white/20">
       <div class="text-4xl font-bold text-amber-300">
        10
       </div>
       <div class="text-emerald-100 text-sm">
        Min / Category
       </div>
      </div>
      <div class="bg-white/10 backdrop-blur-sm rounded-xl p-5 border border-white/20">
       <div class="text-4xl font-bold text-amber-300">
        📊
       </div>
       <div class="text-emerald-100 text-sm">
        Full Results
       </div>
      </div>
     </div>
     <div class="bg-white/10 backdrop-blur-md rounded-2xl p-8 mb-8 border border-white/20 text-left">
      <h3 class="text-white font-semibold text-lg mb-6 flex items-center gap-2">
       <svg class="w-6 h-6 text-amber-300" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-3 7h3m-3 4h3m-6-4h.01M9 16h.01" />
       </svg> Official NCAE Test Categories</h3>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-sm">
       <div class="flex items-center gap-3 text-white bg-white/5 p-3 rounded-lg"><span class="w-4 h-4 rounded-full bg-blue-400 flex-shrink-0"></span> <span><strong>Numerical Reasoning</strong> - 10 items</span>
       </div>
       <div class="flex items-center gap-3 text-white bg-white/5 p-3 rounded-lg"><span class="w-4 h-4 rounded-full bg-rose-400 flex-shrink-0"></span> <span><strong>Verbal Reasoning (English)</strong> - 10 items</span>
       </div>
       <div class="flex items-center gap-3 text-white bg-white/5 p-3 rounded-lg"><span class="w-4 h-4 rounded-full bg-amber-400 flex-shrink-0"></span> <span><strong>Verbal Reasoning (Filipino)</strong> - 10 items</span>
       </div>
       <div class="flex items-center gap-3 text-white bg-white/5 p-3 rounded-lg"><span class="w-4 h-4 rounded-full bg-purple-400 flex-shrink-0"></span> <span><strong>Spatial Reasoning</strong> - 10 items</span>
       </div>
       <div class="flex items-center gap-3 text-white bg-white/5 p-3 rounded-lg"><span class="w-4 h-4 rounded-full bg-cyan-400 flex-shrink-0"></span> <span><strong>Mechanical Reasoning</strong> - 10 items</span>
       </div>
       <div class="flex items-center gap-3 text-white bg-white/5 p-3 rounded-lg"><span class="w-4 h-4 rounded-full bg-emerald-400 flex-shrink-0"></span> <span><strong>Perceptual Accuracy (PARE)</strong> - 10 items</span>
       </div>
       <div class="flex items-center gap-3 text-white bg-white/5 p-3 rounded-lg col-span-1 md:col-span-2"><span class="w-4 h-4 rounded-full bg-fuchsia-400 flex-shrink-0"></span> <span><strong>Career &amp; Occupational Role Explorer (CORE)</strong> - 10 items</span>
       </div>
      </div>
     </div><button id="start-btn" class="px-12 py-5 rounded-xl font-bold text-white text-lg transition-all hover:scale-105 hover:shadow-2xl shadow-xl" style="background: linear-gradient(135deg, #fbbf24, #f59e0b);"> 🚀 Start Practice Test </button>
    </div>
    <footer class="fixed top-6 right-6 text-white/90 text-xs font-medium text-right">
     <p>NCAE Practice Test developed by</p>
     <p class="font-semibold">Joel P. Rodriguez, LPT, MAVED</p>
    </footer>
   </div><!-- Category Introduction Screen -->
   <div id="category-intro-screen" class="min-h-full flex items-center justify-center p-6 hidden">
    <div class="max-w-3xl w-full text-center">
     <div class="bg-white/95 backdrop-blur-lg rounded-3xl p-10 md:p-12 border border-white/40 shadow-2xl">
      <div id="cat-icon" class="text-8xl mb-6">
       🔢
      </div>
      <h2 id="cat-title" class="text-4xl md:text-5xl font-bold text-gray-800 mb-4">Numerical Reasoning</h2>
      <p id="cat-description" class="text-xl text-gray-600 mb-8">Test your mathematical and numerical problem-solving abilities</p>
      <div class="grid grid-cols-3 gap-6 mb-10">
       <div class="bg-emerald-50 rounded-xl p-5 border-2 border-emerald-200">
        <div class="text-3xl font-bold text-emerald-600" id="cat-questions">
         10
        </div>
        <div class="text-gray-600 text-sm font-medium">
         Questions
        </div>
       </div>
       <div class="bg-amber-50 rounded-xl p-5 border-2 border-amber-200">
        <div class="text-3xl font-bold text-amber-600">
         10:00
        </div>
        <div class="text-gray-600 text-sm font-medium">
         Time Limit
        </div>
       </div>
       <div class="bg-blue-50 rounded-xl p-5 border-2 border-blue-200">
        <div class="text-3xl font-bold text-blue-600" id="cat-number">
         1
        </div>
        <div class="text-gray-600 text-sm font-medium">
         of 7
        </div>
       </div>
      </div>
      <div class="bg-yellow-50 border-2 border-yellow-200 rounded-xl p-5 mb-8 text-left">
       <p class="text-gray-700 flex items-start gap-3"><span class="text-2xl">⏱️</span> <span class="flex-1"><strong class="text-yellow-700">Timer Notice:</strong> You will have 10 minutes to complete this section. The timer will start when you click "Begin Section".</span></p>
      </div><button id="begin-category-btn" class="px-12 py-5 rounded-xl font-bold text-white text-lg transition-all hover:scale-105 shadow-xl" style="background: linear-gradient(135deg, #fbbf24, #f59e0b);"> Begin Section → </button>
     </div>
    </div>
   </div><!-- Quiz Screen -->
   <div id="quiz-screen" class="min-h-full p-4 md:p-6 hidden">
    <div class="max-w-4xl mx-auto"><!-- Header -->
     <div class="flex items-center justify-between mb-6">
      <div class="flex items-center gap-3">
       <div class="w-12 h-12 rounded-full flex items-center justify-center border-2 border-white shadow-lg" style="background: linear-gradient(135deg, #fbbf24, #f59e0b);">
        <svg class="w-7 h-7 text-white" fill="currentColor" viewbox="0 0 24 24"><path d="M12 3L1 9L5 11.18V17.18L12 21L19 17.18V11.18L21 10.09V17H23V9L12 3ZM18.82 9L12 12.72L5.18 9L12 5.28L18.82 9ZM17 15.99L12 18.72L7 15.99V12.27L12 15L17 12.27V15.99Z" />
        </svg>
       </div><span class="text-white font-semibold text-lg">NCAE Practice</span>
      </div>
      <div id="timer-display" class="text-white text-lg bg-white/20 px-5 py-3 rounded-xl backdrop-blur-sm font-bold flex items-center gap-2">
       <svg class="w-5 h-5" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
       </svg><span id="timer-text">10:00</span>
      </div>
     </div><!-- Progress Bar -->
     <div class="mb-4">
      <div class="flex justify-between text-emerald-100 text-sm mb-2"><span id="category-progress-text">Question 1 of 10 in this section</span> <span id="overall-progress-text">Overall: 1/70</span>
      </div>
      <div class="h-3 bg-white/20 rounded-full overflow-hidden backdrop-blur-sm">
       <div id="progress-bar" class="progress-fill h-full rounded-full" style="width: 1.4%; background: linear-gradient(90deg, #fbbf24, #f59e0b);"></div>
      </div>
     </div><!-- Question Card -->
     <div id="question-card" class="question-card bg-white/95 backdrop-blur-lg rounded-2xl p-6 md:p-8 border border-white/40 shadow-2xl mb-6">
      <div id="category-tag" class="category-tag inline-block px-4 py-2 rounded-full text-xs font-semibold mb-5 bg-blue-500/20 text-blue-700">
       Numerical Reasoning
      </div>
      <h2 id="question-text" class="text-xl md:text-2xl text-gray-800 font-medium mb-8 leading-relaxed">Loading question...</h2>
      <div id="options-container" class="space-y-3"><!-- Options will be inserted here -->
      </div>
     </div><!-- Navigation -->
     <div class="flex justify-between items-center"><button id="prev-btn" class="px-6 py-3 rounded-xl font-semibold text-white bg-white/20 backdrop-blur-sm border border-white/30 hover:bg-white/30 transition-all disabled:opacity-40 disabled:cursor-not-allowed"> ← Previous </button> <button id="next-btn" class="px-8 py-3 rounded-xl font-semibold text-white transition-all hover:scale-105 shadow-lg disabled:opacity-50 disabled:cursor-not-allowed" style="background: linear-gradient(135deg, #fbbf24, #f59e0b);"> Next → </button>
     </div>
    </div>
   </div><!-- Results Screen -->
   <div id="results-screen" class="min-h-full p-4 md:p-6 hidden">
    <div class="max-w-4xl mx-auto">
     <div class="result-card bg-white/95 backdrop-blur-lg rounded-2xl p-8 md:p-10 border border-white/40 shadow-2xl text-center mb-8">
      <div class="inline-flex items-center justify-center w-24 h-24 rounded-full mb-6" id="result-icon-bg" style="background: linear-gradient(135deg, #10b981, #059669);">
       <svg id="result-icon" class="w-12 h-12 text-white" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
       </svg>
      </div>
      <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-3">Practice Complete!</h2>
      <p class="text-gray-600 text-lg mb-8">Here's your performance summary</p>
      <div class="flex justify-center gap-12 mb-8">
       <div>
        <div id="score-display" class="text-6xl font-bold text-emerald-600">
         0
        </div>
        <div class="text-gray-600 font-medium">
         Correct
        </div>
       </div>
       <div class="w-px bg-gray-300"></div>
       <div>
        <div id="percentage-display" class="text-6xl font-bold text-amber-600">
         0%
        </div>
        <div class="text-gray-600 font-medium">
         Score
        </div>
       </div>
      </div>
     </div><!-- Category Breakdown -->
     <div class="bg-white/95 backdrop-blur-lg rounded-2xl p-8 border border-white/40 shadow-2xl mb-8">
      <h3 class="text-gray-800 font-bold text-xl mb-6 flex items-center gap-2">
       <svg class="w-6 h-6 text-amber-600" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z" />
       </svg> Performance by Category</h3>
      <div id="category-breakdown" class="space-y-5"><!-- Category results will be inserted here -->
      </div>
     </div><!-- Action Buttons -->
     <div class="flex flex-col sm:flex-row gap-4 justify-center"><button id="review-btn" class="px-8 py-4 rounded-xl font-semibold text-white bg-emerald-600 hover:bg-emerald-700 transition-all shadow-lg hover:shadow-xl"> 📝 Review Answers </button> <button id="retry-btn" class="px-8 py-4 rounded-xl font-semibold text-white transition-all hover:scale-105 shadow-lg hover:shadow-xl" style="background: linear-gradient(135deg, #fbbf24, #f59e0b);"> 🔄 Retake Test </button>
     </div>
    </div>
    <footer class="fixed top-6 right-6 text-white/90 text-xs font-medium text-right">
     <p>NCAE Practice Test developed by</p>
     <p class="font-semibold">Joel P. Rodriguez, LPT, MAVED</p>
    </footer>
   </div><!-- Review Screen -->
   <div id="review-screen" class="min-h-full p-4 md:p-6 hidden">
    <div class="max-w-4xl mx-auto">
     <div class="flex items-center justify-between mb-8 bg-white/20 backdrop-blur-sm p-4 rounded-xl">
      <h2 class="text-2xl md:text-3xl font-bold text-white flex items-center gap-3">
       <svg class="w-7 h-7" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z" />
       </svg> Review Your Answers</h2><button id="back-results-btn" class="px-5 py-2 rounded-lg text-white font-medium hover:bg-white/20 transition-all border border-white/30"> ← Back </button>
     </div>
     <div id="review-container" class="space-y-6"><!-- Review items will be inserted here -->
     </div>
     <div class="mt-10 text-center"><button id="retry-from-review-btn" class="px-10 py-4 rounded-xl font-semibold text-white transition-all hover:scale-105 shadow-lg" style="background: linear-gradient(135deg, #fbbf24, #f59e0b);"> 🔄 Retake Test </button>
     </div>
    </div>
    <footer class="fixed top-6 right-6 text-white/90 text-xs font-medium text-right">
     <p>NCAE Practice Test developed by</p>
     <p class="font-semibold">Joel P. Rodriguez, LPT, MAVED</p>
    </footer>
   </div>
  </div>
  <script>
    // Default configuration
    const defaultConfig = {
      main_title: 'NCAE Practice Test',
      subtitle: 'National Career Assessment Examination',
      background_color: '#047857',
      card_color: '#ffffff',
      text_color: '#1f2937',
      primary_action: '#f59e0b',
      accent_color: '#10b981'
    };

    // Category definitions
    const categoryDefinitions = [
      { name: 'Numerical Reasoning', color: 'blue', icon: '🔢', description: 'Test your mathematical and numerical problem-solving abilities', questions: 10 },
      { name: 'Verbal Reasoning (English)', color: 'rose', icon: '📖', description: 'Assess your English vocabulary, grammar, and comprehension', questions: 10 },
      { name: 'Verbal Reasoning (Filipino)', color: 'amber', icon: '📚', description: 'Suriin ang iyong kaalaman sa wikang Filipino', questions: 10 },
      { name: 'Spatial Reasoning', color: 'purple', icon: '🔷', description: 'Evaluate your ability to visualize and manipulate shapes', questions: 10 },
      { name: 'Mechanical Reasoning', color: 'cyan', icon: '⚙����', description: 'Test your understanding of mechanical and physical principles', questions: 10 },
      { name: 'Perceptual Accuracy (PARE)', color: 'emerald', icon: '👁️', description: 'Measure your attention to detail and pattern recognition', questions: 10 },
      { name: 'Career Role Explorer (CORE)', color: 'fuchsia', icon: '💼', description: 'Explore careers that match your interests and skills', questions: 10 }
    ];

    // 70 Questions - 10 items each for 7 categories
    const questions = [
      // NUMERICAL REASONING (10 items)
      {
        category: 'Numerical Reasoning',
        categoryColor: 'blue',
        question: 'What is 25% of 200?',
        options: ['25', '40', '50', '75'],
        correct: 2,
        explanation: '25% = 25/100 = 0.25. So 0.25 × 200 = 50.'
      },
      {
        category: 'Numerical Reasoning',
        categoryColor: 'blue',
        question: 'If 3x + 5 = 20, what is the value of x?',
        options: ['3', '4', '5', '6'],
        correct: 2,
        explanation: '3x + 5 = 20. Subtract 5 from both sides: 3x = 15. Divide by 3: x = 5.'
      },
      {
        category: 'Numerical Reasoning',
        categoryColor: 'blue',
        question: 'A shirt originally costs ₱800. If it is on sale for 30% off, what is the sale price?',
        options: ['₱240', '₱560', '₱600', '₱640'],
        correct: 1,
        explanation: '30% of ₱800 = ₱240 discount. Sale price = ₱800 - ₱240 = ₱560.'
      },
      {
        category: 'Numerical Reasoning',
        categoryColor: 'blue',
        question: 'Complete the sequence: 2, 6, 12, 20, 30, ___',
        options: ['38', '40', '42', '44'],
        correct: 2,
        explanation: 'Pattern: +4, +6, +8, +10, +12. So 30 + 12 = 42.'
      },
      {
        category: 'Numerical Reasoning',
        categoryColor: 'blue',
        question: 'If the ratio of boys to girls is 3:5 and there are 24 boys, how many girls are there?',
        options: ['30', '35', '40', '45'],
        correct: 2,
        explanation: '3:5 ratio means for every 3 boys there are 5 girls. 24÷3=8, so 8×5=40 girls.'
      },
      {
        category: 'Numerical Reasoning',
        categoryColor: 'blue',
        question: 'What is the average of 15, 20, 25, and 40?',
        options: ['20', '22', '25', '27'],
        correct: 2,
        explanation: 'Sum = 15+20+25+40 = 100. Average = 100÷4 = 25.'
      },
      {
        category: 'Numerical Reasoning',
        categoryColor: 'blue',
        question: 'A rectangle has length 15 cm and width 8 cm. What is its perimeter?',
        options: ['23 cm', '46 cm', '120 cm', '30 cm'],
        correct: 1,
        explanation: 'Perimeter = 2(length + width) = 2(15+8) = 2(23) = 46 cm.'
      },
      {
        category: 'Numerical Reasoning',
        categoryColor: 'blue',
        question: 'If 5 notebooks cost ₱125, how much do 8 notebooks cost?',
        options: ['₱180', '₱200', '₱220', '₱240'],
        correct: 1,
        explanation: 'Cost per notebook = ₱125÷5 = ₱25. So 8 notebooks = 8×₱25 = ₱200.'
      },
      {
        category: 'Numerical Reasoning',
        categoryColor: 'blue',
        question: 'What is 2³ × 2² equal to?',
        options: ['16', '32', '64', '128'],
        correct: 1,
        explanation: '2³ = 8 and 2² = 4. So 8 �� 4 = 32. Or using exponent rules: 2�� = 32.'
      },
      {
        category: 'Numerical Reasoning',
        categoryColor: 'blue',
        question: 'A train travels 240 km in 3 hours. What is its average speed?',
        options: ['60 km/h', '70 km/h', '80 km/h', '90 km/h'],
        correct: 2,
        explanation: 'Speed = Distance ÷ Time = 240 km ÷ 3 hours = 80 km/h.'
      },

      // VERBAL REASONING - ENGLISH (10 items)
      {
        category: 'Verbal Reasoning (English)',
        categoryColor: 'rose',
        question: 'Choose the word most similar to "DILIGENT":',
        options: ['Lazy', 'Hardworking', 'Careless', 'Relaxed'],
        correct: 1,
        explanation: 'Diligent means showing care and persistence, similar to hardworking.'
      },
      {
        category: 'Verbal Reasoning (English)',
        categoryColor: 'rose',
        question: 'Choose the word opposite to "ANCIENT":',
        options: ['Old', 'Modern', 'Historic', 'Traditional'],
        correct: 1,
        explanation: 'Ancient means very old, so modern (contemporary or new) is its opposite.'
      },
      {
        category: 'Verbal Reasoning (English)',
        categoryColor: 'rose',
        question: 'Complete the analogy: Doctor is to Hospital as Teacher is to ___',
        options: ['Student', 'School', 'Book', 'Classroom'],
        correct: 1,
        explanation: 'A doctor works in a hospital, just as a teacher works in a school.'
      },
      {
        category: 'Verbal Reasoning (English)',
        categoryColor: 'rose',
        question: 'Which word is spelled CORRECTLY?',
        options: ['Occassion', 'Occurence', 'Necessary', 'Seperate'],
        correct: 2,
        explanation: 'Necessary is the correct spelling. Others should be: Occasion, Occurrence, Separate.'
      },
      {
        category: 'Verbal Reasoning (English)',
        categoryColor: 'rose',
        question: 'What does "break the ice" mean?',
        options: ['To freeze water', 'To start a conversation', 'To break something', 'To feel cold'],
        correct: 1,
        explanation: '"Break the ice" is an idiom meaning to initiate conversation or ease tension in a social situation.'
      },
      {
        category: 'Verbal Reasoning (English)',
        categoryColor: 'rose',
        question: 'Which sentence has correct subject-verb agreement?',
        options: [
          'The team are playing well',
          'The team is playing well',
          'The team were playing well',
          'The team be playing well'
        ],
        correct: 1,
        explanation: '"Team" is a collective noun treated as singular, so it takes "is" not "are".'
      },
      {
        category: 'Verbal Reasoning (English)',
        categoryColor: 'rose',
        question: 'Choose the word that best completes: "She was _____ by the unexpected news."',
        options: ['shocked', 'shocking', 'shock', 'shocks'],
        correct: 0,
        explanation: '"Shocked" is the correct past participle form used as an adjective here.'
      },
      {
        category: 'Verbal Reasoning (English)',
        categoryColor: 'rose',
        question: 'What is the plural form of "analysis"?',
        options: ['Analysises', 'Analysis', 'Analyses', 'Analysies'],
        correct: 2,
        explanation: 'Words ending in -sis change to -ses in plural: analysis → analyses.'
      },
      {
        category: 'Verbal Reasoning (English)',
        categoryColor: 'rose',
        question: 'Which word means "a person who studies the stars and planets"?',
        options: ['Geologist', 'Astronomer', 'Meteorologist', 'Biologist'],
        correct: 1,
        explanation: 'An astronomer is a scientist who studies celestial objects like stars and planets.'
      },
      {
        category: 'Verbal Reasoning (English)',
        categoryColor: 'rose',
        question: 'Complete the analogy: Happy is to Joyful as Sad is to ___',
        options: ['Cheerful', 'Excited', 'Melancholy', 'Pleased'],
        correct: 2,
        explanation: 'Happy and joyful are synonyms, just as sad and melancholy are synonyms.'
      },

      // VERBAL REASONING - FILIPINO (10 items)
      {
        category: 'Verbal Reasoning (Filipino)',
        categoryColor: 'amber',
        question: 'Piliin ang salitang kasingkahulugan ng "MASAYA":',
        options: ['Malungkot', 'Maligaya', 'Galit', 'Takot'],
        correct: 1,
        explanation: 'Masaya at maligaya ay pareho ang kahulugan - kapwa nangangahulugang may saya o galak.'
      },
      {
        category: 'Verbal Reasoning (Filipino)',
        categoryColor: 'amber',
        question: 'Piliin ang salitang kasalungat ng "MABILIS":',
        options: ['Matulin', 'Mabagal', 'Mabilis', 'Magaan'],
        correct: 1,
        explanation: 'Ang kasalungat ng mabilis ay mabagal.'
      },
      {
        category: 'Verbal Reasoning (Filipino)',
        categoryColor: 'amber',
        question: 'Ano ang tamang panghalip sa pangungusap: "___ ay mag-aaral sa Unibersidad."',
        options: ['Ako', 'Ikaw', 'Siya', 'Kami'],
        correct: 2,
        explanation: 'Ang "siya" ay angkop kung nagsasalita tayo tungkol sa ibang tao (third person).'
      },
      {
        category: 'Verbal Reasoning (Filipino)',
        categoryColor: 'amber',
        question: 'Ano ang kahulugan ng idyomang "Nagdilang anghel"?',
        options: [
          'May magandang boses',
          'Natupad ang sinabi',
          'Masama ang dila',
          'Tahimik na tao'
        ],
        correct: 1,
        explanation: 'Ang "nagdilang anghel" ay nangangahulugang natupad o nangyari ang sinabi o hinula.'
      },
      {
        category: 'Verbal Reasoning (Filipino)',
        categoryColor: 'amber',
        question: 'Alin ang wastong baybay?',
        options: ['Pag-ibig', 'Pagibig', 'Pag ibig', 'Pag-Ibig'],
        correct: 0,
        explanation: 'Ang wastong baybay ay "pag-ibig" na may gitling at malaking letra sa simula lamang.'
      },
      {
        category: 'Verbal Reasoning (Filipino)',
        categoryColor: 'amber',
        question: 'Kompletuhin ang analogiya: Guro ay sa Paaralan tulad ng Doktor ay sa ___',
        options: ['Botika', 'Ospital', 'Klinika', 'Silid'],
        correct: 1,
        explanation: 'Ang guro ay nagtatrabaho sa paaralan, tulad ng doktor na nagtatrabaho sa ospital.'
      },
      {
        category: 'Verbal Reasoning (Filipino)',
        categoryColor: 'amber',
        question: 'Ano ang panlaping ginamit sa salitang "BUMILI"?',
        options: ['Um', 'Mag', 'In', 'An'],
        correct: 0,
        explanation: 'Ang unlaping "um" ay inisingit sa pagitan ng unang letra: b-um-ili.'
      },
      {
        category: 'Verbal Reasoning (Filipino)',
        categoryColor: 'amber',
        question: 'Alin ang tamang gamit ng pang-ukol?',
        options: [
          'Pumunta ako para sa bahay',
          'Pumunta ako sa bahay',
          'Pumunta ako ng bahay',
          'Pumunta ako kay bahay'
        ],
        correct: 1,
        explanation: 'Ang "sa" ay tamang pang-ukol para sa lugar o destinasyon.'
      },
      {
        category: 'Verbal Reasoning (Filipino)',
        categoryColor: 'amber',
        question: 'Ano ang uri ng pangungusap na "Kumain ka na ba?"',
        options: ['Pasalaysay', 'Patanong', 'Pakiusap', 'Padamdam'],
        correct: 1,
        explanation: 'Ang pangungusap na nagtatapos sa tandang pananong (?) ay patanong.'
      },
      {
        category: 'Verbal Reasoning (Filipino)',
        categoryColor: 'amber',
        question: 'Ano ang maramihang anyo ng "bahay"?',
        options: ['Bahays', 'Mga bahay', 'Bahayan', 'Bahay-bahay'],
        correct: 1,
        explanation: 'Sa Filipino, ang maramihan ay ginagamit ang "mga" bago ang pangngalan.'
      },

      // SPATIAL REASONING (10 items)
      {
        category: 'Spatial Reasoning',
        categoryColor: 'purple',
        question: 'If you rotate a square 90 degrees clockwise, what shape do you get?',
        options: ['Rectangle', 'Triangle', 'Square', 'Circle'],
        correct: 2,
        explanation: 'Rotating a square any amount still results in a square because all sides are equal.'
      },
      {
        category: 'Spatial Reasoning',
        categoryColor: 'purple',
        question: 'How many edges does a cube have?',
        options: ['6', '8', '10', '12'],
        correct: 3,
        explanation: 'A cube has 12 edges: 4 on top, 4 on bottom, and 4 vertical edges connecting them.'
      },
      {
        category: 'Spatial Reasoning',
        categoryColor: 'purple',
        question: 'If you fold a flat paper with 4 dots in corners into a box, how many dots will be visible?',
        options: ['0', '2', '4', 'Depends on the fold'],
        correct: 3,
        explanation: 'The number of visible dots depends on which faces are showing after folding.'
      },
      {
        category: 'Spatial Reasoning',
        categoryColor: 'purple',
        question: 'Which shape has the most lines of symmetry?',
        options: ['Rectangle', 'Square', 'Triangle', 'Pentagon'],
        correct: 1,
        explanation: 'A square has 4 lines of symmetry: 2 diagonal and 2 through midpoints of opposite sides.'
      },
      {
        category: 'Spatial Reasoning',
        categoryColor: 'purple',
        question: 'If you look at a pyramid from directly above, what shape do you see?',
        options: ['Triangle', 'Square', 'Circle', 'Rectangle'],
        correct: 1,
        explanation: 'From above, you see the base of the pyramid, which is typically a square.'
      },
      {
        category: 'Spatial Reasoning',
        categoryColor: 'purple',
        question: 'How many faces does a rectangular prism (box) have?',
        options: ['4', '5', '6', '8'],
        correct: 2,
        explanation: 'A rectangular prism has 6 faces: top, bottom, front, back, left, and right.'
      },
      {
        category: 'Spatial Reasoning',
        categoryColor: 'purple',
        question: 'Which 3D shape is formed when you rotate a triangle around one of its sides?',
        options: ['Cone', 'Cylinder', 'Sphere', 'Pyramid'],
        correct: 0,
        explanation: 'Rotating a triangle around one side forms a cone.'
      },
      {
        category: 'Spatial Reasoning',
        categoryColor: 'purple',
        question: 'If a cube is painted red on all sides and cut into 27 smaller cubes, how many small cubes have no red paint?',
        options: ['0', '1', '6', '8'],
        correct: 1,
        explanation: 'Only the center cube (1 cube) has no painted faces when a 3×3×3 cube is divided.'
      },
      {
        category: 'Spatial Reasoning',
        categoryColor: 'purple',
        question: 'Which letter looks the same when viewed in a mirror?',
        options: ['R', 'A', 'B', 'F'],
        correct: 1,
        explanation: 'The letter A has vertical symmetry and looks the same in a mirror.'
      },
      {
        category: 'Spatial Reasoning',
        categoryColor: 'purple',
        question: 'How many vertices (corners) does a triangular pyramid have?',
        options: ['3', '4', '5', '6'],
        correct: 1,
        explanation: 'A triangular pyramid has 4 vertices: 3 at the base and 1 at the apex.'
      },

      // MECHANICAL REASONING (10 items)
      {
        category: 'Mechanical Reasoning',
        categoryColor: 'cyan',
        question: 'If Gear A turns clockwise, which direction does Gear B (directly meshed with A) turn?',
        options: ['Clockwise', 'Counter-clockwise', 'Stays still', 'Cannot determine'],
        correct: 1,
        explanation: 'When two gears are meshed, they rotate in opposite directions.'
      },
      {
        category: 'Mechanical Reasoning',
        categoryColor: 'cyan',
        question: 'Which simple machine is a screwdriver an example of?',
        options: ['Lever', 'Pulley', 'Wheel and axle', 'Inclined plane'],
        correct: 2,
        explanation: 'A screwdriver is a wheel and axle where the handle is the wheel and the shaft is the axle.'
      },
      {
        category: 'Mechanical Reasoning',
        categoryColor: 'cyan',
        question: 'If you push down on one side of a seesaw, what happens to the other side?',
        options: ['Goes down', 'Goes up', 'Stays level', 'Moves sideways'],
        correct: 1,
        explanation: 'A seesaw is a lever. When one side goes down, the other side goes up.'
      },
      {
        category: 'Mechanical Reasoning',
        categoryColor: 'cyan',
        question: 'Which tool is best for lifting a heavy object with less effort?',
        options: ['Hammer', 'Crowbar', 'Saw', 'Screwdriver'],
        correct: 1,
        explanation: 'A crowbar is a lever that provides mechanical advantage for lifting heavy objects.'
      },
      {
        category: 'Mechanical Reasoning',
        categoryColor: 'cyan',
        question: 'In a pulley system, what happens when you pull down on the rope?',
        options: ['The load moves down', 'The load moves up', 'Nothing happens', 'The rope breaks'],
        correct: 1,
        explanation: 'In a simple pulley system, pulling down on one end raises the load on the other end.'
      },
      {
        category: 'Mechanical Reasoning',
        categoryColor: 'cyan',
        question: 'Why are gear teeth angled in some gears?',
        options: [
          'For decoration',
          'To make them stronger',
          'For smoother operation and less noise',
          'To make them cheaper'
        ],
        correct: 2,
        explanation: 'Angled teeth (helical gears) mesh more gradually, resulting in smoother operation and reduced noise.'
      },
      {
        category: 'Mechanical Reasoning',
        categoryColor: 'cyan',
        question: 'What is the purpose of a spring in a mechanical system?',
        options: [
          'To store and release energy',
          'To cut materials',
          'To measure weight',
          'To conduct electricity'
        ],
        correct: 0,
        explanation: 'Springs store mechanical energy when compressed or stretched and release it when returning to their original shape.'
      },
      {
        category: 'Mechanical Reasoning',
        categoryColor: 'cyan',
        question: 'If a small gear with 10 teeth drives a large gear with 30 teeth, how many times does the small gear rotate for one rotation of the large gear?',
        options: ['1 time', '2 times', '3 times', '5 times'],
        correct: 2,
        explanation: 'The gear ratio is 30:10 or 3:1, so the small gear rotates 3 times for each rotation of the large gear.'
      },
      {
        category: 'Mechanical Reasoning',
        categoryColor: 'cyan',
        question: 'What happens to friction when you oil a machine part?',
        options: ['Increases', 'Decreases', 'Stays the same', 'Disappears completely'],
        correct: 1,
        explanation: 'Oil acts as a lubricant, reducing friction between moving parts.'
      },
      {
        category: 'Mechanical Reasoning',
        categoryColor: 'cyan',
        question: 'Which of the following is NOT a simple machine?',
        options: ['Lever', 'Pulley', 'Computer', 'Inclined plane'],
        correct: 2,
        explanation: 'A computer is a complex machine. The six simple machines are: lever, pulley, wheel and axle, inclined plane, wedge, and screw.'
      },

      // PERCEPTUAL ACCURACY AND RESPONSE EFFICIENCY (PARE) (10 items)
      {
        category: 'Perceptual Accuracy (PARE)',
        categoryColor: 'emerald',
        question: 'Which pair of numbers is identical? A) 7849362 B) 7849362',
        options: ['They are identical', 'They are different', 'Cannot determine', 'Partially identical'],
        correct: 0,
        explanation: 'Both numbers are exactly the same: 7849362.'
      },
      {
        category: 'Perceptual Accuracy (PARE)',
        categoryColor: 'emerald',
        question: 'Count the letter "E" in this sequence: ENTERTAINMENT',
        options: ['2', '3', '4', '5'],
        correct: 1,
        explanation: 'The letter E appears 3 times in ENTERTAINMENT: E-nt-E-rtainm-E-nt.'
      },
      {
        category: 'Perceptual Accuracy (PARE)',
        categoryColor: 'emerald',
        question: 'Which symbol is different: ★ ★ ☆ ★ ★',
        options: ['First', 'Second', 'Third', 'All are same'],
        correct: 2,
        explanation: 'The third symbol (☆) is an outline star while others (★) are filled.'
      },
      {
        category: 'Perceptual Accuracy (PARE)',
        categoryColor: 'emerald',
        question: 'How many times does the digit "3" appear in: 33133313',
        options: ['4', '5', '6', '7'],
        correct: 2,
        explanation: 'Counting each 3: 3-3-1-3-3-3-1-3 = 6 times.'
      },
      {
        category: 'Perceptual Accuracy (PARE)',
        categoryColor: 'emerald',
        question: 'Which word is spelled differently: RECEIVE, RECIEVE, RECEIVE, RECEIVE',
        options: ['First', 'Second', 'Third', 'All same'],
        correct: 1,
        explanation: 'The second word is RECIEVE (incorrect). Correct spelling is RECEIVE (I before E except after C).'
      },
      {
        category: 'Perceptual Accuracy (PARE)',
        categoryColor: 'emerald',
        question: 'Find the pattern: 2, 4, 8, 16, ___. What comes next?',
        options: ['20', '24', '32', '36'],
        correct: 2,
        explanation: 'Each number is multiplied by 2: 2×2=4, 4×2=8, 8×2=16, 16×2=32.'
      },
      {
        category: 'Perceptual Accuracy (PARE)',
        categoryColor: 'emerald',
        question: 'Which set of parentheses is properly balanced: A) (()) B) (() C) ())',
        options: ['A only', 'B only', 'C only', 'All balanced'],
        correct: 0,
        explanation: 'Only A) (()) has matching pairs of opening and closing parentheses.'
      },
      {
        category: 'Perceptual Accuracy (PARE)',
        categoryColor: 'emerald',
        question: 'How many triangles can you find in a star (5-pointed)?',
        options: ['5', '10', '15', '20'],
        correct: 1,
        explanation: 'A 5-pointed star contains 10 triangles: 5 small points and 5 larger inner triangles.'
      },
      {
        category: 'Perceptual Accuracy (PARE)',
        categoryColor: 'emerald',
        question: 'Which line is longer? A) ————— B) —————',
        options: ['A', 'B', 'Both equal', 'Cannot tell'],
        correct: 2,
        explanation: 'Both lines are equal in length (this tests visual perception accuracy).'
      },
      {
        category: 'Perceptual Accuracy (PARE)',
        categoryColor: 'emerald',
        question: 'Spot the difference: ATTENTION vs ATENTION',
        options: ['No difference', 'One T missing', 'One T extra', 'Different words'],
        correct: 1,
        explanation: 'ATTENTION has two Ts, while ATENTION has only one T (missing a T).'
      },

      // CAREER AND OCCUPATIONAL ROLE EXPLORER (CORE) (10 items)
      {
        category: 'Career Role Explorer (CORE)',
        categoryColor: 'fuchsia',
        question: 'Which career involves designing buildings and structures?',
        options: ['Engineer', 'Architect', 'Carpenter', 'Mason'],
        correct: 1,
        explanation: 'An architect designs buildings and structures, considering aesthetics and functionality.'
      },
      {
        category: 'Career Role Explorer (CORE)',
        categoryColor: 'fuchsia',
        question: 'A person who enjoys working with numbers and finance would best suit which career?',
        options: ['Artist', 'Accountant', 'Writer', 'Chef'],
        correct: 1,
        explanation: 'Accountants work extensively with numbers, financial records, and mathematical calculations.'
      },
      {
        category: 'Career Role Explorer (CORE)',
        categoryColor: 'fuchsia',
        question: 'Which profession requires excellent communication skills and helps people with legal issues?',
        options: ['Doctor', 'Teacher', 'Lawyer', 'Nurse'],
        correct: 2,
        explanation: 'Lawyers need strong communication skills to argue cases and advise clients on legal matters.'
      },
      {
        category: 'Career Role Explorer (CORE)',
        categoryColor: 'fuchsia',
        question: 'If you enjoy caring for sick people and helping them recover, which career is suitable?',
        options: ['Veterinarian', 'Nurse', 'Pharmacist', 'Dentist'],
        correct: 1,
        explanation: 'Nurses provide direct patient care and help people recover from illness and injury.'
      },
      {
        category: 'Career Role Explorer (CORE)',
        categoryColor: 'fuchsia',
        question: 'Which career focuses on creating visual content like logos, advertisements, and websites?',
        options: ['Graphic Designer', 'Programmer', 'Journalist', 'Photographer'],
        correct: 0,
        explanation: 'Graphic designers create visual content for various media including digital and print.'
      },
      {
        category: 'Career Role Explorer (CORE)',
        categoryColor: 'fuchsia',
        question: 'A person interested in studying weather patterns and forecasting would pursue which career?',
        options: ['Geologist', 'Meteorologist', 'Astronomer', 'Oceanographer'],
        correct: 1,
        explanation: 'Meteorologists study weather patterns, atmospheric conditions, and create forecasts.'
      },
      {
        category: 'Career Role Explorer (CORE)',
        categoryColor: 'fuchsia',
        question: 'Which profession involves writing code and developing software applications?',
        options: ['IT Support', 'Software Developer', 'Data Entry', 'Network Admin'],
        correct: 1,
        explanation: 'Software developers write code and create applications, programs, and systems.'
      },
      {
        category: 'Career Role Explorer (CORE)',
        categoryColor: 'fuchsia',
        question: 'If you enjoy cooking and creating new recipes, which career path is most suitable?',
        options: ['Chef', 'Waiter', 'Restaurant Manager', 'Food Critic'],
        correct: 0,
        explanation: 'Chefs prepare food, create recipes, and manage kitchen operations.'
      },
      {
        category: 'Career Role Explorer (CORE)',
        categoryColor: 'fuchsia',
        question: 'Which career involves investigating crimes and maintaining public safety?',
        options: ['Security Guard', 'Police Officer', 'Firefighter', 'Paramedic'],
        correct: 1,
        explanation: 'Police officers investigate crimes, enforce laws, and maintain public safety.'
      },
      {
        category: 'Career Role Explorer (CORE)',
        categoryColor: 'fuchsia',
        question: 'A person who loves teaching and helping students learn would thrive in which profession?',
        options: ['Librarian', 'Teacher', 'Tutor', 'School Counselor'],
        correct: 1,
        explanation: 'Teachers educate students, develop lesson plans, and foster learning environments.'
      }
    ];

    // State
    let currentQuestion = 0;
    let userAnswers = [];
    let config = { ...defaultConfig };
    let currentCategory = 0;
    let categoryStartQuestion = 0;
    let timerInterval = null;
    let timeRemaining = 600; // 10 minutes in seconds

    // DOM Elements
    const loginScreen = document.getElementById('login-screen');
    const startScreen = document.getElementById('start-screen');
    const categoryIntroScreen = document.getElementById('category-intro-screen');
    const quizScreen = document.getElementById('quiz-screen');
    const resultsScreen = document.getElementById('results-screen');
    const reviewScreen = document.getElementById('review-screen');

    // Category colors mapping
    const categoryColors = {
      blue: { bg: 'bg-blue-500/20', text: 'text-blue-700', solid: '#3b82f6', border: 'border-blue-500' },
      rose: { bg: 'bg-rose-500/20', text: 'text-rose-700', solid: '#f43f5e', border: 'border-rose-500' },
      amber: { bg: 'bg-amber-500/20', text: 'text-amber-700', solid: '#f59e0b', border: 'border-amber-500' },
      purple: { bg: 'bg-purple-500/20', text: 'text-purple-700', solid: '#8b5cf6', border: 'border-purple-500' },
      cyan: { bg: 'bg-cyan-500/20', text: 'text-cyan-700', solid: '#06b6d4', border: 'border-cyan-500' },
      emerald: { bg: 'bg-emerald-500/20', text: 'text-emerald-700', solid: '#10b981', border: 'border-emerald-500' },
      fuchsia: { bg: 'bg-fuchsia-500/20', text: 'text-fuchsia-700', solid: '#d946ef', border: 'border-fuchsia-500' }
    };

    function showScreen(screen) {
      [loginScreen, startScreen, categoryIntroScreen, quizScreen, resultsScreen, reviewScreen].forEach(s => s.classList.add('hidden'));
      screen.classList.remove('hidden');
    }

    function formatTime(seconds) {
      const mins = Math.floor(seconds / 60);
      const secs = seconds % 60;
      return `${mins}:${secs.toString().padStart(2, '0')}`;
    }

    function startTimer() {
      if (timerInterval) clearInterval(timerInterval);
      timeRemaining = 600; // Reset to 10 minutes
      
      const timerDisplay = document.getElementById('timer-display');
      const timerText = document.getElementById('timer-text');
      
      timerInterval = setInterval(() => {
        timeRemaining--;
        timerText.textContent = formatTime(timeRemaining);
        
        // Warning when under 1 minute
        if (timeRemaining <= 60) {
          timerDisplay.classList.add('timer-warning');
          timerDisplay.style.background = 'rgba(239, 68, 68, 0.3)';
        }
        
        // Time's up
        if (timeRemaining <= 0) {
          clearInterval(timerInterval);
          moveToNextCategory();
        }
      }, 1000);
    }

    function stopTimer() {
      if (timerInterval) {
        clearInterval(timerInterval);
        timerInterval = null;
      }
    }

    function showCategoryIntro() {
      const cat = categoryDefinitions[currentCategory];
      
      document.getElementById('cat-icon').textContent = cat.icon;
      document.getElementById('cat-title').textContent = cat.name;
      document.getElementById('cat-description').textContent = cat.description;
      document.getElementById('cat-questions').textContent = cat.questions;
      document.getElementById('cat-number').textContent = currentCategory + 1;
      
      showScreen(categoryIntroScreen);
    }

    function moveToNextCategory() {
      stopTimer();
      
      // Check if there are more categories
      if (currentCategory < categoryDefinitions.length - 1) {
        currentCategory++;
        categoryStartQuestion = currentQuestion;
        showCategoryIntro();
      } else {
        // All categories done, show results
        showResults();
      }
    }

    function renderQuestion() {
      const q = questions[currentQuestion];
      const colors = categoryColors[q.categoryColor];
      
      // Update progress
      const questionInCategory = currentQuestion - categoryStartQuestion + 1;
      document.getElementById('category-progress-text').textContent = `Question ${questionInCategory} of ${categoryDefinitions[currentCategory].questions} in this section`;
      document.getElementById('overall-progress-text').textContent = `Overall: ${currentQuestion + 1}/70`;
      document.getElementById('progress-bar').style.width = `${((currentQuestion + 1) / questions.length) * 100}%`;
      
      const categoryTag = document.getElementById('category-tag');
      categoryTag.textContent = q.category;
      categoryTag.className = `category-tag inline-block px-4 py-2 rounded-full text-xs font-semibold mb-5 ${colors.bg} ${colors.text}`;
      
      document.getElementById('question-text').textContent = q.question;
      
      const optionsContainer = document.getElementById('options-container');
      optionsContainer.innerHTML = q.options.map((opt, i) => {
        const isSelected = userAnswers[currentQuestion] === i;
        const selectedClass = isSelected ? 'selected border-emerald-500 bg-emerald-50' : 'border-gray-300 hover:border-gray-400';
        return `
          <button class="option-btn w-full p-4 rounded-xl border-2 ${selectedClass} text-left text-gray-800 transition-all flex items-center gap-4 bg-white/80" data-index="${i}">
            <span class="w-9 h-9 rounded-full border-2 ${isSelected ? 'border-emerald-500 bg-emerald-500 text-white' : 'border-gray-400 text-gray-600'} flex items-center justify-center text-sm font-bold flex-shrink-0">
              ${String.fromCharCode(65 + i)}
            </span>
            <span class="font-medium">${opt}</span>
          </button>
        `;
      }).join('');
      
      // Add click handlers
      optionsContainer.querySelectorAll('.option-btn').forEach(btn => {
        btn.addEventListener('click', () => selectAnswer(parseInt(btn.dataset.index)));
      });
      
      // Update navigation buttons
      const questionInCat = currentQuestion - categoryStartQuestion;
      document.getElementById('prev-btn').disabled = questionInCat === 0;
      
      const isLastInCategory = questionInCat === categoryDefinitions[currentCategory].questions - 1;
      const isLastCategory = currentCategory === categoryDefinitions.length - 1;
      
      if (isLastInCategory && isLastCategory) {
        document.getElementById('next-btn').textContent = 'Finish Test ✓';
      } else if (isLastInCategory) {
        document.getElementById('next-btn').textContent = 'Next Section ��';
      } else {
        document.getElementById('next-btn').textContent = 'Next →';
      }
    }

    function selectAnswer(index) {
      userAnswers[currentQuestion] = index;
      renderQuestion();
    }

    function showResults() {
      stopTimer();
      showScreen(resultsScreen);
      
      const correct = userAnswers.filter((ans, i) => ans === questions[i].correct).length;
      const percentage = Math.round((correct / questions.length) * 100);
      
      document.getElementById('score-display').textContent = correct;
      document.getElementById('percentage-display').textContent = percentage + '%';
      
      // Update result icon based on score
      const iconBg = document.getElementById('result-icon-bg');
      if (percentage >= 80) {
        iconBg.style.background = 'linear-gradient(135deg, #10b981, #059669)';
      } else if (percentage >= 60) {
        iconBg.style.background = 'linear-gradient(135deg, #f59e0b, #d97706)';
      } else {
        iconBg.style.background = 'linear-gradient(135deg, #ef4444, #dc2626)';
      }
      
      // Category breakdown
      const categories = {};
      questions.forEach((q, i) => {
        if (!categories[q.category]) {
          categories[q.category] = { correct: 0, total: 0, color: q.categoryColor };
        }
        categories[q.category].total++;
        if (userAnswers[i] === q.correct) {
          categories[q.category].correct++;
        }
      });
      
      const breakdownContainer = document.getElementById('category-breakdown');
      breakdownContainer.innerHTML = Object.entries(categories).map(([cat, data]) => {
        const catPercent = Math.round((data.correct / data.total) * 100);
        const colors = categoryColors[data.color];
        return `
          <div>
            <div class="flex justify-between items-center mb-2">
              <span class="${colors.text} font-semibold">${cat}</span>
              <span class="text-gray-600 text-sm font-medium">${data.correct}/${data.total} correct (${catPercent}%)</span>
            </div>
            <div class="h-3 bg-gray-200 rounded-full overflow-hidden">
              <div class="h-full rounded-full transition-all duration-500" style="width: ${catPercent}%; background: ${colors.solid};"></div>
            </div>
          </div>
        `;
      }).join('');
    }

    function showReview() {
      showScreen(reviewScreen);
      
      const reviewContainer = document.getElementById('review-container');
      reviewContainer.innerHTML = questions.map((q, i) => {
        const userAns = userAnswers[i];
        const isCorrect = userAns === q.correct;
        const colors = categoryColors[q.categoryColor];
        
        return `
          <div class="bg-white/95 backdrop-blur-lg rounded-2xl p-6 border-2 ${isCorrect ? 'border-emerald-500' : 'border-red-500'} shadow-lg">
            <div class="flex items-start gap-4 mb-4">
              <span class="w-10 h-10 rounded-full ${isCorrect ? 'bg-emerald-500' : 'bg-red-500'} flex items-center justify-center text-white text-sm font-bold flex-shrink-0">
                ${i + 1}
              </span>
              <div class="flex-1">
                <span class="${colors.bg} ${colors.text} text-xs font-semibold px-3 py-1 rounded-full">${q.category}</span>
                <p class="text-gray-800 font-medium mt-2 text-lg">${q.question}</p>
              </div>
            </div>
            <div class="space-y-2 ml-14">
              ${q.options.map((opt, j) => {
                let optClass = 'border-gray-300 text-gray-600 bg-white';
                let icon = '';
                if (j === q.correct) {
                  optClass = 'border-emerald-500 bg-emerald-50 text-emerald-700';
                  icon = '<span class="font-bold text-emerald-600">✓</span>';
                } else if (j === userAns && !isCorrect) {
                  optClass = 'border-red-500 bg-red-50 text-red-700';
                  icon = '<span class="font-bold text-red-600">✗</span>';
                }
                return `
                  <div class="p-3 rounded-lg border-2 ${optClass} flex items-center justify-between font-medium">
                    <span>${String.fromCharCode(65 + j)}. ${opt}</span>
                    ${icon}
                  </div>
                `;
              }).join('')}
            </div>
            <div class="mt-4 ml-14 p-4 bg-blue-50 rounded-xl border border-blue-200">
              <p class="text-sm text-gray-700"><strong class="text-blue-700">💡 Explanation:</strong> ${q.explanation}</p>
            </div>
          </div>
        `;
      }).join('');
    }

    function resetQuiz() {
      currentQuestion = 0;
      userAnswers = [];
      currentCategory = 0;
      categoryStartQuestion = 0;
      stopTimer();
      showScreen(loginScreen);
    }

    // Event Listeners
    document.getElementById('login-form').addEventListener('submit', (e) => {
      e.preventDefault();
      showScreen(startScreen);
    });

    document.getElementById('start-btn').addEventListener('click', () => {
      showCategoryIntro();
    });

    document.getElementById('begin-category-btn').addEventListener('click', () => {
      showScreen(quizScreen);
      startTimer();
      renderQuestion();
    });

    document.getElementById('prev-btn').addEventListener('click', () => {
      if (currentQuestion > categoryStartQuestion) {
        currentQuestion--;
        renderQuestion();
      }
    });

    document.getElementById('next-btn').addEventListener('click', () => {
      const questionInCat = currentQuestion - categoryStartQuestion;
      const isLastInCategory = questionInCat === categoryDefinitions[currentCategory].questions - 1;
      
      if (isLastInCategory) {
        currentQuestion++;
        moveToNextCategory();
      } else {
        currentQuestion++;
        renderQuestion();
      }
    });

    document.getElementById('review-btn').addEventListener('click', showReview);
    document.getElementById('retry-btn').addEventListener('click', resetQuiz);
    document.getElementById('retry-from-review-btn').addEventListener('click', resetQuiz);
    document.getElementById('back-results-btn').addEventListener('click', () => showScreen(resultsScreen));

    // Element SDK initialization
    async function onConfigChange(cfg) {
      config = { ...defaultConfig, ...cfg };
      
      // Update text content
      const mainTitle = document.getElementById('main-title');
      const subtitle = document.getElementById('subtitle');
      
      if (mainTitle) mainTitle.textContent = config.main_title || defaultConfig.main_title;
      if (subtitle) subtitle.textContent = config.subtitle || defaultConfig.subtitle;
    }

    function mapToCapabilities(cfg) {
      return {
        recolorables: [
          {
            get: () => cfg.background_color || defaultConfig.background_color,
            set: (value) => { cfg.background_color = value; window.elementSdk.setConfig({ background_color: value }); }
          },
          {
            get: () => cfg.card_color || defaultConfig.card_color,
            set: (value) => { cfg.card_color = value; window.elementSdk.setConfig({ card_color: value }); }
          },
          {
            get: () => cfg.text_color || defaultConfig.text_color,
            set: (value) => { cfg.text_color = value; window.elementSdk.setConfig({ text_color: value }); }
          },
          {
            get: () => cfg.primary_action || defaultConfig.primary_action,
            set: (value) => { cfg.primary_action = value; window.elementSdk.setConfig({ primary_action: value }); }
          },
          {
            get: () => cfg.accent_color || defaultConfig.accent_color,
            set: (value) => { cfg.accent_color = value; window.elementSdk.setConfig({ accent_color: value }); }
          }
        ],
        borderables: [],
        fontEditable: undefined,
        fontSizeable: undefined
      };
    }

    function mapToEditPanelValues(cfg) {
      return new Map([
        ['main_title', cfg.main_title || defaultConfig.main_title],
        ['subtitle', cfg.subtitle || defaultConfig.subtitle]
      ]);
    }

    // Initialize SDK
    if (window.elementSdk) {
      window.elementSdk.init({
        defaultConfig,
        onConfigChange,
        mapToCapabilities,
        mapToEditPanelValues
      });
    }
  </script>
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9bc531a292e0fed3',t:'MTc2ODE0MjY4NS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
