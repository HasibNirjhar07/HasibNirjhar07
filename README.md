<!DOCTYPE html>
<html>
<head>
  <style>
    @keyframes neon {
      0%, 100% {
        text-shadow: 0 0 10px #00ff00,
                     0 0 20px #00ff00,
                     0 0 30px #00ff00;
      }
      50% {
        text-shadow: 0 0 20px #00ff00,
                     0 0 30px #00ff00,
                     0 0 40px #00ff00;
      }
    }

    @keyframes borderGlow {
      0%, 100% { border-color: #00ff00; }
      50% { border-color: #32cd32; }
    }

    @keyframes gradientBG {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      margin: 0;
      padding: 2rem;
      background: linear-gradient(-45deg, #0a0a0a, #1a1a1a, #2a2a2a, #1a1a1a);
      background-size: 400% 400%;
      animation: gradientBG 15s ease infinite;
      color: #ffffff;
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 2rem;
      background: rgba(0, 0, 0, 0.8);
      border-radius: 20px;
      border: 2px solid #00ff00;
      animation: borderGlow 2s infinite;
      box-shadow: 0 0 20px rgba(0, 255, 0, 0.2);
    }

    .header {
      text-align: center;
      margin-bottom: 2rem;
      position: relative;
    }

    .header h1 {
      font-size: 3em;
      margin: 0.5em 0;
      animation: neon 2s infinite;
      color: #fff;
    }

    .wave-gif {
      height: 35px;
      vertical-align: middle;
      margin-right: 10px;
    }

    .coding-gif {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
      margin: 1rem 0;
      box-shadow: 0 0 20px rgba(0, 255, 0, 0.3);
    }

    .badges-container {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      justify-content: center;
      margin: 1.5rem 0;
    }

    .badge {
      padding: 0.5rem 1rem;
      border-radius: 8px;
      background: rgba(0, 255, 0, 0.1);
      border: 1px solid #00ff00;
      color: #fff;
      text-decoration: none;
      transition: all 0.3s ease;
    }

    .badge:hover {
      transform: translateY(-3px);
      box-shadow: 0 0 15px rgba(0, 255, 0, 0.5);
      background: rgba(0, 255, 0, 0.2);
    }

    .section {
      margin: 2.5rem 0;
      padding: 1.5rem;
      border-radius: 10px;
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid rgba(0, 255, 0, 0.2);
      transition: all 0.3s ease;
    }

    .section:hover {
      transform: translateY(-5px);
      box-shadow: 0 5px 15px rgba(0, 255, 0, 0.2);
    }

    .section h2 {
      color: #00ff00;
      border-bottom: 2px solid #00ff00;
      padding-bottom: 0.5rem;
      margin-bottom: 1rem;
    }

    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
      gap: 1rem;
      margin: 1rem 0;
    }

    .skill-badge {
      background: linear-gradient(45deg, #1a1a1a, #2a2a2a);
      padding: 0.8rem;
      border-radius: 8px;
      text-align: center;
      border: 1px solid #00ff00;
      transition: all 0.3s ease;
    }

    .skill-badge:hover {
      transform: scale(1.05);
      box-shadow: 0 0 15px rgba(0, 255, 0, 0.3);
    }

    .stats-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1.5rem;
      margin: 2rem 0;
    }

    .stats-card {
      background: rgba(0, 0, 0, 0.5);
      padding: 1.5rem;
      border-radius: 10px;
      text-align: center;
      border: 1px solid #00ff00;
      transition: all 0.3s ease;
    }

    .stats-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 5px 15px rgba(0, 255, 0, 0.2);
    }

    .footer {
      text-align: center;
      margin-top: 3rem;
      padding-top: 2rem;
      border-top: 2px solid #00ff00;
    }

    .connect-section {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 1rem;
      margin: 2rem 0;
    }

    .connect-button {
      padding: 0.8rem 2rem;
      border-radius: 30px;
      background: linear-gradient(45deg, #00ff00, #32cd32);
      color: #000;
      text-decoration: none;
      font-weight: bold;
      transition: all 0.3s ease;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    .connect-button:hover {
      transform: translateY(-3px);
      box-shadow: 0 0 20px rgba(0, 255, 0, 0.5);
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="header">
      <img src="https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" alt="Wave" class="wave-gif">
      <h1>Hasibul Islam Nirjhar</h1>
      <h3>Aspiring Software Engineer | Student at Islamic University of Technology</h3>
      <img src="https://media.giphy.com/media/ZVik7pBtu9dNS/giphy.gif" alt="Coding" class="coding-gif">
    </div>

    <div class="badges-container">
      <a href="mailto:hasibulislam@iut-dhaka.edu" class="badge">
        📧 Email
      </a>
      <a href="https://twitter.com/NirjharHasib" class="badge">
        🐦 Twitter
      </a>
      <a href="https://www.linkedin.com/in/hasibul-islam-nirjhar-b50925262/" class="badge">
        💼 LinkedIn
      </a>
    </div>

    <div class="section">
      <h2>🚀 About Me</h2>
      <ul>
        <li>🎓 Currently studying at Islamic University of Technology</li>
        <li>💻 Passionate about software engineering and machine-learning</li>
        <li>🌱 Learning and growing in Python, C++, and C#</li>
        <li>🔍 Actively seeking software engineering internships</li>
        <li>🎮 Fun fact: I'm an avid video game enthusiast!</li>
      </ul>
    </div>

    <div class="section">
      <h2>🛠️ Skills & Tools</h2>
      <div class="skills-grid">
        <div class="skill-badge">Python</div>
        <div class="skill-badge">C++</div>
        <div class="skill-badge">C#</div>
        <div class="skill-badge">JavaScript</div>
        <div class="skill-badge">React</div>
        <div class="skill-badge">Git</div>
        <div class="skill-badge">VS Code</div>
      </div>
    </div>

    <div class="section">
      <h2>📊 GitHub Stats</h2>
      <div class="stats-container">
        <div class="stats-card">
          <h3>Profile Statistics</h3>
          <img src="https://github-readme-stats.vercel.app/api?username=HasibNirjhar07&show_icons=true&theme=radical" alt="GitHub Stats" style="max-width: 100%; height: auto;">
        </div>
        <div class="stats-card">
          <h3>Contribution Streak</h3>
          <img src="https://github-readme-streak-stats.herokuapp.com/?user=HasibNirjhar07&theme=radical" alt="GitHub Streak" style="max-width: 100%; height: auto;">
        </div>
      </div>
    </div>

    <div class="footer">
      <div class="connect-section">
        <h2>🤝 Let's Connect</h2>
        <p>I'm always excited to collaborate on interesting projects or discuss tech!</p>
        <div class="badges-container">
          <a href="https://www.linkedin.com/in/hasibul-islam-nirjhar-b50925262/" class="connect-button">Connect on LinkedIn</a>
          <a href="mailto:hasibulislam@iut-dhaka.edu" class="connect-button">Send Email</a>
        </div>
      </div>
      <p>Happy Coding! 😄</p>
    </div>
  </div>
</body>
</html>
