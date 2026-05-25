

<style>
  @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;700&display=swap');
  * { box-sizing: border-box; margin: 0; padding: 0; }
  .wrap { font-family: 'JetBrains Mono', monospace; background: #0d1117; color: #c9d1d9; padding: 2rem; border-radius: 12px; min-height: 500px; }
  .prompt { color: #58a6ff; }
  .path { color: #3fb950; }
  .dim { color: #6e7681; }
  .white { color: #e6edf3; }
  .yellow { color: #d29922; }
  .cyan { color: #39c5cf; }
  .section-title { color: #58a6ff; font-size: 13px; margin: 1.5rem 0 0.5rem; }
  .line { display: flex; gap: 0.5rem; align-items: baseline; font-size: 13px; line-height: 1.8; }
  .badge-row { display: flex; flex-wrap: wrap; gap: 8px; margin: 0.75rem 0 0; }
  .badge { display: inline-block; padding: 3px 10px; border-radius: 4px; font-size: 11px; font-family: 'JetBrains Mono', monospace; border: 1px solid; }
  .b-blue { background: #0d2a4a; color: #58a6ff; border-color: #1f4a7c; }
  .b-green { background: #0d2a1a; color: #3fb950; border-color: #1a4a2a; }
  .b-orange { background: #2a1a0d; color: #d29922; border-color: #4a3010; }
  .b-purple { background: #1a0d2a; color: #bc8cff; border-color: #3a1f5c; }
  .b-cyan { background: #0d2a2a; color: #39c5cf; border-color: #1a4a4a; }
  .b-red { background: #2a0d0d; color: #f85149; border-color: #5c1f1f; }
  .divider { border: none; border-top: 1px solid #21262d; margin: 1.25rem 0; }
  .stats-row { display: grid; grid-template-columns: repeat(auto-fit, minmax(160px, 1fr)); gap: 10px; margin-top: 0.75rem; }
  .stat-card { background: #161b22; border: 1px solid #21262d; border-radius: 8px; padding: 12px 14px; }
  .stat-label { font-size: 11px; color: #6e7681; margin-bottom: 4px; }
  .stat-val { font-size: 18px; color: #e6edf3; font-weight: 700; }
  .cursor { display: inline-block; width: 8px; height: 14px; background: #58a6ff; animation: blink 1.1s step-end infinite; vertical-align: -2px; }
  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }
  .copy-btn { float: right; background: #21262d; border: 1px solid #30363d; color: #8b949e; border-radius: 6px; padding: 4px 10px; font-size: 11px; cursor: pointer; font-family: 'JetBrains Mono', monospace; }
  .copy-btn:hover { background: #30363d; color: #e6edf3; }
  .header-bar { display: flex; align-items: center; justify-content: space-between; margin-bottom: 1.25rem; }
  .dots { display: flex; gap: 6px; }
  .dot { width: 12px; height: 12px; border-radius: 50%; }
  .tab-label { font-size: 12px; color: #8b949e; }
</style>

<div class="wrap">
  <div class="header-bar">
    <div class="dots">
      <div class="dot" style="background:#ff5f56"></div>
      <div class="dot" style="background:#ffbd2e"></div>
      <div class="dot" style="background:#27c93f"></div>
    </div>
    <span class="tab-label">README.md — xxrin</span>
    <button class="copy-btn" onclick="copyMd()">copy markdown</button>
  </div>

  <div class="line"><span class="dim">~/github/xxrin</span> <span class="prompt">❯</span> <span class="white">cat README.md</span></div>

  <hr class="divider">

  <div class="line"><span class="yellow">▍</span><span class="white" style="font-size:15px; font-weight:700;">xxrin</span><span class="dim" style="margin-left:8px;">// backend engineer</span></div>

  <div style="margin-top: 0.75rem; font-size: 12px; line-height:1.9; color: #8b949e;">
    <div class="line"><span class="prompt">$</span><span>whoami</span></div>
    <div style="padding-left:1.25rem; color:#c9d1d9;">
      Backend engineer focused on distributed systems,<br>
      cloud infrastructure, and scalable APIs.
    </div>
  </div>

  <hr class="divider">

  <div class="section-title">// tech stack</div>

  <div style="margin-top: 0.5rem; font-size: 12px; color: #6e7681; margin-bottom: 4px;">languages &amp; frameworks</div>
  <div class="badge-row">
    <span class="badge b-blue">Python</span>
    <span class="badge b-green">Spring</span>
    <span class="badge b-orange">Node.js</span>
  </div>

  <div style="margin-top: 0.75rem; font-size: 12px; color: #6e7681; margin-bottom: 4px;">infrastructure</div>
  <div class="badge-row">
    <span class="badge b-cyan">Docker</span>
    <span class="badge b-purple">Kubernetes</span>
    <span class="badge b-blue">GCP</span>
    <span class="badge b-cyan">Azure</span>
  </div>

  <div style="margin-top: 0.75rem; font-size: 12px; color: #6e7681; margin-bottom: 4px;">databases</div>
  <div class="badge-row">
    <span class="badge b-orange">PostgreSQL</span>
    <span class="badge b-green">MySQL</span>
    <span class="badge b-red">MSSQL</span>
  </div>

  <hr class="divider">

  <div class="section-title">// github stats</div>
  <div class="stats-row">
    <div class="stat-card">
      <div class="stat-label">most used lang</div>
      <div class="stat-val" style="color:#58a6ff;">Python</div>
    </div>
    <div class="stat-card">
      <div class="stat-label">focus</div>
      <div class="stat-val" style="color:#3fb950;">Backend</div>
    </div>
    <div class="stat-card">
      <div class="stat-label">cloud</div>
      <div class="stat-val" style="color:#39c5cf;">GCP + Azure</div>
    </div>
  </div>

  <div style="margin-top: 1rem; font-size: 12px; color: #6e7681; font-style: italic;">
    ↳ stats card: <span style="color:#58a6ff;">github-readme-stats.vercel.app</span> 로 자동 연동 가능
  </div>

  <hr class="divider">

  <div class="line"><span class="dim">~/github/xxrin</span> <span class="prompt">❯</span> <span class="cursor"></span></div>
</div>

<div id="md-source" style="display:none">### 👾 xxrin — backend engineer

```
whoami: backend engineer
focus : distributed systems · cloud infra · scalable APIs
```

---

#### // tech stack

**languages & frameworks**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)

**infrastructure**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=google-cloud&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoft-azure&logoColor=white)

**databases**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MSSQL](https://img.shields.io/badge/MSSQL-CC2927?style=flat-square&logo=microsoft-sql-server&logoColor=white)

---

#### // github stats

![xxrin's GitHub stats](https://github-readme-stats.vercel.app/api?username=xxrin&show_icons=true&theme=github_dark&hide_border=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=xxrin&layout=compact&theme=github_dark&hide_border=true)
</div>

<script>
function copyMd() {
  const md = document.getElementById('md-source').innerText;
  navigator.clipboard.writeText(md).then(() => {
    const btn = document.querySelector('.copy-btn');
    btn.textContent = 'copied!';
    btn.style.color = '#3fb950';
    setTimeout(() => { btn.textContent = 'copy markdown'; btn.style.color = ''; }, 2000);
  });
}
</script>
