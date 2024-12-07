<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Phantom Developer Profile</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/tailwindcss/2.2.19/tailwind.min.css" rel="stylesheet">
    <style>
        body {
            background: linear-gradient(45deg, #0a0a1a, #1a1a2e, #16213e);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            color: #e0e0e0;
            font-family: 'Arial', sans-serif;
        }
        @keyframes gradientBG {
        0% { background-position: 0% 50%; }
        50% { background-position: 100% 50%; }
        100% { background-position: 0% 50%; }
    }

    .glitch-text {
        position: relative;
        color: #00ffff;
        animation: glitch 1s infinite;
    }

    @keyframes glitch {
        2%, 64% { transform: translate(2px, 0) skew(0deg); }
        4%, 60% { transform: translate(-2px, 0) skew(0deg); }
        62% { transform: translate(0, 0) skew(5deg); }
    }

    .tech-badge {
        transition: all 0.3s ease;
        filter: brightness(0.7);
    }

    .tech-badge:hover {
        transform: scale(1.1);
        filter: brightness(1.2);
    }

    .animate-pulse-slow {
        animation: pulse 3s infinite;
    }

    @keyframes pulse {
        0%, 100% { opacity: 0.7; }
        50% { opacity: 1; }
    }
</style>
</head>
<body class="min-h-screen flex flex-col items-center justify-center p-6">
    <div class="max-w-4xl w-full bg-black bg-opacity-50 rounded-2xl shadow-2xl p-8 text-center">
        <div class="flex items-center justify-center mb-6">
            <img src="https://api.dicebear.com/7.x/personas/svg?seed=pjjj23" 
                 alt="Avatar" 
                 class="w-32 h-32 rounded-full border-4 border-cyan-500 animate-pulse-slow">
        </div>
        <h1 class="text-4xl font-bold glitch-text mb-4">Phantom Developer</h1>
    
    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mb-6">
        <div class="bg-gray-800 bg-opacity-70 p-4 rounded-lg">
            <h2 class="text-xl font-semibold text-cyan-400 mb-2">🚀 Tech Stack</h2>
            <div class="flex flex-wrap justify-center gap-2">
                <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" class="tech-badge" alt="Python">
                <img src="https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E" class="tech-badge" alt="JavaScript">
                <img src="https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white" class="tech-badge" alt="Django">
            </div>
        </div>

        <div class="bg-gray-800 bg-opacity-70 p-4 rounded-lg">
            <h2 class="text-xl font-semibold text-cyan-400 mb-2">📊 GitHub Stats</h2>
            <img src="https://github-readme-stats.vercel.app/api?username=pjjj23&theme=transparent&hide_border=true&text_color=e0e0e0&title_color=00ffff" alt="GitHub Stats" class="w-full rounded-lg">
        </div>

        <div class="bg-gray-800 bg-opacity-70 p-4 rounded-lg">
            <h2 class="text-xl font-semibold text-cyan-400 mb-2">🏆 Achievements</h2>
            <img src="https://github-profile-trophy.vercel.app/?username=pjjj23&theme=darkhub&no-frame=true&no-bg=true&margin-w=4" alt="Trophies" class="w-full rounded-lg">
        </div>
    </div>

    <div class="bg-gray-800 bg-opacity-70 p-4 rounded-lg mb-6">
        <h2 class="text-xl font-semibold text-cyan-400 mb-2">💻 Current Mission</h2>
        <p class="text-gray-300">Stealth coding | Transforming ideas into digital phantoms</p>
    </div>

    <div class="flex justify-center space-x-4">
        <a href="https://github.com/pjjj23" target="_blank" class="bg-cyan-600 hover:bg-cyan-500 text-white px-4 py-2 rounded-full transition duration-300">
            GitHub Profile
        </a>
        <div class="text-gray-500">Visitor Count: <span class="text-cyan-400">∞</span></div>
    </div>
</div>

<script>
    // Optional JavaScript for additional interactivity
    document.querySelectorAll('.tech-badge').forEach(badge => {
        badge.addEventListener('mouseenter', (e) => {
            e.target.style.transform = 'scale(1.1)';
        });
        badge.addEventListener('mouseleave', (e) => {
            e.target.style.transform = 'scale(1)';
        });
    });
</script>
</body>
</html>
