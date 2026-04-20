<!DOCTYPE html>
<html>
<head>
    <title>Happy Birthday Mahek 💖</title>

    <style>
        body {
            margin: 0;
            font-family: 'Segoe UI', sans-serif;
            text-align: center;
            background: linear-gradient(135deg, #ff758c, #ff7eb3);
            color: white;
            overflow-x: hidden;
        }

        .container {
            padding: 25px;
        }

        .title {
            font-size: 38px;
            margin-top: 30px;
        }

        .mahek {
            display: inline-block;
            font-size: 52px;
            font-weight: bold;
            overflow: hidden;
            white-space: nowrap;
            border-right: 3px solid white;
            animation: typingName 3s steps(10) forwards,
                       glow 2s infinite alternate,
                       heartbeat 1.5s infinite;
        }

        @keyframes typingName {
            from { width: 0 }
            to { width: 100% }
        }

        @keyframes glow {
            from { text-shadow: 0 0 5px #fff, 0 0 10px #ff4e75; }
            to { text-shadow: 0 0 20px #fff, 0 0 40px #ff4e75; }
        }

        @keyframes heartbeat {
            0%,100% { transform: scale(1); }
            50% { transform: scale(1.1); }
        }

        p {
            font-size: 18px;
            line-height: 1.7;
            margin: 15px;
        }

        .btn {
            background: white;
            color: #ff4e75;
            padding: 12px 25px;
            border-radius: 25px;
            border: none;
            font-size: 16px;
            cursor: pointer;
            margin-top: 20px;
        }

        .hidden {
            display: none;
            margin-top: 25px;
            animation: fadeIn 2s ease;
        }

        @keyframes fadeIn {
            from {opacity: 0;}
            to {opacity: 1;}
        }

        .heart {
            position: fixed;
            font-size: 20px;
            animation: float 6s linear infinite;
        }

        @keyframes float {
            0% {transform: translateY(100vh);}
            100% {transform: translateY(-10vh);}
        }
    </style>
</head>

<body>

<div class="container">

    <h1 class="title">
        🎉 Happy Birthday <br>
        <span class="mahek">Mahek</span> 💖
    </h1>

    <p>
        Today is not just a day… it’s the day someone truly special came into this world 💖  
        And honestly, everything feels a little more beautiful because of you.
    </p>

    <p>
        Mahek, you are not just beautiful by face 😍  
        but your nature, your kindness, your simplicity… that’s what makes you unforgettable.
    </p>

    <p>
        The way you smile, the way you talk, the way you make people feel comfortable…  
        it’s something rare and really special 🌸
    </p>

    <p>
        I feel lucky that I get to know you, talk to you, and have you in my life 💫  
        Because people like you don’t come again and again.
    </p>

    <button class="btn" onclick="startSurprise()">Click here… something special 💌</button>

    <div class="hidden" id="surprise">

        <p>
            💕 Dear Mahek 💕 <br><br>

            I don’t say this often… but today I want to say it.  
            You are honestly one of the most special people in my life.  

            It’s not just your beauty…  
            it’s your heart, your kindness, and the way you are 🌷  

            And maybe I don’t say it directly…  
            but you really mean more to me than just a friend.
        </p>

        <p>
            I just want you to stay happy always, keep smiling,  
            and never change the beautiful person you are 💖
        </p>

        <h2>🎂 Happy Birthday Again 🎂</h2>

    </div>

</div>

<!-- Music -->
<audio id="music" loop>
    <source src="https://www.bensound.com/bensound-music/bensound-romantic.mp3">
</audio>

<script>
function startSurprise() {
    document.getElementById("surprise").style.display = "block";

    // Play music
    document.getElementById("music").play();

    // Fireworks 🎆
    for(let i=0;i<30;i++){
        let fire = document.createElement("div");
        fire.innerHTML = "🎆";
        fire.style.position = "fixed";
        fire.style.left = Math.random()*100+"vw";
        fire.style.top = Math.random()*100+"vh";
        fire.style.fontSize = "24px";
        document.body.appendChild(fire);

        setTimeout(()=>fire.remove(),2000);
    }
}

// Floating hearts 💖
setInterval(()=>{
    let heart = document.createElement("div");
    heart.className="heart";
    heart.innerHTML="💖";
    heart.style.left=Math.random()*100+"vw";
    document.body.appendChild(heart);

    setTimeout(()=>heart.remove(),6000);
},500);

// Sparkles ✨
setInterval(()=>{
    let s=document.createElement("div");
    s.innerHTML="✨";
    s.style.position="fixed";
    s.style.left=Math.random()*100+"vw";
    s.style.top=Math.random()*100+"vh";
    document.body.appendChild(s);
    setTimeout(()=>s.remove(),2000);
},300);
</script>

</body>
</html>