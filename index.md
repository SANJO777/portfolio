---
layout: none
title: ""
---

<style>
  :root {
    --bg-light: #f7f0ff;
    --text-light: #3d0066;
    --accent-light: #b57fff;

    --bg-dark: #1a0b24;
    --text-dark: #e7dbff;
    --accent-dark: #d5aaff;
  }

  body {
    font-family: 'Segoe UI', sans-serif;
    margin: 0;
    padding: 20px;
    transition: background 0.3s, color 0.3s;
  }

  @media (prefers-color-scheme: light) {
    body {
      background-color: var(--bg-light);
      color: var(--text-light);
    }
    a {
      color: var(--accent-light);
    }
  }

  @media (prefers-color-scheme: dark) {
    body {
      background-color: var(--bg-dark);
      color: var(--text-dark);
    }
    a {
      color: var(--accent-dark);
    }
  }

  .profile-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
    text-align: center;
  }

  @media screen and (min-width: 768px) {
    .profile-container {
      flex-direction: row;
      justify-content: center;
      text-align: left;
    }
  }

  .bio p {
    max-width: 400px;
    line-height: 1.6;
  }

  .social-icons {
    display: flex;
    gap: 15px;
    margin-top: 10px;
    justify-content: center;
  }

  @media screen and (min-width: 768px) {
    .social-icons {
      justify-content: flex-start;
    }
  }

  .profile-pic {
    width: 220px;
    height: 220px;
    border-radius: 50%;
    border: 4px solid var(--accent-light);
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }

  @media (prefers-color-scheme: dark) {
    .profile-pic {
      border-color: var(--accent-dark);
    }
  }
</style>

<div class="profile-container">
  <!-- Imagen de perfil -->
  <a href="https://github.com/SANJO777" target="_blank">
    <img src="https://github.com/SANJO777.png" alt="Profile Photo" class="profile-pic">
  </a>

  <!-- Bio -->
  <div class="bio">
    <h2 style="margin: 0;">👋 Hi, I'm Santiago Rodríguez</h2>
    <p>
      🎓 I'm currently studying Information Security Engineering.<br>
      🧠 I'm passionate about solving problems as a team, always guided by the Lord (God).<br>
      💡 I truly believe that every problem has a solution —<br>
      and if it doesn't…<br>
      …it’s because the problem has already been solved. Amen! 🙏🏻
    </p>

    <!-- Redes sociales -->
    <div class="social-icons">
      <a href="https://github.com/SANJO777" target="_blank">
        <picture>
          <source srcset="https://i.imgur.com/5YhPqPu.png" media="(prefers-color-scheme: dark)">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" style="width:30px;">
        </picture>
      </a>
      <a href="https://linkedin.com/in/santiago-rodríguez-0b7476375" target="_blank">
        <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn" style="width:30px;">
      </a>
      <a href="https://instagram.com/saantiago.rodriguez" target="_blank">
        <img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" style="width:30px;">
      </a>
      <a href="https://youtube.com/@sjrpnocommentary" target="_blank">
        <img src="https://cdn-icons-png.flaticon.com/512/1384/1384060.png" alt="YouTube" style="width:30px;">
      </a>
    </div>
  </div>
</div>
