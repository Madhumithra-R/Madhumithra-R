<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Madhumithra R - Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body { 
            font-family: 'JetBrains Mono', monospace; 
            background: linear-gradient(135deg, #0f111a 0%, #1e293b 50%, #0f172a 100%);
            scroll-behavior: smooth;
        }
        .glass { 
            background: rgba(255,255,255,0.05); 
            backdrop-filter: blur(20px); 
            border: 1px solid rgba(255,255,255,0.1);
        }
        .gradient-text {
            background: linear-gradient(135deg, #8B5CF6 0%, #14B8A6 50%, #E2E8F0 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        .typing-cursor {
            display: inline-block;
            background-color: #14B8A6;
            margin-left: 3px;
            width: 3px;
            animation: blink 1s infinite;
        }
        @keyframes blink {
            0%, 50% { opacity: 1; }
            51%, 100% { opacity: 0; }
        }
        .hover-lift:hover {
            transform: translateY(-8px);
            transition: all 0.3s ease;
        }
        .pulse-glow {
            box-shadow: 0 0 20px rgba(139, 92, 246, 0.3);
            animation: pulse 2s infinite;
        }
        @keyframes pulse {
            0%, 100% { box-shadow: 0 0 20px rgba(139, 92, 246, 0.3); }
            50% { box-shadow: 0 0 40px rgba(139, 92, 246, 0.6); }
        }
    </style>
</head>
<body class="min-h-screen text-white overflow-x-hidden">

<!-- Hero Section -->
<section class="min-h-screen flex items-center justify-center py-20 px-4 relative overflow-hidden">
    <!-- Animated Background -->
    <div class="absolute inset-0">
        <div class="absolute inset-0 bg-gradient-to-br from-purple-900/20 via-blue-900/20 to-indigo-900/20"></div>
        <div class="absolute inset-0 opacity-20">
            <div class="w-72 h-72 bg-gradient-to-r from-purple-400/20 to-pink-400/20 rounded-full blur-3xl animate-pulse absolute top-20 left-10"></div>
            <div class="w-96 h-96 bg-gradient-to-r from-blue-400/20 to-cyan-400/20 rounded-full blur-3xl animate-pulse absolute bottom-40 right-20 delay-1000"></div>
        </div>
    </div>
    
    <div class="max-w-6xl mx-auto text-center relative z-10 glass p-12 rounded-3xl hover-lift">
        <!-- Profile Image -->
        <div class="w-48 h-48 bg-gradient-to-br from-purple-500 to-pink-500 rounded-full mx-auto mb-8 shadow-2xl pulse-glow">
            <i class="fas fa-user-graduate text-6xl text-white pt-16"></i>
        </div>
        
        <h1 class="text-6xl md:text-7xl font-bold mb-4 gradient-text">
            Madhumithra R
        </h1>
        <p class="text-xl md:text-2xl text-purple-300 mb-8 font-medium">
            Computer Science Engineering Student | Class of 2026
        </p>
        
        <!-- Typing Animation -->
        <div class="typing-container mb-12">
            <div class="typing-text text-2xl md:text-3xl font-semibold text-cyan-400 mb-4">
                Building innovative solutions...
                <span class="typing-cursor">|</span>
            </div>
        </div>
        
        <!-- Skills Tags -->
        <div class="flex flex-wrap justify-center gap-3 mb-12">
            <span class="px-6 py-3 bg-gradient-to-r from-purple-500/20 to-pink-500/20 backdrop-blur-sm rounded-full text-sm font-semibold border border-purple-500/30 hover:bg-purple-500/30 transition-all">Web Development</span>
            <span class="px-6 py-3 bg-gradient-to-r from-blue-500/20 to-cyan-500/20 backdrop-blur-sm rounded-full text-sm font-semibold border border-blue-500/30 hover:bg-blue-500/30 transition-all">AI/ML</span>
            <span class="px-6 py-3 bg-gradient-to-r from-emerald-500/20 to-teal-500/20 backdrop-blur-sm rounded-full text-sm font-semibold border border-emerald-500/30 hover:bg-emerald-500/30 transition-all">IoT Systems</span>
            <span class="px-6 py-3 bg-gradient-to-r from-orange-500/20 to-red-500/20 backdrop-blur-sm rounded-full text-sm font-semibold border border-orange-500/30 hover:bg-orange-500/30 transition-all">Problem Solving</span>
        </div>
        
        <!-- Social Links -->
        <div class="flex flex-wrap justify-center gap-4 mb-8">
            <a href="https://linkedin.com/in/Madhumithra-R" class="group">
                <div class="w-16 h-16 bg-gradient-to-br from-blue-600 to-blue-700 rounded-2xl flex items-center justify-center text-xl hover-lift glass backdrop-blur-sm group-hover:bg-blue-500/80 transition-all">
                    <i class="fab fa-linkedin"></i>
                </div>
            </a>
            <a href="https://github.com/Madhumithra-R" class="group">
                <div class="w-16 h-16 bg-gradient-to-br from-gray-800 to-gray-700 rounded-2xl flex items-center justify-center text-xl hover-lift glass backdrop-blur-sm group-hover:bg-gray-600/80 transition-all">
                    <i class="fab fa-github"></i>
                </div>
            </a>
            <a href="https://leetcode.com/u/Madhumithra_R/" class="group">
                <div class="w-16 h-16 bg-gradient-to-br from-yellow-500 to-orange-500 rounded-2xl flex items-center justify-center text-xl hover-lift glass backdrop-blur-sm group-hover:bg-yellow-500/80 transition-all">
                    <i class="fab fa-leetcode"></i>
                </div>
            </a>
        </div>
        
        <div class="text-sm opacity-75">
            <i class="fas fa-chart-line mr-2"></i>
            <span id="views-counter">Profile Views: Loading...</span>
        </div>
    </div>
</section>

<!-- About Section -->
<section id="about" class="py-24 px-4">
    <div class="max-w-6xl mx-auto">
        <h2 class="text-5xl font-bold text-center mb-20 gradient-text">About Me</h2>
        
        <div class="grid md:grid-cols-2 gap-12 items-center">
            <div class="glass p-10 rounded-3xl hover-lift">
                <h3 class="text-3xl font-bold mb-6 text-white">🎓 Education</h3>
                <div class="space-y-4 text-lg">
                    <div class="flex items-center">
                        <div class="w-3 h-3 bg-purple-500 rounded-full mr-4"></div>
                        <span><strong>KS Rangasamy College of Technology</strong></span>
                    </div>
                    <div>B.E. Computer Science & Engineering</div>
                    <div>CGPA: <span class="text-2xl font-bold text-cyan-400">8.5/10.0</span></div>
                    <div>Expected Graduation: <span class="text-purple-400">2026</span></div>
                </div>
            </div>
            
            <div class="grid grid-cols-2 gap-6">
                <div class="glass p-8 rounded-2xl hover-lift">
                    <div class="text-4xl mb-4"><i class="fas fa-project-diagram text-purple-400"></i></div>
                    <h4 class="font-bold mb-2">25+</h4>
                    <p>Projects</p>
                </div>
                <div class="glass p-8 rounded-2xl hover-lift">
                    <div class="text-4xl mb-4"><i class="fas fa-crown text-yellow-400"></i></div>
                    <h4 class="font-bold mb-2">5+</h4>
                    <p>Hackathons & Certs</p>
                </div>
                <div class="glass p-8 rounded-2xl hover-lift">
                    <div class="text-4xl mb-4"><i class="fas fa-code text-emerald-400"></i></div>
                    <h4 class="font-bold mb-2">200+</h4>
                    <p>LeetCode Problems</p>
                </div>
                <div class="glass p-8 rounded-2xl hover-lift">
                    <div class="text-4xl mb-4"><i class="fas fa-clock text-orange-400"></i></div>
                    <h4 class="font-bold mb-2">180+</h4>
                    <p>GitHub Days</p>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Skills Section -->
<section id="skills" class="py-24 px-4 bg-black/20">
    <div class="max-w-6xl mx-auto">
        <h2 class="text-5xl font-bold text-center mb-20 gradient-text">Tech Stack</h2>
        
        <div class="grid md:grid-cols-4 gap-8">
            <div class="glass p-8 rounded-3xl hover-lift group">
                <div class="text-5xl mb-6 text-center"><i class="fas fa-globe text-purple-400"></i></div>
                <h3 class="text-2xl font-bold mb-6 text-center">Web Development</h3>
                <div class="space-y-3 text-sm">
                    <div>React • Next.js • Tailwind</div>
                    <div>Node.js • Express • MongoDB</div>
                    <div>HTML/CSS/JS • TypeScript</div>
                </div>
            </div>
            
            <div class="glass p-8 rounded-3xl hover-lift group">
                <div class="text-5xl mb-6 text-center"><i class="fas fa-brain text-emerald-400"></i></div>
                <h3 class="text-2xl font-bold mb-6 text-center">AI/ML</h3>
                <div class="space-y-3 text-sm">
                    <div>Python • TensorFlow • PyTorch</div>
                    <div>HuggingFace • Scikit-learn</div>
                    <div>NLP • Computer Vision</div>
                </div>
            </div>
            
            <div class="glass p-8 rounded-3xl hover-lift group">
                <div class="text-5xl mb-6 text-center"><i class="fas fa-microchip text-orange-400"></i></div>
                <h3 class="text-2xl font-bold mb-6 text-center">IoT Systems</h3>
                <div class="space-y-3 text-sm">
                    <div>ESP32 • Arduino • Raspberry Pi</div>
                    <div>Sensors • MQTT • Blynk</div>
                    <div>Home Automation</div>
                </div>
            </div>
            
            <div class="glass p-8 rounded-3xl hover-lift group">
                <div class="text-5xl mb-6 text-center"><i class="fas fa-puzzle-piece text-pink-400"></i></div>
                <h3 class="text-2xl font-bold mb-6 text-center">Tools & DSA</h3>
                <div class="space-y-3 text-sm">
                    <div>Java • Python • C++</div>
                    <div>Git • Docker • Vercel</div>
                    <div>LeetCode • HackerRank</div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- CTA Section -->
<section class="py-24 px-4 text-center">
    <div class="max-w-4xl mx-auto glass p-16 rounded-3xl hover-lift">
        <h2 class="text-5xl font-bold mb-8 gradient-text">Ready to Build Something Amazing?</h2>
        <p class="text-xl mb-12 opacity-90">Open to exciting opportunities in Web Development, AI/ML, and IoT 🚀</p>
        <div class="flex flex-col sm:flex-row gap-6 justify-center">
            <a href="mailto:madhumithramithra8@gmail.com" class="px-12 py-6 bg-gradient-to-r from-purple-600 to-pink-600 rounded-2xl font-bold text-xl hover:from-purple-500 hover:to-pink-500 hover-lift transition-all shadow-2xl">
                <i class="fas fa-envelope mr-3"></i>Get In Touch
            </a>
            <a href="https://github.com/Madhumithra-R" class="px-12 py-6 border-2 border-white/30 rounded-2xl font-bold text-xl hover:bg-white/10 hover-lift transition-all backdrop-blur-sm">
                <i class="fab fa-github mr-3"></i>View GitHub
            </a>
        </div>
    </div>
</section>

<!-- Typing Animation Script -->
<script>
    const phrases = [
        "Building real-world solutions through code...",
        "Exploring AI and intelligent systems...",
        "Developing scalable web applications...",
        "Creating innovative IoT smart systems...",
        "Mastering Data Structures & Algorithms...",
        "Open to exciting opportunities!"
    ];
    let phraseIndex = 0;
    let charIndex = 0;
    let isDeleting = false;

    function typeWriter() {
        const typingElement = document.querySelector('.typing-text');
        const currentPhrase = phrases[phraseIndex];
        
        if (isDeleting) {
            typingElement.textContent = currentPhrase.substring(0, charIndex - 1) + '|';
            charIndex--;
        } else {
            typingElement.textContent = currentPhrase.substring(0, charIndex) + '|';
            charIndex++;
        }
        
        let typeSpeed = isDeleting ? 50 : 100;
        if (charIndex <= 0) {
            isDeleting = true;
            typeSpeed = 500;
        } else if (charIndex >= currentPhrase.length) {
            isDeleting = true;
            typeSpeed = 2000;
        }
        
        setTimeout(typeWriter, typeSpeed);
        
        if (!isDeleting && charIndex >= currentPhrase.length) {
            setTimeout(() => {
                isDeleting = true;
            }, 1500);
        } else if (isDeleting && charIndex <= 0) {
            phraseIndex = (phraseIndex + 1) % phrases.length;
            isDeleting = false;
        }
    }

    // Start typing animation
    document.addEventListener('DOMContentLoaded', typeWriter);

    // Smooth scrolling for anchor links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();
            document.querySelector(this.getAttribute('href')).scrollIntoView({
                behavior: 'smooth'
            });
        });
    });

    // Profile views counter (mock)
    document.getElementById('views-counter').textContent = 'Profile Views: 1,247+';
</script>

</body>
</html>
