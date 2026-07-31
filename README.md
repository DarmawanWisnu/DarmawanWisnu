<style>
  @import url('https://fonts.googleapis.com/css2?family=Syne:wght@600;700;800&family=JetBrains+Mono:wght@400;500;600&display=swap');

  /* =========================
     GLOBAL
     ========================= */

  .profile-container {
    width: 100%;
    max-width: 900px;
    margin: 0 auto;
    text-align: center;
  }

  /* =========================
     HERO
     ========================= */

  .hero-title {
    font-family: 'Syne', sans-serif;
    font-size: 48px;
    font-weight: 800;
    margin: 10px 0 0 0;
    background: linear-gradient(
      135deg,
      #10b981 0%,
      #06d6a0 45%,
      #06b6d4 100%
    );
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    filter: drop-shadow(0 0 14px rgba(6,182,212,0.28));
  }

  .hero-subtitle {
    font-family: 'Syne', sans-serif;
    font-size: 17px;
    font-weight: 700;
    color: #a3aeb8;
    margin-top: 10px;
    letter-spacing: 0.3px;
  }

  .rocket {
    display: inline-block;
  }

  /* =========================
     BADGES
     ========================= */

  .badges-wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 14px;
    margin-top: 24px;
    flex-wrap: wrap;
    font-family: 'JetBrains Mono', monospace;
  }

  .cyber-badge {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 7px 15px;
    border-radius: 5px;

    background: rgba(16,185,129,0.05);
    border: 1px solid rgba(16,185,129,0.35);

    color: #a3e6d3;
    font-size: 13px;
    font-weight: 600;

    box-shadow:
      0 0 12px rgba(16,185,129,0.08);
  }

  .cyber-badge.cyan {
    background: rgba(6,182,212,0.05);
    border-color: rgba(6,182,212,0.35);
    color: #93c5fd;

    box-shadow:
      0 0 12px rgba(6,182,212,0.08);
  }

  /* =========================
     STATS
     ========================= */

  .stats-wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 28px;
    font-family: 'JetBrains Mono', monospace;
  }

  .stat-label {
    padding: 8px 12px;
    background: #171b22;
    color: #d1d5db;
    font-size: 11px;
    font-weight: 600;
    letter-spacing: 0.5px;
    border: 1px solid #303640;
  }

  .stat-value {
    padding: 8px 12px;
    font-size: 12px;
    font-weight: 700;
    color: #ffffff;
  }

  .stars-value {
    background: #f59e0b;
  }

  .views-value {
    background: #10b981;
  }

  /* =========================
     CODE WINDOW
     ========================= */

  .code-window {
    margin-top: 36px;
    width: 100%;
    text-align: left;

    background: #061411;

    border: 1px solid rgba(16,185,129,0.42);
    border-radius: 16px;

    overflow: hidden;

    box-shadow:
      0 0 25px rgba(16,185,129,0.08),
      inset 0 0 35px rgba(6,182,212,0.025);
  }

  /* =========================
     WINDOW HEADER
     ========================= */

  .code-header {
    height: 42px;

    display: flex;
    align-items: center;

    padding: 0 16px;

    background: rgba(4,15,13,0.92);

    border-bottom: 1px solid rgba(16,185,129,0.18);

    font-family: 'JetBrains Mono', monospace;
  }

  .window-dots {
    display: flex;
    gap: 7px;
    align-items: center;
  }

  .dot {
    width: 11px;
    height: 11px;
    border-radius: 50%;
  }

  .dot.red {
    background: #ff5f56;
  }

  .dot.yellow {
    background: #ffbd2e;
  }

  .dot.green {
    background: #27c93f;
  }

  .filename {
    flex: 1;
    text-align: center;

    color: #6ee7b7;
    font-size: 11px;
    letter-spacing: 1px;
  }

  .status {
    color: #10b981;
    font-size: 10px;
  }

  /* =========================
     CODE BODY
     ========================= */

  .code-body {
    padding: 25px 28px;

    background:
      linear-gradient(
        90deg,
        rgba(16,185,129,0.025),
        transparent 25%,
        transparent 75%,
        rgba(6,182,212,0.025)
      );

    font-family: 'JetBrains Mono', monospace;
    font-size: 13px;
    line-height: 1.85;

    color: #d1fae5;

    overflow-x: auto;
  }

  .line {
    display: flex;
    white-space: nowrap;
  }

  .line-number {
    width: 38px;
    margin-right: 14px;

    text-align: right;

    color: #24574b;

    user-select: none;
  }

  .code {
    color: #d1fae5;
  }

  .keyword {
    color: #f472b6;
  }

  .variable {
    color: #67e8f9;
  }

  .property {
    color: #86efac;
  }

  .string {
    color: #93c5fd;
  }

  .comment {
    color: #4b756c;
  }

  .function {
    color: #fbbf24;
  }

  .operator {
    color: #a78bfa;
  }

  /* =========================
     FOOTER
     ========================= */

  .code-footer {
    display: flex;
    align-items: center;
    justify-content: space-between;

    padding: 8px 15px;

    background: rgba(3,12,10,0.95);

    border-top: 1px solid rgba(16,185,129,0.16);

    color: #397568;

    font-family: 'JetBrains Mono', monospace;
    font-size: 10px;
  }

  .footer-right {
    color: #10b981;
  }

  /* =========================
     ABOUT
     ========================= */

  .about {
    margin-top: 32px;
    padding: 20px;

    border: 1px solid #252d35;
    border-radius: 10px;

    background: rgba(13,17,23,0.45);

    text-align: center;
  }

  .about-title {
    color: #10b981;
    font-family: 'JetBrains Mono', monospace;
    font-size: 13px;
    font-weight: 600;
  }

  .about-text {
    color: #8b949e;
    font-family: 'Syne', sans-serif;
    font-size: 14px;
    line-height: 1.7;
  }

  /* =========================
     TECH STACK
     ========================= */

  .stack-title {
    margin-top: 32px;

    color: #6ee7b7;

    font-family: 'JetBrains Mono', monospace;
    font-size: 13px;
    font-weight: 600;
  }

  .stack-wrapper {
    margin-top: 14px;

    display: flex;
    justify-content: center;
    gap: 8px;
    flex-wrap: wrap;
  }

  .stack {
    padding: 6px 11px;

    border-radius: 4px;

    background: #0d1117;

    border: 1px solid #30363d;

    color: #8b949e;

    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
  }

  .stack:hover {
    border-color: #10b981;
    color: #6ee7b7;
  }

  /* =========================
     FOOT NOTE
     ========================= */

  .footer-note {
    margin-top: 28px;

    color: #484f58;

    font-family: 'JetBrains Mono', monospace;
    font-size: 10px;
  }
