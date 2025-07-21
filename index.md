---
layout: none
title: ""
---

<style>
:root {
  --bg-light:#f7f0ff; --text-light:#3d0066; --accent-light:#b57fff;
  --bg-dark:#1a0b24; --text-dark:#e7dbff; --accent-dark:#d5aaff;
}
body {
  font-family:'Segoe UI',sans-serif;
  margin:0; padding:20px;
  background:var(--bg-light);
  color:var(--text-light);
  transition: .3s;
}
a {
  color:var(--accent-light);
  text-decoration:none;
}
@media(prefers-color-scheme:dark){
  body {
    background:var(--bg-dark);
    color:var(--text-dark);
  }
  a {
    color:var(--accent-dark);
  }
}
.profile-container {
  display:flex;
  flex-direction:column;
  align-items:center;
  gap:20px;
  text-align:center;
  max-width:800px;
  margin:0 auto 30px;
}
@media(min-width:768px){
  .profile-container {
    flex-direction:row;
    text-align:left;
    justify-content:center;
  }
}
.profile-pic {
  width:220px; height:220px;
  border-radius:50%;
  border:4px solid var(--accent-light);
  box-shadow:0 0 10px rgba(0,0,0,.1);
  flex-shrink:0;
}
@media(prefers-color-scheme:dark){
  .profile-pic {border-color:var(--accent-dark);}
}
.bio p {
  max-width:400px;
  line-height:1.6;
  margin:0;
}
.social-icons {
  display:flex;
  gap:15px;
  margin-top:10px;
  justify-content:center;
}
@media(min-width:768px){
  .social-icons {justify-content:flex-start;}
}

/* Tabs container */
.tabs {
  display:flex;
  gap:20px;
  justify-content:center;
  max-width:800px;
  margin:0 auto;
  flex-wrap:wrap;
}

/* Hide radio buttons */
.tabs input[type=radio] {
  display:none;
}

/* Style labels as tabs */
.tabs label {
  cursor:pointer;
  background:var(--accent-light);
  color:#fff;
  padding:15px 30px;
  border-radius:8px;
  flex:1 1 150px;
  text-align:center;
  font-weight:600;
  user-select:none;
  transition:.3s;
  box-shadow:0 3px 6px rgba(0,0,0,.2);
}
@media(prefers-color-scheme:dark){
  .tabs label {
    background:var(--accent-dark);
  }
}
/* Change label style when checked */
.tabs input[type=radio]:checked + label {
  background:#fff;
  color:var(--accent-light);
  box-shadow:none;
}
@media(prefers-color-scheme:dark){
  .tabs input[type=radio]:checked + label {
    background:#1a0b24;
    color:var(--accent-dark);
  }
}

/* Tab content */
.tab-content {
  max-width:800px;
  margin:20px auto 0;
  background:#fff;
  color:#000;
  padding:20px;
  border-radius:8px;
  box-shadow:0 0 10px rgba(0,0,0,.1);
  display:none;
  transition:.3s;
}
@media(prefers-color-scheme:dark){
  .tab-content {
    background:#1a0b24;
    color:var(--text-dark);
  }
}
/* Show content of checked tab */
#tab1:checked ~ .content #content1,
#tab2:checked ~ .content #content2 {
  display:block;
}
</style>

<div class="profile-container">
  <a href="https://github.com/SANJO777" target="_blank">
    <img src="https://github.com/SANJO777.png" alt="Profile Photo" class="profile-pic" />
  </a>
  <div class="bio">
    <h2 style="margin:0;">👋 Hi, I'm Santiago Rodríguez</h2>
    <p>
      🎓 I'm currently studying Information Security Engineering.<br />
      🧠 I'm passionate about solving problems as a team, always guided by the Lord (God).<br />
      💡 I truly believe that every problem has a solution —<br />
      and if it doesn't…<br />
      …it’s because the problem has already been solved. Amen! 🙏🏻
    </p>
    <div class="social-icons">
      <a href="https://github.com/SANJO777" target="_blank">
        <img src="https://i.imgur.com/POhgYus.png" alt="GitHub" style="width:30px;" />
      </a>
      <a href="https://linkedin.com/in/santiago-rodríguez-0b7476375" target="_blank">
        <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn" style="width:30px;" />
      </a>
      <a href="https://instagram.com/saantiago.rodriguez" target="_blank">
        <img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" style="width:30px;" />
      </a>
      <a href="https://youtube.com/@sjrpnocommentary" target="_blank">
        <img src="https://cdn-icons-png.flaticon.com/512/1384/1384060.png" alt="YouTube" style="width:30px;" />
      </a>
    </div>
  </div>
</div>

<div class="tabs">
  <input type="radio" id="tab1" name="tabs" checked />
  <label for="tab1">Tab 1</label>

  <input type="radio" id="tab2" name="tabs" />
  <label for="tab2">Tab 2</label>
</div>

<div class="content">
  <div id="content1" class="tab-content">
    <h3>Content for Tab 1</h3>
    <p>This is the content area for the first tab.</p>
  </div>
  <div id="content2" class="tab-content">
    <h3>Content for Tab 2</h3>
    <p>This is the content area for the second tab.</p>
  </div>
</div>
