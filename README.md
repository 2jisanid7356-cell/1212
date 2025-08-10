
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Anniversary Bubu ! 💕</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;600;700&family=Poppins:wght@300;400;500;600&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        
        .greeting-card {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 25px;
            padding: 60px 40px;
            text-align: center;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            position: relative;
            overflow: hidden;
            animation: fadeInUp 1s ease-out;
        }
        
        .greeting-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            animation: shimmer 3s infinite;
        }
        
        .main-title {
            font-family: 'Dancing Script', cursive;
            font-size: 3.5rem;
            font-weight: 700;
            color: #4a5568;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
            animation: bounceIn 1.5s ease-out;
        }
        
        .subtitle {
            font-size: 1.4rem;
            color: #667eea;
            margin-bottom: 30px;
            font-weight: 500;
            animation: fadeIn 2s ease-out;
        }
        
        .hearts-container {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 30px 0;
            animation: pulse 2s infinite;
        }
        
        .heart {
            font-size: 2rem;
            animation: heartbeat 1.5s ease-in-out infinite;
        }
        
        .heart:nth-child(1) { animation-delay: 0s; color: #ff6b6b; }
        .heart:nth-child(2) { animation-delay: 0.3s; color: #ff8e8e; }
        .heart:nth-child(3) { animation-delay: 0.6s; color: #ffb3b3; }
        .heart:nth-child(4) { animation-delay: 0.9s; color: #ff8e8e; }
        .heart:nth-child(5) { animation-delay: 1.2s; color: #ff6b6b; }
        
        .message {
            font-size: 1.1rem;
            line-height: 1.8;
            color: #4a5568;
            margin: 30px 0;
            font-weight: 400;
            animation: slideInLeft 1.8s ease-out;
        }
        
        .wishes-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin: 40px 0;
            animation: slideInRight 2s ease-out;
        }
        
        .wish-item {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 20px;
            border-radius: 15px;
            text-align: center;
            transform: translateY(0);
            transition: all 0.3s ease;
            cursor: pointer;
        }
        
        .wish-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(102, 126, 234, 0.3);
        }
        
        .wish-emoji {
            font-size: 2rem;
            display: block;
            margin-bottom: 10px;
        }
        
        .wish-text {
            font-size: 0.9rem;
            font-weight: 500;
        }
        
        .celebration-btn {
            background: linear-gradient(135deg, #ff6b6b, #ff8e8e);
            color: white;
            border: none;
            padding: 15px 40px;
            border-radius: 50px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 30px;
            box-shadow: 0 5px 15px rgba(255, 107, 107, 0.3);
            animation: fadeInUp 2.5s ease-out;
        }
        
        .celebration-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
        }
        
        .floating-hearts {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .floating-heart {
            position: absolute;
            font-size: 1.5rem;
            color: rgba(255, 107, 107, 0.6);
            animation: float 6s infinite ease-in-out;
        }
        
        .signature {
            margin-top: 40px;
            font-style: italic;
            color: #667eea;
            font-size: 1rem;
            animation: fadeIn 3s ease-out;
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes bounceIn {
            0% {
                opacity: 0;
                transform: scale(0.3);
            }
            50% {
                opacity: 1;
                transform: scale(1.05);
            }
            70% {
                transform: scale(0.9);
            }
            100% {
                opacity: 1;
                transform: scale(1);
            }
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes slideInLeft {
            from {
                opacity: 0;
                transform: translateX(-30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        @keyframes slideInRight {
            from {
                opacity: 0;
                transform: translateX(30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        @keyframes heartbeat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.2); }
        }
        
        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.7; }
        }
        
        @keyframes shimmer {
            0% { transform: translateX(-100%) translateY(-100%) rotate(45deg); }
            100% { transform: translateX(100%) translateY(100%) rotate(45deg); }
        }
        
        @keyframes float {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }
        
        @media (max-width: 768px) {
            .greeting-card {
                padding: 40px 20px;
                margin: 20px;
            }
            
            .main-title {
                font-size: 2.5rem;
            }
            
            .subtitle {
                font-size: 1.2rem;
            }
            
            .wishes-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="floating-hearts" id="floatingHearts"></div>
    
    <div class="container">
        <div class="greeting-card">
            <h1 class="main-title">Happy Anniversary!</h1>
            <p class="subtitle">To My Amazing Elder Sister 💕</p>
            
            <div class="hearts-container">
                <span class="heart">💖</span>
                <span class="heart">💕</span>
                <span class="heart">💗</span>
                <span class="heart">💕</span>
                <span class="heart">💖</span>
            </div>
            
            <div class="message">
                Dear Londoni Afa,<br><br>
                On this special day, I want to celebrate not just your marriage anniversary, 
                but also the beautiful example of love and commitment you've shown us all. 
                Your journey together has been an inspiration, filled with laughter, understanding, 
                and endless love. May your bond continue to grow stronger with each passing year!
            </div>
            
            <div class="wishes-grid">
                <div class="wish-item">
                    <span class="wish-emoji">🌹</span>
                    <div class="wish-text">May your love bloom forever like the most beautiful roses</div>
                </div>
                <div class="wish-item">
                    <span class="wish-emoji">✨</span>
                    <div class="wish-text">May every day sparkle with joy and happiness</div>
                </div>
                <div class="wish-item">
                    <span class="wish-emoji">🎉</span>
                    <div class="wish-text">Here's to many more years of celebration together</div>
                </div>
                <div class="wish-item">
                    <span class="wish-emoji">💑</span>
                    <div class="wish-text">May your partnership be blessed with endless love</div>
                </div>
            </div>
            
            <button class="celebration-btn" onclick="celebrate()">🎊 Celebrate! 🎊</button>
            
            <div class="signature">
                With all my love and best wishes,<br>
                Your loving,Jisan ❤️
            </div>
        </div>
    </div>
    
    <script>
        // Create floating hearts
        function createFloatingHeart() {
            const heart = document.createElement('div');
            heart.className = 'floating-heart';
            heart.innerHTML = ['💖', '💕', '💗', '💝', '💘'][Math.floor(Math.random() * 5)];
            heart.style.left = Math.random() * 100 + '%';
            heart.style.animationDuration = (Math.random() * 3 + 3) + 's';
            heart.style.animationDelay = Math.random() * 2 + 's';
            
            document.getElementById('floatingHearts').appendChild(heart);
            
            setTimeout(() => {
                heart.remove();
            }, 6000);
        }
        
        // Create hearts periodically
        setInterval(createFloatingHeart, 800);
        
        // Celebration function
        function celebrate() {
            // Create burst of hearts
            for (let i = 0; i < 20; i++) {
                setTimeout(() => {
                    createFloatingHeart();
                }, i * 100);
            }
            
            // Add celebration message
            const btn = document.querySelector('.celebration-btn');
            const originalText = btn.innerHTML;
            btn.innerHTML = '🎉 Celebrating Your Love! 🎉';
            btn.style.background = 'linear-gradient(135deg, #667eea, #764ba2)';
            
            setTimeout(() => {
                btn.innerHTML = originalText;
                btn.style.background = 'linear-gradient(135deg, #ff6b6b, #ff8e8e)';
            }, 3000);
        }
        
        // Add hover effects to wish items
        document.querySelectorAll('.wish-item').forEach(item => {
            item.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-5px) scale(1.02)';
            });
            
            item.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0) scale(1)';
            });
        });
        
        // Initial hearts
        for (let i = 0; i < 5; i++) {
            setTimeout(createFloatingHeart, i * 1000);
        }
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'96d1364cf4b04ea0',t:'MTc1NDg0NjkzMi4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