</style>

<div class="profile-container">

  <!-- =========================
       HERO
       ========================= -->

  <h1 class="hero-title">
    Wisnu Darmawan
  </h1>

  <div class="hero-subtitle">
    <span class="rocket">🚀</span>
    Building Data-Driven Solutions & Intelligent Systems
    <span class="rocket">🚀</span>
  </div>


  <!-- =========================
       BADGES
       ========================= -->

  <div class="badges-wrapper">

    <div class="cyber-badge">
      <span>📊</span>
      <span>Data Analyst</span>
    </div>

    <div class="cyber-badge cyan">
      <span>📍</span>
      <span>Banten, Indonesia</span>
    </div>

  </div>


  <!-- =========================
       STATS
       ========================= -->

  <div class="stats-wrapper">

    <span class="stat-label">
      ⭐ STARS
    </span>

    <span class="stat-value stars-value">
      7
    </span>

    <span class="stat-label">
      PROFILE VIEWS
    </span>

    <span class="stat-value views-value">
      3
    </span>

  </div>


  <!-- =========================
       CODE WINDOW
       ========================= -->

  <div class="code-window">

    <!-- HEADER -->

    <div class="code-header">

      <div class="window-dots">

        <span class="dot red"></span>
        <span class="dot yellow"></span>
        <span class="dot green"></span>

      </div>

      <div class="filename">
        analyst.js
      </div>

      <div class="status">
        ● status
      </div>

    </div>


    <!-- CODE -->

    <div class="code-body">

      <div class="line">
        <span class="line-number">1</span>
        <span class="code">
          <span class="keyword">const</span>
          <span class="variable"> analyst</span>
          <span class="operator"> = </span>{
        </span>
      </div>


      <div class="line">
        <span class="line-number">2</span>
        <span class="code">
          &nbsp;&nbsp;
          <span class="property">name</span>:
          <span class="string">"Wisnu Darmawan"</span>,
        </span>
      </div>


      <div class="line">
        <span class="line-number">3</span>
        <span class="code">
          &nbsp;&nbsp;
          <span class="property">role</span>:
          <span class="string">"Data Analyst"</span>,
        </span>
      </div>


      <div class="line">
        <span class="line-number">4</span>
        <span class="code">
          &nbsp;&nbsp;
          <span class="property">stack</span>:
          [
          <span class="string">"Python"</span>,
          <span class="string">"SQL"</span>,
          <span class="string">"Tableau"</span>,
          <span class="string">"Excel"</span>
          ],
        </span>
      </div>


      <div class="line">
        <span class="line-number">5</span>
        <span class="code">
          &nbsp;&nbsp;
          <span class="property">principle</span>:
          <span class="string">
            "Leveraging data to drive decisions, not guesses."
          </span>,
        </span>
      </div>


      <div class="line">
        <span class="line-number">6</span>
        <span class="code">
          &nbsp;&nbsp;
          <span class="property">focus</span>:
          <span class="string">
            "turning raw data into actionable insight"
          </span>,
        </span>
      </div>


      <div class="line">
        <span class="line-number">7</span>
        <span class="code">
          &nbsp;&nbsp;
          <span class="property">build</span>:
          <span class="function">()</span>
          <span class="operator"> =&gt; </span>{
        </span>
      </div>


      <div class="line">
        <span class="line-number">8</span>
        <span class="code">
          &nbsp;&nbsp;&nbsp;&nbsp;
          <span class="keyword">return</span>
          <span class="string">
            "data-driven solutions & intelligent systems"
          </span>;
        </span>
      </div>


      <div class="line">
        <span class="line-number">9</span>
        <span class="code">
          &nbsp;&nbsp;}
        </span>
      </div>


      <div class="line">
        <span class="line-number">10</span>
        <span class="code">
          };
        </span>
      </div>

    </div>


    <!-- FOOTER -->

    <div class="code-footer">

      <span>
        ⌁ main &nbsp; Ln 10, Col 2
      </span>

      <span class="footer-right">
        ● Live &nbsp; JavaScript
      </span>

    </div>

  </div>


  <!-- =========================
       ABOUT
       ========================= -->

  <div class="about">

    <div class="about-title">
      // about.me
    </div>

    <p class="about-text">
      Turning raw data into meaningful insights,
      practical solutions, and smarter decisions.
    </p>

  </div>


  <!-- =========================
       TECH STACK
       ========================= -->

  <div class="stack-title">
    &lt; tech_stack /&gt;
  </div>

  <div class="stack-wrapper">

    <span class="stack">Python</span>
    <span class="stack">SQL</span>
    <span class="stack">Excel</span>
    <span class="stack">Tableau</span>
    <span class="stack">Power BI</span>
    <span class="stack">Pandas</span>
    <span class="stack">PostgreSQL</span>
    <span class="stack">Git</span>

  </div>


  <div class="footer-note">
    Building with data. Learning every day. 🚀
  </div>

</div>
