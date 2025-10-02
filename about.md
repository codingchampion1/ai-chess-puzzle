---
layout: default
title: About
---

<style>
.about-container {
  max-width: 760px;
  margin: 2rem auto 3rem auto;
  font-family: 'Segoe UI', 'Arial', sans-serif;
}
.collapse-card {
  margin-bottom: 1.5em;
  border-radius: 12px;
  box-shadow: 0 1px 6px 0 rgba(0,0,0,0.04);
  overflow: hidden;
  background: #fff;
  border-left: 12px solid var(--card-color, #2563eb);
  transition: box-shadow 0.2s;
}
.collapse-card[open] {
  box-shadow: 0 4px 16px 0 rgba(0,0,0,0.08);
}
.collapse-card summary {
  cursor: pointer;
  font-size: 1.15rem;
  font-weight: bold;
  padding: 1.05em 1.2em 1.05em 1em;
  background: var(--card-bg, #e0e7ff);
  color: var(--card-color, #2563eb);
  display: flex;
  align-items: center;
  border-bottom: 1px solid #e5e7eb;
  user-select: none;
  outline: none;
  position: relative;
}
.collapse-card summary::-webkit-details-marker {
  display: none;
}
.collapse-card summary:focus {
  outline: none;
}
.collapse-card .arrow {
  width: 20px;
  height: 20px;
  display: inline-block;
  margin-right: 0.89em;
  transition: transform 0.23s;
  font-size: 1.2em;
  font-weight: bold;
  color: var(--card-color, #2563eb);
}
.collapse-card[open] .arrow {
  transform: rotate(90deg);
}
.collapse-card .card-content {
  padding: 1.2em 1.5em 1.3em 2.2em;
  font-size: 1.04rem;
  color: #1e293b;
  background: var(--card-bg, #e0e7ff);
}
.collapse-card ul {
  margin-left: 1.4em;
  margin-bottom: 1em;
}
.collapse-card ol {
  margin-left: 1.4em;
  margin-bottom: 1em;
}
.collapse-card li {
  padding-bottom: 0.35em;
}
.collapse-card .muted {
  color: #64748b;
  font-size: 0.97em;
  margin-top: 0.7em;
  margin-bottom: 0.9em;
}
@media (max-width: 600px) {
  .about-container {
    padding: 0.3rem;
  }
  .collapse-card .card-content {
    padding: 1em 0.6em 1.2em 1em;
  }
}
</style>

<div class="about-container">

<details class="collapse-card" style="--card-color: #2563eb; --card-bg: #e0e7ff;" open>
  <summary><span class="arrow">&gt;</span>🌟 Overview</summary>
  <div class="card-content">
    <strong>FreeChessed Puzzle AI Tutor</strong> is your open-source, free chess learning companion designed for enthusiasts who want <b>in-depth, educational analysis</b> of their puzzle mistakes—<i>without</i> paying for premium subscriptions.
    <br><br>
    Every missed puzzle becomes an actionable lesson: our custom AI explains <b>why</b> your move failed and what immediate counter-threat you missed—helping you improve faster, for free.
    <ul>
      <li><strong>No subscriptions or paywalls</strong>: Powered by <a href="https://lichess.org/api" target="_blank">Lichess's free API</a> and Google's free-tier backend.</li>
      <li><strong>Instant, educational feedback</strong>: Focused on your mistake, not just the solution.</li>
      <li><strong>Easy access</strong>: Use from any browser, no installation required.</li>
    </ul>
  </div>
</details>

<details class="collapse-card" style="--card-color: #f59e42; --card-bg: #fef6e6;">
  <summary><span class="arrow">&gt;</span>🛡️ Architecture &amp; Security</summary>
  <div class="card-content">
    <ol>
      <li>
        <b>Web Frontend (Public):</b> A modern, responsive web app where you solve puzzles and receive instant analysis.
      </li>
      <li>
        <b>Google Apps Script Backend (Private API):</b> Secure, serverless, and managed by the developer.
        <ul>
          <li>Keeps API keys safe</li>
          <li>Executes the custom AI logic (the “AI Tutor”)</li>
          <li>Logs user performance privately for ongoing improvement</li>
        </ul>
      </li>
    </ol>
    <div class="muted">
      <b>Privacy-first:</b> You interact only with the public site; all complex logic and private data stay secure on the backend.
    </div>
  </div>
</details>

<details class="collapse-card" style="--card-color: #10b981; --card-bg: #ecfdf5;">
  <summary><span class="arrow">&gt;</span>🔑 Core Features</summary>
  <div class="card-content">
    <ul>
      <li><b>Tactical, actionable explanations:</b> Discover the decisive refutation to your mistake for stronger learning.</li>
      <li><b>Performance tracking (private):</b> Data helps us continuously improve the AI’s coaching ability.</li>
      <li><b>Open-source &amp; customizable:</b> Contribute or adapt the core logic to cover more chess concepts.</li>
    </ul>
  </div>
</details>

<details class="collapse-card" style="--card-color: #d946ef; --card-bg: #faf5ff;">
  <summary><span class="arrow">&gt;</span>🤝 Contribute</summary>
  <div class="card-content">
    We welcome your ideas, code, and feedback! Opportunities for contribution:
    <ul>
      <li><b>Frontend:</b> Enhance UI/UX, visualization, or puzzle presentation.</li>
      <li><b>Backend:</b> Improve explanations and optimize analysis routines.</li>
    </ul>
    <div class="muted">
      See <a href="https://github.com/codingchampion1/ai-chess-puzzle/issues" target="_blank">open issues</a> or open a Pull Request to get involved!
    </div>
  </div>
</details>

<div style="text-align:center; color:#64748b; font-size:0.98em; margin-top:2em;">
  This project is open source. <a href="https://github.com/codingchampion1/ai-chess-puzzle" target="_blank">View on GitHub</a>
</div>

<script>
document.querySelectorAll('.collapse-card summary').forEach((summary) => {
  summary.addEventListener('click', function(e) {
    // toggle the arrow icon
    const arrow = summary.querySelector('.arrow');
    setTimeout(() => {
      if (summary.parentNode.open) {
        arrow.style.transform = 'rotate(90deg)';
      } else {
        arrow.style.transform = 'rotate(0deg)';
      }
    }, 10);
  });
  // Set correct direction on load if open
  if (summary.parentNode.open) {
    summary.querySelector('.arrow').style.transform = 'rotate(90deg)';
  }
});
</script>
