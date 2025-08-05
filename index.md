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
    margin:0; padding:20px;
    transition: background 0.3s, color 0.3s;
  }
  @media (prefers-color-scheme: light) {
    body {background: var(--bg-light); color: var(--text-light);}
    a {color: var(--accent-light);}
  }
  @media (prefers-color-scheme: dark) {
    body {background: var(--bg-dark); color: var(--text-dark);}
    a {color: var(--accent-dark);}
  }
  .profile-container {
    display: flex; flex-direction: column; align-items: center; gap: 20px; text-align: center;
  }
  @media (min-width: 768px) {
    .profile-container {flex-direction: row; justify-content: center; text-align: left;}
  }
  .bio p {
    max-width: 400px; line-height: 1.6;
  }
  .social-icons {
    display: flex; gap: 15px; margin-top: 10px; justify-content: center;
  }
  @media (min-width: 768px) {
    .social-icons {justify-content: flex-start;}
  }
  .profile-pic {
    width: 220px; height: 220px; border-radius: 50%;
    border: 4px solid var(--accent-light);
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
  }
  @media (prefers-color-scheme: dark) {
    .profile-pic {
      border-color: var(--accent-dark);
    }
  }
  .tabs {
    max-width: 700px;
    margin: 30px auto 0 auto;
  }
  input[type="radio"] {
    display: none;
  }
  label.tab-label {
    display: inline-block;
    background: var(--accent-light);
    color: white;
    padding: 12px 25px;
    margin-right: 5px;
    border-radius: 8px 8px 0 0;
    font-weight: bold;
    cursor: pointer;
    user-select: none;
    transition: background 0.3s;
  }
  @media (prefers-color-scheme: dark) {
    label.tab-label {
      background: var(--accent-dark);
    }
  }
  input[type="radio"]:checked + label.tab-label {
    background: var(--text-light);
    color: var(--bg-light);
  }
  @media (prefers-color-scheme: dark) {
    input[type="radio"]:checked + label.tab-label {
      background: var(--text-dark);
      color: var(--bg-dark);
    }
  }
  .tab-content {
    border: 1px solid var(--accent-light);
    border-top: none;
    padding: 20px;
    background: var(--bg-light);
    color: var(--text-light);
    border-radius: 0 0 10px 10px;
    display: none;
  }
  @media (prefers-color-scheme: dark) {
    .tab-content {
      background: var(--bg-dark);
      color: var(--text-dark);
      border-color: var(--accent-dark);
    }
  }
  #tab1:checked ~ #content1,
  #tab2:checked ~ #content2 {
    display: block;
  }
  .repo {
    display: flex;
    flex-direction: column;
    gap: 4px;
    margin-bottom: 16px;
    border-radius: 8px;
    transition: background-color 0.3s;
  }
  .repo-header {
    display: flex;
    align-items: center;
    gap: 15px;
  }
  .repo-header a {
    font-weight: 600;
    text-decoration: none;
    color: inherit;
    display: flex;
    align-items: center;
    gap: 8px;
    flex-grow: 1;
    padding: 4px 8px;
    border-radius: 8px;
    transition: background-color 0.3s, color 0.3s;
  }
  .repo-header a:hover {
    background-color: var(--accent-light);
    color: var(--bg-light);
  }
  @media (prefers-color-scheme: dark) {
    .repo-header a:hover {
      background-color: var(--accent-dark);
      color: var(--bg-dark);
    }
  }
  .repo-language {
    margin-left: auto;
    font-style: italic;
    font-size: 0.9em;
    color: var(--accent-light);
    user-select: none;
  }
  @media (prefers-color-scheme: dark) {
    .repo-language {
      color: var(--accent-dark);
    }
  }
  .repo-description {
    font-size: 0.9em;
    color: var(--text-light);
    max-width: 600px;
    margin-left: 8px;
  }
  @media (prefers-color-scheme: dark) {
    .repo-description {
      color: var(--text-dark);
    }
  }
</style>

<div class="profile-container">
  <a href="https://github.com/SANJO777" target="_blank">
    <img src="https://github.com/SANJO777.png" alt="Profile Photo" class="profile-pic">
  </a>
  <div class="bio">
    <h2 style="margin:0;">👋 Hi, I'm Santiago Rodríguez</h2>
    <p>
      🎓 I'm currently studying Information Security Engineering.<br>
      🧠 I'm passionate about solving problems as a team, always guided by the Lord (God).<br>
      💡 I truly believe that every problem has a solution —<br>
      and if it doesn't…<br>
      …it’s because the problem has already been solved. Amen! 🙏🏻
    </p>
    <div class="social-icons">
      <a href="https://github.com/SANJO777" target="_blank">
        <img src="https://i.imgur.com/POhgYus.png" alt="GitHub" style="width:30px;">
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
      <a href="https://sanjo777.github.io/linkhub/" target="_blank">
        <img src="https://cdn-icons-png.flaticon.com/512/929/929564.png" alt="LinkHub" style="width:30px;">
      </a>
    </div>
  </div>
</div>

<div class="tabs">
  <input type="radio" id="tab1" name="tab" checked>
  <label for="tab1" class="tab-label">Completed Repositories</label>

  <input type="radio" id="tab2" name="tab">
  <label for="tab2" class="tab-label">Active Repositories</label>

  <div id="content1" class="tab-content">
    <!-- No repos here yet -->
  </div>

  <div id="content2" class="tab-content">
    <div class="repo">
      <div class="repo-header">
        <a href="https://github.com/SANJO777/geometry-crush" target="_blank" rel="noopener noreferrer">
          <span>Geometry Crush</span>
        </a>
        <span class="repo-language">Godot / GDScript</span>
      </div>
      <div class="repo-description">
        This is my first video game mechanic created in Godot on mobile, inspired by the mobile game Candy Crush.
      </div>
    </div>
  </div>

    <div id="content2" class="tab-content">
    <div class="repo">
      <div class="repo-header">
        <a href="https://github.com/SANJO777/my-graphic-engine" target="_blank" rel="noopener noreferrer">
          <span>My Graphic Engine</span>
        </a>
        <span class="repo-language">Visual Studio / C++</span>
      </div>
      <div class="repo-description">
        This is my first graphic engine created with C++ on Windows 11.
      </div>
    </div>
  </div>
</div>
