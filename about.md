# ♟️ FreeChessed Puzzle AI Tutor

## 🌟 Overview: Your Open-Source, Free-Tier Chess Coach
The **FreeChessed Puzzle AI Tutor** is a powerful, web-hosted learning application designed for serious chess improvers who want **in-depth, educational analysis** of their puzzle mistakes **without subscribing to premium services** (like Chess.com Premium or paid cloud analysis).

This tool acts as a private, personalized coach that goes beyond simply showing the correct move. It uses a custom AI logic (running on a secure backend) to provide a structured, natural language explanation of **why your move failed** and highlights the immediate, decisive counter-threat you missed. This transforms every failed puzzle into a concise, actionable lesson, accelerating your tactical improvement entirely within a free and accessible ecosystem.

### Key Value Proposition
* **Zero Subscription Cost for Users:** Built entirely on Lichess's free API and Google's free-tier serverless services (managed by the developers).

* **Instant, Educational Feedback:** Get analysis focused on the consequences of your mistake, not just the solution.

* **Always Available:** Access the tutor directly through the web interface with no setup or installation required.

## 🎯 Architecture: Security and Efficiency
This application is built using a secure, two-part architecture to ensure fast analysis while protecting sensitive operations:

<ol>
<li> <b>Web Frontend (Public):</b> The client-side application (HTML, CSS, JavaScript) that handles the user interface, displays the puzzles, and presents the analysis report.</li>

<li> <b>Google Apps Script (GAS) Backend (Private API):</b> This component is deployed as a secure, serverless API endpoint managed by the developer. It is the project's AI Engine and Secure Vault.</li>

<ul>
<li> It <b>securely holds</b> the necessary API keys.</li>

<li> It <b>executes</b> the custom analysis logic (the "AI Tutor").</li>

<li>
  It <b>logs</b> all user performance and analysis results to a private, safe, and secure Google Sheet for system maintenance and performance review.</li>
</ul>
</ol>


**As a user, you interact only with the public website; all complex, secure logic runs seamlessly in the backend.**

## 🔑 Core Features
* **Tactical Focus:** Explanations center on the immediate, decisive refutation to your incorrect move, maximizing learning impact.

* **Performance Tracking:** All puzzle attempts are logged and analyzed to help the developers continuously improve the AI's coaching ability.

* **Customizable Logic:** The open-source nature of the AI logic allows for continuous refinement and adaptation to focus on new or specific chess concepts.

## 🤝 Contribution
Contributions are highly valued! Since the service is fully hosted, contributions are primarily focused on code quality, feature enhancements, and the core AI logic:

* **Frontend:** Improving the UI/UX, data visualization, and the presentation of the puzzle analysis.

* **Backend:** Enhancing the natural language generation (NLG) of the explanations and optimizing the Apps Script analysis routines.

If you wish to contribute, please check the project's open issues or submit a Pull Request.
