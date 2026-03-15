<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Syifa Ananda Sukmana - GitHub Profile</title>

<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;700&family=Poppins:wght@400;600&display=swap" rel="stylesheet">

<!-- CSS -->
<style>
    /* Global */
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Poppins', sans-serif; }
    body { 
        background: linear-gradient(135deg, #FFB6C1, #FF69B4); 
        color: #fff; 
        display: flex; flex-direction: column; align-items: center; 
        min-height: 100vh; 
    }

    h1 { font-family: 'JetBrains Mono', monospace; font-size: 3rem; text-align: center; margin-top: 2rem; text-shadow: 2px 2px #ff7eb9; }
    h2 { font-size: 2rem; margin: 2rem 0 1rem; text-align: center; }
    p { text-align: center; font-size: 1.1rem; margin-bottom: 1rem; }

    /* Typing animation */
    .typing {
        font-family: 'JetBrains Mono', monospace;
        font-size: 1.3rem;
        color: #fff;
        border-right: .1em solid #fff;
        white-space: nowrap;
        overflow: hidden;
        width: 0;
        animation: typing 3s steps(30, end) forwards, blink .75s step-end infinite;
        margin-bottom: 2rem;
    }

    @keyframes typing { from { width: 0 } to { width: 30ch; } }
    @keyframes blink { 50% { border-color: transparent; } }

    /* Profile GIF */
    .profile-gif img { border-radius: 20px; margin: 1rem 0; width: 350px; }

    /* Tech Stack */
    .tech-stack { display: flex; justify-content: center; gap: 1rem; margin: 1rem 0; }
    .tech-stack img { width: 50px; }

    /* GitHub Stats */
    .stats { display: flex; flex-wrap: wrap; justify-content: center; gap: 1rem; margin: 2rem 0; }
    .stats img { border-radius: 20px; }

    /* Footer */
    footer { margin-top: auto; margin-bottom: 2rem; font-style: italic; color: #ffe0f0; text-align: center; }

</style>
</head>
<body>

<h1>Welcome to my profile ᵔ ᵕ ᵔ</h1>
<p>Information Technology Student • Web Development</p>

<div class="typing" id="typing">const developer = "Syifa Ananda Sukmana"; let focus = "Web Development"; while(learning) { build(); improve(); }</div>

<div class="profile-gif">
    <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExNGpyeHN4aTh0NjRjbnF2NnI4MG00Mmp5ZWZpd2E1M2U3YzNwNHFpbSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/dNgK7Ws7y176U/giphy.gif" alt="Pink Laptop GIF">
</div>

<h2>About Me</h2>
<p>I am an Information Technology student learning web development & programming. I love exploring new tech, building projects, and leveling up my coding skills.</p>

<h2>Tech Stack</h2>
<div class="tech-stack">
    <img src="https://skillicons.dev/icons?i=html" alt="HTML">
    <img src="https://skillicons.dev/icons?i=css" alt="CSS">
    <img src="https://skillicons.dev/icons?i=js" alt="JavaScript">
</div>

<h2>GitHub Stats</h2>
<div class="stats" id="stats">
    <!-- Stats akan dimasukkan via JS -->
</div>

<footer>✨ Small projects today build the skills for bigger systems tomorrow ✨</footer>

<!-- JS untuk fetch stats -->
<script>
const username = "syifaananda22";

// Fungsi untuk bikin GitHub stats card
function createStatsCard(title, url) {
    const img = document.createElement('img');
    img.src = url;
    img.alt = title;
    img.height = 165;
    return img;
}

// Masukkan stats ke container
const statsContainer = document.getElementById('stats');
statsContainer.appendChild(createStatsCard("GitHub Stats", `https://github-readme-stats.vercel.app/api?username=${username}&show_icons=true&title_color=ffffff&icon_color=ffffff&text_color=ffffff&bg_color=ff69b4&hide_border=true&cache_seconds=60`));
statsContainer.appendChild(createStatsCard("Top Languages", `https://github-readme-stats.vercel.app/api/top-langs/?username=${username}&layout=compact&title_color=ffffff&text_color=ffffff&bg_color=ff69b4&hide_border=true&cache_seconds=60`));
statsContainer.appendChild(createStatsCard("Streak Stats", `https://github-readme-streak-stats.herokuapp.com/?user=${username}&ring=ffffff&fire=ffffff&currStreakLabel=ffffff&sideLabels=ffffff&dates=ffffff&hide_border=true`));
</script>

</body>
</html>
