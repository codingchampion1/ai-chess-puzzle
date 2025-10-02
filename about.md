---
layout: default
title: About
---

<style>
.about-container {
  max-width: 760px;
  margin: 2rem auto 3rem auto;
  padding: 2rem 2.5rem;
  background: #f8fafc;
  border-radius: 14px;
  box-shadow: 0 2px 18px 0 rgba(0,0,0,0.08);
  font-family: 'Segoe UI', 'Arial', sans-serif;
}
.about-container h1, .about-container h2, .about-container h3 {
  color: #1e293b;
}
.about-container h1 {
  font-size: 2.2rem;
  margin-bottom: 0.35em;
  text-align: center;
  letter-spacing: -1px;
}
.about-container h2 {
  font-size: 1.35rem;
  margin-top: 2em;
  margin-bottom: 1em;
  border-left: 4px solid #2563eb;
  padding-left: 0.6em;
  background: #e0e7ff;
  border-radius: 0 6px 6px 0;
  display: flex;
  align-items: center;
  gap: 0.5em;
}
.about-container h2 .emoji {
  font-size: 1.3em;
  margin-right: 0.2em;
}
.about-container h3 {
  font-size: 1.13rem;
  margin-top: 1.7em;
}
.about-container ul, .about-container ol {
  margin-left: 1.5em;
  margin-bottom: 1em;
}
.about-container li {
  padding-bottom: 0.4em;
}
.about-container .card-section {
  background: #fff;
  border-radius: 10px;
  padding: 1.3em 1.3em 1.1em 1.3em;
  margin-bottom: 1.5em;
  border-left: 5px solid #2563eb;
  box-shadow: 0 1px 6px 0 rgba(0,0,0,0.03);
}
.about-container .muted {
  color: #64748b;
  font-size: 0.96em;
  margin-top: 0.7em;
  margin-bottom: 0.9em;
}
.about-container a {
  color: #2563eb;
  text-decoration: underline;
}
@media (max-width: 600px) {
  .about-container {
    padding: 1.2rem 0.7rem;
  }
}
</style>

<div class="about-container">

<h1>♟️ FreeChessed Puzzle AI Tutor</h1>

<div class="card-section">
  <h2><span class="emoji">🌟</span> Overview</h2>
  <p>
    <strong>FreeChessed Puzzle AI Tutor</strong> is your open-source, free chess learning companion designed for enthusiasts who want <b>in-depth, educational analysis</b> of their puzzle mistakes—<i>without</i> paying for premium subscriptions.
  </p>
  <p>
    Every missed puzzle becomes an actionable lesson: our custom AI explains <b>why</b> your move failed and what immediate counter-threat you missed—helping you improve faster, for free.
  </p>
  <ul>
    <li><strong>No subscriptions or paywalls</strong>: Powered by <a href="https://lichess.org/api" target="_blank">Lichess's free API</a> and Google's free-tier backend.</li>
    <li><strong>Instant, educational feedback</strong>: Focused on your mistake, not just the solution.</li>
    <li><strong>Easy access</strong>: Use from any browser, no installation required.</li>
  </ul>
</div>

<div class="card-section">
  <h2><span class="emoji">🛡️</span> Architecture &amp; Security</h2>
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

<div class="card-section">
  <h2><span class="emoji">🔑</span> Core Features</h2>
  <ul>
    <li><b>Tactical, actionable explanations:</b> Discover the decisive refutation to your mistake for stronger learning.</li>
    <li><b>Performance tracking (private):</b> Data helps us continuously improve the AI’s coaching ability.</li>
    <li><b>Open-source &amp; customizable:</b> Contribute or adapt the core logic to cover more chess concepts.</li>
  </ul>
</div>

<div class="card-section">
  <h2><span class="emoji">🤝</span> Contribute</h2>
  <p>
    We welcome your ideas, code, and feedback! Opportunities for contribution:
  </p>
  <ul>
    <li><b>Frontend:</b> Enhance UI/UX, visualization, or puzzle presentation.</li>
    <li><b>Backend:</b> Improve explanations and optimize analysis routines.</li>
  </ul>
  <div class="muted">
    See <a href="https://github.com/codingchampion1/ai-chess-puzzle/issues" target="_blank">open issues</a> or open a Pull Request to get involved!
  </div>
</div>

<div style="text-align:center; color:#64748b; font-size:0.98em; margin-top:2em;">
  This project is open source. <a href="https://github.com/codingchampion1/ai-chess-puzzle" target="_blank">View on GitHub</a>
</div>

</div>
