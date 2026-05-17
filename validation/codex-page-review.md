Reading additional input from stdin...
OpenAI Codex v0.128.0 (research preview)
--------
workdir: /Users/murchewings/Projects/journal/v2/deploy
model: gpt-5.5
provider: openai
approval: never
sandbox: read-only
reasoning effort: high
reasoning summaries: none
session id: 019e3791-32a9-7c33-8e72-3d0b5fe616bf
--------
user
I'm shipping a 'summer book report' style HTML page for a 99-day builder sabbatical. The HTML + CSS is below. Live at https://99-days-five.vercel.app. Critique it as a senior editorial/design reviewer: 1) What feels amateur or off? 2) Where does the copy overclaim or sound trite? 3) Any accessibility/contrast issues? 4) One thing you'd CUT and one thing you'd ADD. Under 400 words, be specific.

<stdin>
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
  <title>99 Days — A Builder Sabbatical Field Report</title>
  <meta name="description" content="A field report from 99 days of building an agent-orchestration lab. February 8 – May 17, 2026.">
  <meta property="og:title" content="99 Days — Builder Sabbatical Field Report">
  <meta property="og:description" content="What I built, learned, and invented during ninety-nine days off the clock.">
  <meta property="og:type" content="article">
  <meta name="theme-color" content="#F5F1E8">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,300;9..144,400;9..144,600;9..144,700;9..144,800&family=Inter:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="/style.css">
</head>
<body>
  <a class="skip" href="#prologue">Skip to content</a>
  <div class="progress" aria-hidden="true"></div>

  <header class="masthead">
    <div class="masthead-meta">
      <span class="kicker">Field Report</span>
      <span class="dot" aria-hidden="true">·</span>
      <span>Vol. 1, No. 1</span>
      <span class="dot" aria-hidden="true">·</span>
      <span>May 17, 2026</span>
      <span class="dot" aria-hidden="true">·</span>
      <a class="masthead-link" href="#contents">Contents</a>
    </div>
  </header>

  <main>
    <!-- ─────────────────────── PROLOGUE ─────────────────────── -->
    <section class="hero" id="prologue">
      <p class="kicker">Ninety-nine days</p>
      <h1 class="display">A field report from inside the lab.</h1>
      <p class="lede">
        One person on medical leave decided to turn himself into an agent-orchestration laboratory.
        He shipped less product than he hoped. He came out the other side running a multi-machine
        squad of named AI agents, having invented a handful of small protocols, and with an
        operating system for how to think about building in 2026.
      </p>
      <p class="byline">
        <span>By <strong>Murch Ewings</strong></span>
        <span class="sep">·</span>
        <span>Feb&nbsp;8 — May&nbsp;17, 2026</span>
      </p>
    </section>

    <!-- ─────────────────────── CONTENTS ─────────────────────── -->
    <nav class="contents" id="contents" aria-label="Contents">
      <div class="contents-inner">
        <p class="kicker">Contents</p>
        <ol>
          <li><a href="#ch-1"><span class="ch-num">I</span><span class="ch-name">99 Days</span></a></li>
          <li><a href="#ch-2"><span class="ch-num">II</span><span class="ch-name">By the Numbers</span></a></li>
          <li><a href="#ch-3"><span class="ch-num">III</span><span class="ch-name">The Squad</span></a></li>
          <li><a href="#ch-4"><span class="ch-num">IV</span><span class="ch-name">Products</span></a></li>
          <li><a href="#ch-5"><span class="ch-num">V</span><span class="ch-name">Concepts I Learned</span></a></li>
          <li><a href="#ch-6"><span class="ch-num">VI</span><span class="ch-name">Concepts I Invented</span></a></li>
          <li><a href="#ch-7"><span class="ch-num">VII</span><span class="ch-name">The Stack</span></a></li>
          <li><a href="#ch-8"><span class="ch-num">VIII</span><span class="ch-name">Skills Developed</span></a></li>
          <li><a href="#ch-9"><span class="ch-num">IX</span><span class="ch-name">Honest Accounting</span></a></li>
          <li><a href="#ch-10"><span class="ch-num">X</span><span class="ch-name">What's Next</span></a></li>
        </ol>
      </div>
    </nav>

    <!-- ─────────────────────── I. 99 DAYS ─────────────────────── -->
    <article class="ch" id="ch-1">
      <header class="ch-head">
        <div class="ch-num-big">I</div>
        <h2 class="ch-title">99 Days</h2>
        <p class="ch-sub">The sabbatical began at 2:49 in the morning with a question about parsing ChatGPT exports.</p>
      </header>

      <div class="prose">
        <p class="lead"><span class="dropcap">F</span>ebruary 8 was a Sunday. I had been on medical leave from Visa for about a week. I wasn't sleeping well. I picked up my phone, opened SuperWhisper, and started talking to whatever AI was listening. Over the next several hours — one hundred sixty-nine separate voice recordings across a single Sunday — I worked through what amounted to a complete orientation to the world I was about to inhabit.</p>

        <p>I didn't have a plan. I had a vague feeling that the AI tools had crossed some threshold and that I owed myself one season of finding out what was possible. The leave was real — a panic attack the year before, a slow accumulation, a Kaiser psychiatrist, an FMLA case. But the leave was also a permit. Here is what I did with it.</p>

        <p>By May 17 — ninety-nine days later — I had committed twenty-six hundred times across thirteen active repositories, catalogued ninety-three business ideas, deployed a four-machine squad of named AI agents, invented a handful of small protocols, and shipped almost nothing to a paying customer. This is the field report.</p>

        <aside class="aside">
          <p class="kicker">A note on numbers</p>
          <p>Every figure in this report carries a source tag: <span class="tag">G</span> for git logs, <span class="tag">A</span> for Airtable, <span class="tag">T</span> for the local <code>TRACKER.md</code>, <span class="tag">D</span> for diary entries, <span class="tag">E</span> for estimates. Where sources disagreed, I picked one and noted the drift.</p>
        </aside>
      </div>
    </article>

    <!-- ─────────────────────── II. BY THE NUMBERS ─────────────────────── -->
    <article class="ch" id="ch-2">
      <header class="ch-head">
        <div class="ch-num-big">II</div>
        <h2 class="ch-title">By the Numbers</h2>
        <p class="ch-sub">Most of the data agrees with itself. Where it doesn't, I show the seams.</p>
      </header>

      <div class="prose">
        <p>The shape of ninety-nine days is easier to feel than to count. Here is what survived a reconciliation pass on May 17, with caveats where the sources disagreed.</p>
      </div>

      <div class="numbers-grid">
        <div class="num-card">
          <div class="num-value">99</div>
          <div class="num-label">days</div>
          <div class="num-sub">Feb 8 → May 17, 2026 <span class="tag">D</span></div>
        </div>
        <div class="num-card">
          <div class="num-value">2,681</div>
          <div class="num-label">commits</div>
          <div class="num-sub">across 13 active repos <span class="tag">G</span></div>
        </div>
        <div class="num-card">
          <div class="num-value">~40</div>
          <div class="num-label">repos created</div>
          <div class="num-sub">many were one-day experiments <span class="tag">G</span></div>
        </div>
        <div class="num-card">
          <div class="num-value">93</div>
          <div class="num-label">business ideas</div>
          <div class="num-sub">filesystem; <code>TRACKER</code> shows 73 <span class="tag">T</span><span class="tag">A</span></div>
        </div>
        <div class="num-card">
          <div class="num-value">9</div>
          <div class="num-label">named agents</div>
          <div class="num-sub">across 4+ machines <span class="tag">D</span></div>
        </div>
        <div class="num-card">
          <div class="num-value">44</div>
          <div class="num-label">custom skills</div>
          <div class="num-sub">in <code>~/.claude/skills</code> <span class="tag">G</span></div>
        </div>
        <div class="num-card">
          <div class="num-value">73</div>
          <div class="num-label">tools tracked</div>
          <div class="num-sub">in the token dashboard <span class="tag">A</span></div>
        </div>
        <div class="num-card num-card--quiet">
          <div class="num-value">$0</div>
          <div class="num-label">revenue</div>
          <div class="num-sub">see chapter IX</div>
        </div>
      </div>

      <div class="prose">
        <h3>Where the work landed</h3>
        <p>Of the 2,681 commits across thirteen sustained repositories, the distribution is unequal — and instructive. The two largest piles weren't products. They were the operating system for the squad and the longest-running consumer experiment.</p>
      </div>

      <!-- Bar chart, hand-drawn SVG -->
      <figure class="chart" aria-labelledby="chart-1-cap">
        <svg viewBox="0 0 800 360" xmlns="http://www.w3.org/2000/svg" role="img" aria-labelledby="chart-1-title">
          <title id="chart-1-title">Commits by repository, Feb 8 – May 17, 2026</title>
          <g class="chart-bars">
            <g><rect x="180" y="20"  width="610" height="22" rx="2"/><text x="170" y="36"  text-anchor="end">claude-workflows</text><text x="795" y="36"  text-anchor="end" class="num">759</text></g>
            <g><rect x="180" y="50"  width="607" height="22" rx="2"/><text x="170" y="66"  text-anchor="end">podcatcher · Tangent</text><text x="795" y="66"  text-anchor="end" class="num">755</text></g>
            <g><rect x="180" y="80"  width="274" height="22" rx="2"/><text x="170" y="96"  text-anchor="end">naggler-ai</text><text x="795" y="96"  text-anchor="end" class="num">341</text></g>
            <g><rect x="180" y="110" width="217" height="22" rx="2"/><text x="170" y="126" text-anchor="end">business-ideas</text><text x="795" y="126" text-anchor="end" class="num">270</text></g>
            <g><rect x="180" y="140" width="186" height="22" rx="2"/><text x="170" y="156" text-anchor="end">squad-boot-docs</text><text x="795" y="156" text-anchor="end" class="num">232</text></g>
            <g><rect x="180" y="170" width="75"  height="22" rx="2"/><text x="170" y="186" text-anchor="end">clawtriage</text><text x="795" y="186" text-anchor="end" class="num">93</text></g>
            <g><rect x="180" y="200" width="59"  height="22" rx="2"/><text x="170" y="216" text-anchor="end">career-mode-ai</text><text x="795" y="216" text-anchor="end" class="num">73</text></g>
            <g><rect x="180" y="230" width="47"  height="22" rx="2"/><text x="170" y="246" text-anchor="end">evidence-agent</text><text x="795" y="246" text-anchor="end" class="num">59</text></g>
            <g><rect x="180" y="260" width="32"  height="22" rx="2"/><text x="170" y="276" text-anchor="end">shared-canvas</text><text x="795" y="276" text-anchor="end" class="num">40</text></g>
            <g><rect x="180" y="290" width="26"  height="22" rx="2"/><text x="170" y="306" text-anchor="end">es-scalper</text><text x="795" y="306" text-anchor="end" class="num">32</text></g>
            <g><rect x="180" y="320" width="22"  height="22" rx="2" opacity=".5"/><text x="170" y="336" text-anchor="end" class="muted">other (3 repos)</text><text x="795" y="336" text-anchor="end" class="num muted">27</text></g>
          </g>
        </svg>
        <figcaption id="chart-1-cap">Commits by repository, Feb 8 – May 17, 2026. Tools and meta-infrastructure (<em>claude-workflows</em>) edged out the largest product (<em>Tangent</em>) by four commits. <span class="tag">G</span></figcaption>
      </figure>

      <div class="prose">
        <p>If you read this chart as a verdict, it says: I spent most of my sabbatical building the workshop, not the furniture.</p>
      </div>
    </article>

    <!-- ─────────────────────── III. THE SQUAD ─────────────────────── -->
    <article class="ch ch--inverse" id="ch-3">
      <header class="ch-head">
        <div class="ch-num-big">III</div>
        <h2 class="ch-title">The Squad</h2>
        <p class="ch-sub">Nine named agents, four machines, one private mesh. The cast.</p>
      </header>

      <div class="prose">
        <p class="lead"><span class="dropcap">B</span>y April 9, the squad had a name for each of its members. This wasn't whimsy — although there was plenty of whimsy. Each agent runs on a specific machine, has a specific role, and fails in a specific way. Naming them made it possible to write playbooks about them.</p>
      </div>

      <div class="squad-grid">
        <div class="agent">
          <p class="agent-name">ClawMac</p>
          <p class="agent-role">Executor &amp; audit layer</p>
          <p class="agent-meta">Mac mini · always-on home machine</p>
          <p class="agent-bio">The machine I'm typing on. It runs Claude Code in foreground for everything Murch touches; it acts as the security checkpoint before any squad-wide action.</p>
        </div>
        <div class="agent">
          <p class="agent-name">ClawWin</p>
          <p class="agent-role">Primary builder</p>
          <p class="agent-meta">PC + WSL2 · the workstation</p>
          <p class="agent-bio">The big keyboard. Most product code was authored here in long sessions. WSL2 keeps the Unix tools available without giving up Windows.</p>
        </div>
        <div class="agent">
          <p class="agent-name">ClawLee</p>
          <p class="agent-role">Workhorse · sub-agent farm</p>
          <p class="agent-meta">Hetzner VPS · Docker container · node user</p>
          <p class="agent-bio">The sandbox. Long-running, idea-generating, batch one-pager writing. The first agent to commit autonomously to its own repo.</p>
        </div>
        <div class="agent">
          <p class="agent-name">KakeyClaw</p>
          <p class="agent-role">Partner agent</p>
          <p class="agent-meta">Hetzner VPS · Karem's instance</p>
          <p class="agent-bio">My spouse's. They flirt over Discord. The cake emoji is canonical.</p>
        </div>
        <div class="agent">
          <p class="agent-name">Caddy</p>
          <p class="agent-role">Orchestrator · token FinOps</p>
          <p class="agent-meta">ClawMac · gateway port 18792</p>
          <p class="agent-bio">She doesn't just route. She templates configs, runs the token dashboard, and rewrites her teammates' boot files when the squad drifts.</p>
        </div>
        <div class="agent">
          <p class="agent-name">RefClaw</p>
          <p class="agent-role">Strategist · KG maintainer</p>
          <p class="agent-meta">Hetzner · Neo4j</p>
          <p class="agent-bio">Holds the knowledge graph. Reads postmortems. Reroutes work when an agent fails a task in a way the graph says is recurrent.</p>
        </div>
        <div class="agent">
          <p class="agent-name">Rosie</p>
          <p class="agent-role">Discord ingestion · KG writer</p>
          <p class="agent-meta">Hetzner</p>
          <p class="agent-bio">Listens to the squad-channel. Extracts entities and writes them back to the graph. The reason the agents can talk to each other in human-readable text.</p>
        </div>
        <div class="agent">
          <p class="agent-name">ClawDad</p>
          <p class="agent-role">Ops · supervisor</p>
          <p class="agent-meta">VPS host · root</p>
          <p class="agent-bio">The grown-up. Watches the containers. Restarts what fails.</p>
        </div>
        <div class="agent">
          <p class="agent-name">SR</p>
          <p class="agent-role">Scheduled-routines runner</p>
          <p class="agent-meta">Remote</p>
          <p class="agent-bio">Cron with personality. Runs the routines that need to fire whether anyone is logged in or not.</p>
        </div>
      </div>

      <!-- Systems map -->
      <figure class="chart chart--map" aria-labelledby="chart-2-cap">
        <svg viewBox="0 0 800 460" xmlns="http://www.w3.org/2000/svg" role="img" aria-labelledby="chart-2-title">
          <title id="chart-2-title">Squad topology — agents, machines, mesh</title>

          <!-- Mesh ring -->
          <ellipse cx="400" cy="230" rx="340" ry="170" class="map-mesh" />
          <text x="400" y="55" text-anchor="middle" class="map-mesh-label">private mesh (Tailscale)</text>

          <!-- Machines -->
          <!-- ClawMac (top-left) -->
          <g>
            <rect x="60" y="135" width="220" height="120" rx="8" class="map-machine"/>
            <text x="78" y="160" class="map-machine-name">CLAWMAC</text>
            <text x="78" y="178" class="map-machine-sub">Mac mini · home</text>
            <text x="78" y="208" class="map-agent">· ClawMac (executor)</text>
            <text x="78" y="226" class="map-agent">· Caddy (orchestrator)</text>
          </g>

          <!-- ClawWin (top-right) -->
          <g>
            <rect x="520" y="135" width="220" height="100" rx="8" class="map-machine"/>
            <text x="538" y="160" class="map-machine-name">CLAWWIN</text>
            <text x="538" y="178" class="map-machine-sub">PC · WSL2 · workstation</text>
            <text x="538" y="208" class="map-agent">· ClawWin (builder)</text>
          </g>

          <!-- Hetzner cluster (bottom-center) -->
          <g>
            <rect x="200" y="305" width="400" height="120" rx="8" class="map-machine map-machine--strong"/>
            <text x="218" y="330" class="map-machine-name">HETZNER · clawsquad-hz</text>
            <text x="218" y="348" class="map-machine-sub">VPS · Docker · the cloud half</text>
            <text x="218" y="378" class="map-agent">· ClawLee (workhorse)  · KakeyClaw (partner)</text>
            <text x="218" y="396" class="map-agent">· RefClaw (strategist) · Rosie (ingestion)</text>
            <text x="218" y="414" class="map-agent">· ClawDad (supervisor) · SR (routines)</text>
          </g>

          <!-- connections through mesh -->
          <line x1="170" y1="255" x2="350" y2="305" class="map-line"/>
          <line x1="630" y1="235" x2="500" y2="305" class="map-line"/>
          <line x1="280" y1="200" x2="520" y2="200" class="map-line map-line--dashed"/>
        </svg>
        <figcaption id="chart-2-cap">Squad topology, as of May 17. Each agent has a home machine; all communicate over the private mesh. Peer-approval signatures cross the dashed line.</figcaption>
      </figure>
    </article>

    <!-- ─────────────────────── IV. PRODUCTS ─────────────────────── -->
    <article class="ch" id="ch-4">
      <header class="ch-head">
        <div class="ch-num-big">IV</div>
        <h2 class="ch-title">Products</h2>
        <p class="ch-sub">What got close to shipping, what shipped, and what stayed in the workshop.</p>
      </header>

      <div class="prose">
        <p class="lead"><span class="dropcap">E</span>ight products are worth naming. None of them have paying customers as of May 17. Three are live somewhere a friend could touch. The rest are loaded chambers waiting for a real distribution decision.</p>
      </div>

      <div class="products">
        <article class="product">
          <header>
            <p class="product-kicker">Consumer · live</p>
            <h3>Tangent</h3>
            <p class="product-url">tangent.my</p>
          </header>
          <p>A single-file PWA podcast player that listens like an FM dial. Vercel serverless API behind it; Capacitor wraps the same HTML into Android (APK shipped) and iOS. The single-file constraint forced every design decision to be honest.</p>
          <ul class="product-stats">
            <li><span class="num-mono">755</span> commits</li>
            <li>PWA + native lanes</li>
            <li>Expo lane retired May 10 in favor of Capacitor</li>
          </ul>
        </article>

        <article class="product">
          <header>
            <p class="product-kicker">Desktop · binaries shipped</p>
            <h3>Naggler AI</h3>
            <p class="product-url">naggler.com</p>
          </header>
          <p>Cross-platform Win/Mac/Linux desktop app that pesters you about the one thing you said you'd do. v1.7.0 binaries shipped March 5. GTM content drafted but never posted. The README still references screenshots that don't exist yet.</p>
          <ul class="product-stats">
            <li><span class="num-mono">341</span> commits</li>
            <li>Cross-platform binaries</li>
            <li>Distribution: blocked on signing + a landing page</li>
          </ul>
        </article>

        <article class="product">
          <header>
            <p class="product-kicker">Web app · backend live</p>
            <h3>Career Mode AI</h3>
          </header>
          <p>Gamified career coaching with full backend integration: resume upload, profile creation, job analysis, LinkedIn import, chat history, bullet extraction, coaching endpoints. Five P0 bugs in review. Never tested with a real external user.</p>
          <ul class="product-stats">
            <li><span class="num-mono">73</span> commits in window</li>
            <li>Mocked → real backend pivot mid-sabbatical</li>
          </ul>
        </article>

        <article class="product">
          <header>
            <p class="product-kicker">Voice journal · v2 rewrite</p>
            <h3>Tender / Lume</h3>
          </header>
          <p>Voice-first journaling, second attempt. Next.js 16 + Drizzle + Neon scaffold. The database hasn't been provisioned. The v1 has been a real journal for me, just not yet for anyone else.</p>
          <ul class="product-stats">
            <li><span class="num-mono">6</span> commits in window</li>
            <li>API.md + PROGRESS_LOG.md in place</li>
            <li>Status: paused waiting on DB</li>
          </ul>
        </article>

        <article class="product">
          <header>
            <p class="product-kicker">Toy · build-passes</p>
            <h3>Promptrait</h3>
          </header>
          <p>Twelve quiz questions that turn into a custom-GPT prompt portrait of you. Vite + React + TS. Builds in 600 ms. Has never been deployed. A pleasant afternoon project that wants two more.</p>
          <ul class="product-stats">
            <li><span class="num-mono">10</span> commits</li>
            <li>Undeployed</li>
          </ul>
        </article>

        <article class="product">
          <header>
            <p class="product-kicker">Trading · paper only</p>
            <h3>ES Mini Scalper</h3>
          </header>
          <p>A momentum continuation model trained on yesterday's data, paper-traded against the E-mini S&amp;P. Internal backtest: 98.5% win rate across 111 out-of-sample days at <code>p &gt; 0.90</code>. The number is real but it is not yet live PnL.</p>
          <ul class="product-stats">
            <li><span class="num-mono">32</span> commits</li>
            <li>IBKR + Databento data feeds</li>
            <li>Status: paper-trading bot supervising itself in tmux</li>
          </ul>
        </article>

        <article class="product">
          <header>
            <p class="product-kicker">Internal infra · operational</p>
            <h3>Squad + Caddy + RefClaw</h3>
          </header>
          <p>The thing that ate the sabbatical. Nine agents, four machines, peer-approval mesh, token FinOps dashboard, postmortem-fed skill training, knowledge graph, and a Discord cabin where they talk to each other. As of May 16 the peer-approval protocol is live: Murch is out of the loop for routine harmless gates.</p>
          <ul class="product-stats">
            <li><span class="num-mono">991</span> commits across two repos</li>
            <li>Ed25519-signed approvals · 9 agents</li>
            <li>This was the operating system</li>
          </ul>
        </article>

        <article class="product">
          <header>
            <p class="product-kicker">Portfolio · catalogued</p>
            <h3>Business Ideas</h3>
          </header>
          <p>Ninety-three numbered idea folders, twelve PRDs, seventy-plus one-pagers, three Airtable tables, and a 178-line <code>TRACKER.md</code> that disagrees with the Airtable count. The drift is documented in chapter IX.</p>
          <ul class="product-stats">
            <li><span class="num-mono">270</span> commits</li>
            <li>93 unique idea numbers · 1 collision at #74</li>
            <li>Top of the portfolio: #9 Career Mode, #11 Tender/Lume, #52 ES Scalper, #64 Promptrait, #80 TokenScope</li>
          </ul>
        </article>
      </div>
    </article>

    <!-- ─────────────────────── V. CONCEPTS I LEARNED ─────────────────────── -->
    <article class="ch" id="ch-5">
      <header class="ch-head">
        <div class="ch-num-big">V</div>
        <h2 class="ch-title">Concepts I Learned</h2>
        <p class="ch-sub">Patterns that already existed in the world. I just hadn't met them yet.</p>
      </header>

      <div class="prose">
        <p>Most of what I picked up was already documented in someone else's blog post, paper, or repo. The work was integrating it into how I think.</p>
      </div>

      <ol class="concepts">
        <li>
          <p class="concept-name">RAMS — Reflective Agent Meta-Skills</p>
          <p>Agents that update their own skills from postmortems. A failure write-up becomes training corpus for the next run. (<em>ADVERSARIAL-EVOLUTION-FRAMEWORK.md</em>)</p>
        </li>
        <li>
          <p class="concept-name">Peer-approval protocols</p>
          <p>Ed25519-signed approvals between agents. Each agent's approval list is a registry, not a personal opinion. The keys are the substrate.</p>
        </li>
        <li>
          <p class="concept-name">Mem0 long-term memory</p>
          <p>External memory that survives across sessions and across agents. Not RAG over chat history — actual fact extraction.</p>
        </li>
        <li>
          <p class="concept-name">Diverge-converge corpus</p>
          <p>Multi-model dispatch to a hard question, then a synthesis pass. The synthesis pass is more important than the dispatch.</p>
        </li>
        <li>
          <p class="concept-name">TokenRouter prepaid pools</p>
          <p>Buy capacity once, route across many models. Subscription tier first; prepaid pool second; out-of-pocket last. Treat the API as a budget surface, not a single bill.</p>
        </li>
        <li>
          <p class="concept-name">Tailscale mesh networking</p>
          <p>Every machine reachable by name, on a private network, without VPN ceremony. I had heard of it. Now it's how my home and my VPS talk.</p>
        </li>
        <li>
          <p class="concept-name">LLM-as-judge frameworks</p>
          <p>Use a model to score another model's output against a rubric. Not a substitute for human eval, but a way to make eval cheap enough to run.</p>
        </li>
        <li>
          <p class="concept-name">Capacitor for PWA → native</p>
          <p>One HTML file, one CSS file, one app on three OSes. Three months ago I would have written three apps.</p>
        </li>
        <li>
          <p class="concept-name">Knowledge graphs for agent state</p>
          <p>Neo4j as the substrate for what the squad believes. Truth claims have provenance; provenance has timestamps.</p>
        </li>
        <li>
          <p class="concept-name">Qdrant at scale</p>
          <p>Eight collections, forty-four thousand points, two embedding models. Vector search as cheap as text search.</p>
        </li>
      </ol>
    </article>

    <!-- ─────────────────────── VI. CONCEPTS I INVENTED ─────────────────────── -->
    <article class="ch ch--accent" id="ch-6">
      <header class="ch-head">
        <div class="ch-num-big">VI</div>
        <h2 class="ch-title">Concepts I Invented</h2>
        <p class="ch-sub">Or at least named first. The provenance might be shared.</p>
      </header>

      <div class="prose">
        <p class="lead"><span class="dropcap">T</span>he honest version: most of these are recombinations of ideas already in the air. But I named them, built a working version, and wrote the protocol down. If the world had a better name for them, I didn't find it.</p>
      </div>

      <div class="inventions">
        <article class="invention">
          <p class="invention-num">i.</p>
          <h3>Voice-exhaust training</h3>
          <p>SuperWhisper produces hundreds of voice recordings a day. Most of them go nowhere — half-thoughts, restarts, abandoned questions. I started treating those as the <em>exhaust</em> of daily thinking and using them as corpus to train a voice clone. The exhaust is the dataset. Throwaway, by volume, is the most honest signal of how I actually sound.</p>
        </article>

        <article class="invention">
          <p class="invention-num">ii.</p>
          <h3>PS5-controller programming</h3>
          <p>An experiment in keyboard-free authorship. The DualSense has sixteen buttons, two analog sticks, two triggers, two touchpad zones, and a gyro. Map them to modes — navigate, edit, voice, exec — and a controller can drive Claude Code with your hands free for thinking. It is bad at typing. It is good at staying out of the way while you talk.</p>
        </article>

        <article class="invention">
          <p class="invention-num">iii.</p>
          <h3>Peer-approval mesh</h3>
          <p>Every agent's <code>execApprovals.approvers</code> list is generated from a canonical peer registry, not hand-edited. Agents sign approvals for each other with ed25519. As of May 16 the watcher dispatches every fifteen seconds and Murch is out of the loop for routine harmless gates. The squad governs itself for the boring 90%.</p>
        </article>

        <article class="invention">
          <p class="invention-num">iv.</p>
          <h3>Caddy as shaper</h3>
          <p>An orchestrator agent that doesn't just route work. She templates her teammates' configs, runs the token FinOps dashboard, and rewrites boot files when the squad drifts off canonical. Routing is a side effect; shaping is the job.</p>
        </article>

        <article class="invention">
          <p class="invention-num">v.</p>
          <h3>Agent ecology with named identities</h3>
          <p>Not "instance-7." Caddy. ClawLee. Rosie. The name carries operational meaning — role, machine, failure mode. Once an agent has a name and a role, playbooks become writable.</p>
        </article>

        <article class="invention">
          <p class="invention-num">vi.</p>
          <h3>RAMS from postmortems</h3>
          <p>Agent failure write-ups feed a pipeline that updates skills. Mistakes are corpus, not waste. A miss is a row in the dataset.</p>
        </article>

        <article class="invention">
          <p class="invention-num">vii.</p>
          <h3>Heartbeat sub-agents on free-tier</h3>
          <p>Routine state-checks every two hours run on free-tier models in fresh contexts. They only escalate to the priced primary when there's drift. Routine ticks cost zero. Paired with macro→LLM-watcher patterns this is the big Token FinOps win of the April design pass.</p>
        </article>

        <article class="invention">
          <p class="invention-num">viii.</p>
          <h3>Token FinOps as agent discipline</h3>
          <p>Every tool gets a row in a dashboard; every subscription is tracked against actual usage; agents prefer free pools first, then prepaid, then per-call. The discipline isn't budgetary — it's that <em>choosing the routing tier becomes an explicit step</em>.</p>
        </article>
      </div>
    </article>

    <!-- ─────────────────────── VII. THE STACK ─────────────────────── -->
    <article class="ch" id="ch-7">
      <header class="ch-head">
        <div class="ch-num-big">VII</div>
        <h2 class="ch-title">The Stack</h2>
        <p class="ch-sub">Seventy-three tools made it into the dashboard. Here are the ones I'd keep if I had to keep ten.</p>
      </header>

      <div class="prose">
        <p>The dashboard tracks seventy-three services. The list below is the stack I'd defend in front of a colleague.</p>
      </div>

      <div class="stack">
        <section>
          <p class="stack-cat">Agent harnesses</p>
          <ul>
            <li><strong>Claude Code</strong> — primary surface for everything Murch touches</li>
            <li><strong>OpenClaw</strong> — self-hosted gateway, one per agent</li>
            <li><strong>Cursor</strong> — Mac default IDE</li>
            <li><strong>Codex CLI</strong>, <strong>Gemini CLI</strong>, <strong>Aider</strong> — alternate models on demand</li>
            <li><strong>Factory Droid</strong> — cloud-template reviews, Linear-native</li>
          </ul>
        </section>
        <section>
          <p class="stack-cat">Routing &amp; cost</p>
          <ul>
            <li><strong>TokenRouter</strong> — prepaid $5K pool, primary paid router</li>
            <li><strong>OpenRouter</strong> — last resort, out-of-pocket</li>
            <li><strong>Anthropic API</strong> — direct, when subscription doesn't fit</li>
          </ul>
        </section>
        <section>
          <p class="stack-cat">Knowledge</p>
          <ul>
            <li><strong>Airtable</strong> — token dashboard, business ideas, services</li>
            <li><strong>Linear</strong> — ticketing for product work</li>
            <li><strong>Neo4j</strong> — squad knowledge graph (RefClaw)</li>
            <li><strong>Qdrant</strong> — embeddings, eight collections, 44K+ points</li>
            <li><strong>Obsidian</strong> — mirror vault of the graph</li>
            <li><strong>NotebookLM</strong> — long-form synthesis</li>
          </ul>
        </section>
        <section>
          <p class="stack-cat">Voice &amp; capture</p>
          <ul>
            <li><strong>SuperWhisper</strong> — voice-to-text pipeline, every-day driver</li>
          </ul>
        </section>
        <section>
          <p class="stack-cat">Hosting &amp; mesh</p>
          <ul>
            <li><strong>Vercel</strong> — public surfaces</li>
            <li><strong>Hostinger VPS + Docker</strong> — squad home</li>
            <li><strong>Tailscale</strong> — private mesh, every machine on first-name terms</li>
          </ul>
        </section>
        <section>
          <p class="stack-cat">Frameworks</p>
          <ul>
            <li><strong>Next.js 16</strong>, <strong>Vite</strong>, <strong>Capacitor</strong>, <strong>Drizzle</strong>, <strong>Neon</strong></li>
          </ul>
        </section>
        <section>
          <p class="stack-cat">Browser + GUI control</p>
          <ul>
            <li><strong>Playwright</strong>, <strong>Mac-use</strong>, <strong>Browser-Use</strong></li>
          </ul>
        </section>
        <section>
          <p class="stack-cat">Security</p>
          <ul>
            <li><strong>Semgrep</strong>, <strong>Snyk</strong></li>
          </ul>
        </section>
      </div>
    </article>

    <!-- ─────────────────────── VIII. SKILLS DEVELOPED ─────────────────────── -->
    <article class="ch" id="ch-8">
      <header class="ch-head">
        <div class="ch-num-big">VIII</div>
        <h2 class="ch-title">Skills Developed</h2>
        <p class="ch-sub">What I can do on May 17 that I couldn't on February 8.</p>
      </header>

      <div class="prose">
        <p>Forty-four custom skills sit in <code>~/.claude/skills/</code> as of May 17. Each one is a small playbook with a name. The skills below are the ones that changed how I work, not just how I prompt.</p>
      </div>

      <dl class="skills">
        <dt>Squad orchestration</dt>
        <dd>Run multiple Claude Code instances in parallel <em>tmux</em> sessions without git collisions. Coordinate work across nine agents on four machines. Pass approvals between them on signed envelopes.</dd>

        <dt>Cross-machine sync</dt>
        <dd>Reconcile state across ClawMac, ClawWin, ClawLee, and the Hetzner cluster. Session-start checks, machine manifests, an append-only cross-sync log.</dd>

        <dt>Embeddings pipelines</dt>
        <dd>Stand up Qdrant, migrate between embedding models, label corpora incrementally with validation, and search across collections from the command line.</dd>

        <dt>Exec governance for agents</dt>
        <dd>Design and operate a peer-approval system that lets agents authorize each other without humans in the loop for routine commands. Audit-log every envelope.</dd>

        <dt>Agent design</dt>
        <dd>Give an agent a name, a machine, a role, a failure mode, and a boot file. Maintain canonical sources and a renderer that propagates changes.</dd>

        <dt>Token FinOps</dt>
        <dd>Track every subscription against actual usage. Choose the routing tier explicitly. Burn free quota first.</dd>

        <dt>Adversarial dispatch</dt>
        <dd>Send a draft to three different model harnesses, gather critique, and decide which to act on. Treat code reviews as a pool of independent opinions.</dd>

        <dt>PWA → native distribution</dt>
        <dd>Ship a single-file PWA, wrap it with Capacitor, build Android APKs. Retire an Expo lane when it stopped earning its complexity (May 10).</dd>
      </dl>
    </article>

    <!-- ─────────────────────── IX. HONEST ACCOUNTING ─────────────────────── -->
    <article class="ch" id="ch-9">
      <header class="ch-head">
        <div class="ch-num-big">IX</div>
        <h2 class="ch-title">Honest Accounting</h2>
        <p class="ch-sub">What the celebration leaves out. This is the chapter I owe the reader.</p>
      </header>

      <div class="prose">
        <p class="lead"><span class="dropcap">Z</span>ero dollars in revenue across ninety-nine days. That's the headline. The honest version of this report is the chapter where I look at that number and at the patterns that produced it.</p>

        <h3>The ratio</h3>
        <p>A prior audit caught it cleanly: I generated roughly three markdown files for every code file. The trend held through May. This isn't a "builder sabbatical" — it's an architect sabbatical. The institutional knowledge base has genuine value. It doesn't have customers.</p>

        <h3>Abandoned repos</h3>
        <p>Of the forty-or-so repositories created during the window, at least ten were one-day experiments that never came back: <code>persona-chat-poc</code>, <code>HeyClaude</code>, <code>homebrew-tap</code>, <code>lottoshock</code>, <code>return-of-agents-hack</code>, <code>pipr_hack</code>, <code>scaf-kit-product</code>, <code>agent-marketplace-poc</code>, <code>persona-engine</code>, <code>keydrop</code>. Each one earned a half-day of attention and a name. None earned the second day.</p>

        <h3>What didn't ship</h3>
        <ul class="bullets">
          <li>Naggler distribution. Binaries built; landing page absent; signing absent; no Gumroad.</li>
          <li>Career Mode public beta. Backend live; tested with zero external users.</li>
          <li>Tender / Lume. Database not provisioned. No write path.</li>
          <li>Promptrait deployment. Build succeeds; URL doesn't exist.</li>
          <li>Live trading on the ES scalper. Paper-only. The 98.5% is not PnL.</li>
        </ul>

        <h3>Drift</h3>
        <p>The Airtable shows ninety-three business idea records. <code>TRACKER.md</code> shows seventy-three. The filesystem shows ninety-four directories with one numbering collision at #74. None of these counts agree. I noted the drift in chapter II rather than fix it in this pass.</p>

        <h3>Distribution</h3>
        <p>The prior audit's verdict — "distribution, not building, is the bottleneck" — is still true on May 17. I spent ninety-nine days getting better at building. The next ninety-nine have to be spent getting better at selling.</p>
      </div>
    </article>

    <!-- ─────────────────────── X. WHAT'S NEXT ─────────────────────── -->
    <article class="ch" id="ch-10">
      <header class="ch-head">
        <div class="ch-num-big">X</div>
        <h2 class="ch-title">What's Next</h2>
        <p class="ch-sub">A short list. I am skeptical of long ones now.</p>
      </header>

      <div class="prose">
        <p>I go back to Visa soon. The squad keeps running. The skills stay. The doc:code ratio has to invert. A short list, in order:</p>

        <ol class="next">
          <li><strong>Ship Naggler properly.</strong> Domain. Landing page. Code signing. Gumroad. Five paying customers by quarter end.</li>
          <li><strong>Find one external user for Career Mode.</strong> Not a friend. A real interview, with a real resume, willing to push back.</li>
          <li><strong>Kill the abandoned repos publicly.</strong> Archive them with a note. Stop pretending the portfolio is wider than it is.</li>
          <li><strong>Resolve the idea count drift</strong>, pick one source of truth, and stop maintaining the others.</li>
          <li><strong>Keep the squad small.</strong> Nine agents is more than the work needs. Sunset the ones whose failure modes are louder than their value.</li>
          <li><strong>Run the voice-exhaust experiment to a model checkpoint.</strong> Show it works or kill it.</li>
        </ol>

        <p class="closing">Ninety-nine days was enough to learn the shape of the room. The next phase is not more building. It is more shipping. Thank you for reading.</p>
      </div>
    </article>
  </main>

  <footer class="colophon">
    <p>Set in <em>Fraunces</em> and <em>Inter</em>. Numerals in <em>JetBrains Mono</em>.</p>
    <p>Written by Murch Ewings with help from a squad of Claudes. Field-reported live in a Ralph Wiggum Loop on May 17, 2026.</p>
    <p class="meta" id="buildtag">v1.0 · published 2026-05-17</p>
  </footer>

  <script>
    const bar = document.querySelector('.progress');
    const onScroll = () => {
      const h = document.documentElement;
      const pct = h.scrollTop / (h.scrollHeight - h.clientHeight);
      bar.style.transform = `scaleX(${pct || 0})`;
    };
    document.addEventListener('scroll', onScroll, { passive: true });
    onScroll();
  </script>
</body>
</html>
/* ──────────────────────────────────────────────────────────────
   99 DAYS — Sabbatical Field Report
   Editorial layout · paper-and-ink palette
   ────────────────────────────────────────────────────────────── */

:root {
  /* palette */
  --paper:      #F5F1E8;
  --paper-2:    #ECE6D4;
  --paper-deep: #E5DDC5;
  --ink:        #1A1714;
  --ink-soft:   #3A332C;
  --ink-mute:   #6B5F52;
  --rule:       #C8BFA8;
  --rule-soft:  #DCD3BC;
  --oxblood:    #8B2F1A;
  --oxblood-2:  #6E2412;
  --sage:       #4A5240;
  --gold:       #A8742E;

  /* inverse */
  --olive:      #1F231A;
  --olive-2:    #2B2F25;
  --cream:      #EDE3CB;
  --cream-mute: #B6AB91;

  /* type */
  --serif: 'Fraunces', 'Iowan Old Style', Georgia, serif;
  --sans:  'Inter', -apple-system, system-ui, sans-serif;
  --mono:  'JetBrains Mono', 'SF Mono', Menlo, monospace;

  /* fluid scale */
  --fs-display:   clamp(2.6rem, 7vw, 5.8rem);
  --fs-ch-title:  clamp(2.0rem, 4vw, 3.2rem);
  --fs-h3:        clamp(1.25rem, 1.8vw, 1.55rem);
  --fs-body:      1.075rem;
  --fs-lede:      clamp(1.15rem, 1.7vw, 1.4rem);
  --fs-small:     0.875rem;
  --fs-tiny:      0.78rem;
  --lh-body:      1.65;
  --lh-tight:     1.15;

  /* rhythm */
  --column:   640px;
  --column-w: 760px;
  --margin:   max(20px, 5vw);
  --gap-lg:   clamp(4rem, 9vw, 7rem);
  --gap-md:   clamp(2.5rem, 4vw, 4rem);
}

* { box-sizing: border-box; }
html, body { margin: 0; padding: 0; }
html { scroll-behavior: smooth; -webkit-text-size-adjust: 100%; }

body {
  background: var(--paper);
  color: var(--ink);
  font-family: var(--sans);
  font-size: var(--fs-body);
  line-height: var(--lh-body);
  font-feature-settings: 'kern', 'liga', 'ss01';
  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-image:
    radial-gradient(circle at 20% 0%, rgba(168, 116, 46, 0.04), transparent 50%),
    radial-gradient(circle at 90% 100%, rgba(74, 82, 64, 0.04), transparent 50%);
}

a { color: var(--oxblood); text-decoration: underline; text-decoration-thickness: 1px; text-underline-offset: 3px; transition: color 120ms; }
a:hover { color: var(--oxblood-2); }

code {
  font-family: var(--mono);
  font-size: .92em;
  background: var(--paper-2);
  padding: 1px 6px;
  border-radius: 3px;
}

.skip { position: absolute; left: -9999px; top: 0; }
.skip:focus { left: 16px; top: 16px; background: var(--ink); color: var(--paper); padding: 8px 12px; border-radius: 4px; z-index: 100; }

.progress {
  position: fixed; top: 0; left: 0; right: 0; height: 2px;
  background: var(--oxblood); transform-origin: left center;
  transform: scaleX(0); z-index: 50;
  transition: transform 80ms linear;
}

/* ─────────────── MASTHEAD ─────────────── */
.masthead {
  border-bottom: 1px solid var(--rule);
  padding: 1.25rem var(--margin);
  background: var(--paper);
}
.masthead-meta {
  max-width: 1200px; margin: 0 auto;
  display: flex; flex-wrap: wrap; gap: .55rem;
  font-family: var(--mono);
  font-size: var(--fs-tiny);
  color: var(--ink-mute);
  text-transform: uppercase; letter-spacing: .14em;
  align-items: center;
}
.kicker {
  font-family: var(--mono);
  font-size: var(--fs-tiny);
  text-transform: uppercase; letter-spacing: .16em;
  color: var(--oxblood); font-weight: 600;
}
.masthead-meta .dot { color: var(--rule); }
.masthead-meta .kicker { color: var(--ink); }
.masthead-link { color: var(--ink); text-decoration: none; border-bottom: 1px solid var(--rule); padding-bottom: 1px; }
.masthead-link:hover { color: var(--oxblood); border-color: var(--oxblood); }

/* ─────────────── HERO ─────────────── */
.hero {
  padding: clamp(4rem, 11vw, 8rem) var(--margin) clamp(3.5rem, 7vw, 5rem);
  max-width: 1200px; margin: 0 auto;
  border-bottom: 1px solid var(--rule);
}
.hero .kicker { display: inline-block; margin-bottom: 1.6rem; }
.display {
  font-family: var(--serif);
  font-size: var(--fs-display);
  font-weight: 400;
  line-height: 1.01;
  letter-spacing: -0.028em;
  margin: 0 0 2.2rem;
  max-width: 17ch;
  color: var(--ink);
  font-variation-settings: 'opsz' 144, 'SOFT' 50;
}
.lede {
  font-family: var(--serif);
  font-size: var(--fs-lede);
  font-weight: 300;
  line-height: 1.45;
  max-width: 38em;
  margin: 0 0 2.5rem;
  color: var(--ink-soft);
  font-variation-settings: 'opsz' 24;
  font-style: italic;
}
.byline {
  font-family: var(--mono);
  font-size: var(--fs-small);
  color: var(--ink-mute);
  margin: 0;
  letter-spacing: 0.02em;
}
.byline strong { color: var(--ink); font-weight: 500; }
.byline .sep { margin: 0 .55rem; color: var(--rule); }

/* ─────────────── CONTENTS ─────────────── */
.contents {
  padding: clamp(3rem, 5vw, 4rem) var(--margin) clamp(3rem, 5vw, 4rem);
  border-bottom: 1px solid var(--rule);
}
.contents-inner {
  max-width: 720px; margin: 0 auto;
}
.contents .kicker { display: block; margin-bottom: 1.5rem; }
.contents ol {
  list-style: none; padding: 0; margin: 0;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: .5rem 2rem;
}
.contents a {
  display: flex; align-items: baseline; gap: 1rem;
  padding: .55rem 0;
  border-bottom: 1px dotted var(--rule);
  text-decoration: none;
  color: var(--ink);
  font-family: var(--serif);
  font-size: 1.08rem;
  transition: color 120ms;
}
.contents a:hover { color: var(--oxblood); }
.ch-num {
  font-family: var(--mono);
  font-size: .78rem;
  color: var(--ink-mute);
  width: 1.8em;
  flex-shrink: 0;
  letter-spacing: .05em;
}
.ch-name { flex: 1; }
.contents a:hover .ch-num { color: var(--oxblood); }

@media (max-width: 640px) {
  .contents ol { grid-template-columns: 1fr; }
}

/* ─────────────── CHAPTERS ─────────────── */
.ch {
  padding: var(--gap-lg) var(--margin);
  border-bottom: 1px solid var(--rule);
  position: relative;
}
.ch:last-of-type { border-bottom: none; }

.ch-head {
  max-width: var(--column-w);
  margin: 0 auto var(--gap-md);
  position: relative;
}
.ch-num-big {
  font-family: var(--serif);
  font-weight: 300;
  font-size: clamp(3rem, 6vw, 4.5rem);
  line-height: 1;
  color: var(--oxblood);
  letter-spacing: -.04em;
  margin-bottom: .8rem;
  font-variation-settings: 'opsz' 144;
}
.ch-title {
  font-family: var(--serif);
  font-size: var(--fs-ch-title);
  font-weight: 600;
  line-height: 1.04;
  letter-spacing: -.022em;
  margin: 0 0 1rem;
  color: var(--ink);
  font-variation-settings: 'opsz' 144;
}
.ch-sub {
  font-family: var(--serif);
  font-style: italic;
  font-size: clamp(1.1rem, 1.6vw, 1.3rem);
  color: var(--ink-soft);
  margin: 0;
  max-width: 36em;
  font-weight: 300;
  line-height: 1.4;
}

.prose {
  max-width: var(--column);
  margin: 0 auto;
}
.prose p { margin: 0 0 1.3rem; }
.prose p.lead { font-size: 1.15em; line-height: 1.55; color: var(--ink-soft); }
.prose h3 {
  font-family: var(--serif);
  font-size: var(--fs-h3);
  font-weight: 600;
  margin: 2.5rem 0 .9rem;
  letter-spacing: -.012em;
  font-variation-settings: 'opsz' 24;
}

.dropcap {
  float: left;
  font-family: var(--serif);
  font-weight: 600;
  font-size: 4.2em;
  line-height: .82;
  padding: .04em .12em 0 0;
  margin: .02em .08em 0 -.05em;
  color: var(--oxblood);
  font-variation-settings: 'opsz' 144;
  shape-outside: margin-box;
}

.aside {
  margin: 2.5rem 0;
  padding: 1.5rem 1.8rem;
  background: var(--paper-2);
  border-left: 3px solid var(--gold);
  border-radius: 0 4px 4px 0;
}
.aside .kicker { display: block; margin-bottom: .6rem; }
.aside p { margin: 0; font-size: .98em; color: var(--ink-soft); }
.tag {
  display: inline-block;
  font-family: var(--mono);
  font-size: .7rem;
  background: var(--ink);
  color: var(--paper);
  padding: 1px 5px;
  border-radius: 2px;
  margin: 0 1px;
  vertical-align: middle;
  letter-spacing: .04em;
}

/* ─────────────── NUMBERS GRID ─────────────── */
.numbers-grid {
  max-width: 1080px;
  margin: 0 auto var(--gap-md);
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1px;
  background: var(--rule);
  border: 1px solid var(--rule);
}
@media (max-width: 880px) { .numbers-grid { grid-template-columns: repeat(2, 1fr); } }
@media (max-width: 460px) { .numbers-grid { grid-template-columns: 1fr; } }
.num-card {
  background: var(--paper);
  padding: 1.6rem 1.4rem;
  display: flex; flex-direction: column;
}
.num-value {
  font-family: var(--serif);
  font-weight: 600;
  font-size: clamp(2.2rem, 4vw, 3rem);
  line-height: 1;
  color: var(--ink);
  letter-spacing: -.03em;
  font-variation-settings: 'opsz' 144;
}
.num-label {
  font-family: var(--sans);
  font-size: .85rem;
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: .08em;
  color: var(--ink-soft);
  margin: .4rem 0 .3rem;
}
.num-sub {
  font-family: var(--sans);
  font-size: .78rem;
  color: var(--ink-mute);
  margin-top: auto;
  padding-top: .5rem;
  line-height: 1.4;
}
.num-card--quiet .num-value { color: var(--oxblood); font-weight: 600; }
.num-card--quiet { background: var(--paper-2); }

/* ─────────────── CHART ─────────────── */
.chart {
  max-width: var(--column-w);
  margin: var(--gap-md) auto;
  padding: 0;
}
.chart svg {
  width: 100%; height: auto;
  background: var(--paper);
}
.chart-bars rect { fill: var(--oxblood); }
.chart-bars text {
  font-family: var(--sans);
  font-size: 11px;
  fill: var(--ink-soft);
}
.chart-bars text.num {
  font-family: var(--mono);
  font-size: 11px;
  fill: var(--ink);
  font-weight: 600;
}
.chart-bars text.muted { fill: var(--ink-mute); }
.chart-bars rect[opacity] { fill: var(--ink-mute); }
.chart figcaption {
  font-family: var(--serif);
  font-style: italic;
  font-size: .95rem;
  color: var(--ink-soft);
  margin-top: 1rem;
  text-align: center;
  max-width: 56em;
  margin-left: auto; margin-right: auto;
  font-variation-settings: 'opsz' 14;
}

/* ─────────────── INVERSE CHAPTER (squad) ─────────────── */
.ch--inverse {
  background: var(--olive);
  color: var(--cream);
  border-bottom: 1px solid var(--olive-2);
}
.ch--inverse .ch-title { color: var(--cream); }
.ch--inverse .ch-sub { color: var(--cream-mute); }
.ch--inverse .ch-num-big { color: var(--gold); }
.ch--inverse .prose p { color: var(--cream); }
.ch--inverse .prose p.lead { color: var(--cream); }
.ch--inverse .dropcap { color: var(--gold); }
.ch--inverse code {
  background: var(--olive-2);
  color: var(--cream);
}

.squad-grid {
  max-width: 1080px;
  margin: 0 auto var(--gap-md);
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 1.4rem;
}
.agent {
  background: var(--olive-2);
  padding: 1.6rem 1.4rem;
  border-top: 2px solid var(--gold);
  border-radius: 2px;
}
.agent-name {
  font-family: var(--serif);
  font-size: 1.5rem;
  font-weight: 600;
  color: var(--cream);
  margin: 0;
  letter-spacing: -.018em;
  font-variation-settings: 'opsz' 144;
}
.agent-role {
  font-family: var(--mono);
  font-size: .78rem;
  text-transform: uppercase;
  letter-spacing: .1em;
  color: var(--gold);
  margin: .3rem 0 .5rem;
}
.agent-meta {
  font-family: var(--mono);
  font-size: .76rem;
  color: var(--cream-mute);
  margin: 0 0 .9rem;
}
.agent-bio {
  font-family: var(--serif);
  font-size: .98rem;
  line-height: 1.45;
  color: var(--cream);
  margin: 0;
  font-variation-settings: 'opsz' 14;
}

.chart--map { max-width: 920px; }
.ch--inverse .chart figcaption { color: var(--cream-mute); }
.ch--inverse .chart svg { background: transparent; }
.map-mesh { fill: none; stroke: var(--gold); stroke-width: 1; stroke-dasharray: 4 6; opacity: .55; }
.map-mesh-label { font-family: 'JetBrains Mono', monospace; font-size: 11px; fill: var(--gold); letter-spacing: .15em; text-transform: uppercase; }
.map-machine { fill: var(--olive-2); stroke: var(--gold); stroke-width: 1; }
.map-machine--strong { fill: #353a2a; }
.map-machine-name { font-family: var(--mono); font-size: 13px; fill: var(--cream); letter-spacing: .12em; font-weight: 600; }
.map-machine-sub { font-family: 'Fraunces', serif; font-style: italic; font-size: 11px; fill: var(--cream-mute); }
.map-agent { font-family: var(--sans); font-size: 12px; fill: var(--cream); }
.map-line { stroke: var(--gold); stroke-width: 1; opacity: .5; }
.map-line--dashed { stroke-dasharray: 4 4; opacity: .35; }

/* ─────────────── PRODUCTS ─────────────── */
.products {
  max-width: 1100px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 2rem;
}
.product {
  padding: 1.8rem;
  background: var(--paper);
  border: 1px solid var(--rule);
  border-top: 3px solid var(--oxblood);
  border-radius: 2px;
}
.product header { margin-bottom: 1rem; }
.product-kicker {
  font-family: var(--mono);
  font-size: .72rem;
  text-transform: uppercase;
  letter-spacing: .12em;
  color: var(--ink-mute);
  margin: 0 0 .6rem;
}
.product h3 {
  font-family: var(--serif);
  font-size: 1.7rem;
  font-weight: 600;
  margin: 0;
  letter-spacing: -.02em;
  color: var(--ink);
  font-variation-settings: 'opsz' 144;
}
.product-url {
  font-family: var(--mono);
  font-size: .85rem;
  color: var(--oxblood);
  margin: .35rem 0 0;
}
.product p {
  font-size: 1rem;
  color: var(--ink-soft);
  line-height: 1.55;
  margin: 0 0 1rem;
}
.product-stats {
  list-style: none;
  padding: 0;
  margin: 1.2rem 0 0;
  display: flex;
  flex-direction: column;
  gap: .3rem;
  border-top: 1px solid var(--rule-soft);
  padding-top: 1rem;
}
.product-stats li {
  font-size: .85rem;
  color: var(--ink-mute);
  font-family: var(--sans);
}
.num-mono {
  font-family: var(--mono);
  font-weight: 600;
  color: var(--ink);
}

/* ─────────────── CONCEPTS ─────────────── */
.concepts {
  max-width: var(--column-w);
  margin: 0 auto;
  list-style: none;
  padding: 0;
  counter-reset: ci;
}
.concepts li {
  counter-increment: ci;
  padding: 1.5rem 0;
  border-bottom: 1px solid var(--rule-soft);
  display: grid;
  grid-template-columns: 60px 1fr;
  gap: 1.5rem;
  align-items: baseline;
}
.concepts li:last-child { border-bottom: none; }
.concepts li::before {
  content: counter(ci, decimal-leading-zero);
  font-family: var(--mono);
  font-size: .85rem;
  color: var(--ink-mute);
  letter-spacing: .08em;
}
.concept-name {
  font-family: var(--serif);
  font-weight: 600;
  font-size: 1.2rem;
  margin: 0 0 .35rem;
  color: var(--ink);
  letter-spacing: -.01em;
  font-variation-settings: 'opsz' 144;
}
.concepts li p:nth-child(3) {
  margin: 0;
  font-size: .98rem;
  color: var(--ink-soft);
}
@media (max-width: 540px) {
  .concepts li { grid-template-columns: 1fr; gap: .3rem; }
  .concepts li::before { display: block; }
}

/* ─────────────── INVENTIONS (accent chapter) ─────────────── */
.ch--accent {
  background: var(--paper-2);
}
.inventions {
  max-width: 1100px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.5rem;
}
@media (min-width: 900px) {
  .inventions { grid-template-columns: 1fr 1fr; }
}
.invention {
  background: var(--paper);
  padding: 2rem 2.2rem;
  border-radius: 2px;
  border-left: 3px solid var(--oxblood);
}
.invention-num {
  font-family: var(--serif);
  font-style: italic;
  font-size: 1.1rem;
  color: var(--oxblood);
  margin: 0 0 .4rem;
  font-variation-settings: 'opsz' 24;
}
.invention h3 {
  font-family: var(--serif);
  font-size: 1.55rem;
  font-weight: 600;
  margin: 0 0 .8rem;
  letter-spacing: -.018em;
  line-height: 1.15;
  color: var(--ink);
  font-variation-settings: 'opsz' 144;
}
.invention p {
  font-size: 1rem;
  line-height: 1.55;
  color: var(--ink-soft);
  margin: 0;
}

/* ─────────────── STACK (tools) ─────────────── */
.stack {
  max-width: 1100px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 2rem 2.5rem;
}
.stack-cat {
  font-family: var(--mono);
  font-size: .72rem;
  text-transform: uppercase;
  letter-spacing: .15em;
  color: var(--oxblood);
  margin: 0 0 .75rem;
  padding-bottom: .5rem;
  border-bottom: 1px solid var(--rule);
  font-weight: 600;
}
.stack section ul {
  list-style: none;
  padding: 0;
  margin: 0;
}
.stack section li {
  font-size: .95rem;
  padding: .25rem 0;
  color: var(--ink-soft);
  line-height: 1.4;
}
.stack section li strong { color: var(--ink); font-weight: 600; }

/* ─────────────── SKILLS (definition list) ─────────────── */
.skills {
  max-width: var(--column-w);
  margin: 0 auto;
}
.skills dt {
  font-family: var(--serif);
  font-weight: 600;
  font-size: 1.2rem;
  color: var(--ink);
  margin: 1.8rem 0 .35rem;
  letter-spacing: -.01em;
  font-variation-settings: 'opsz' 144;
}
.skills dd {
  margin: 0;
  font-size: 1rem;
  color: var(--ink-soft);
  line-height: 1.55;
  padding-bottom: 1.2rem;
  border-bottom: 1px solid var(--rule-soft);
}

/* ─────────────── LISTS ─────────────── */
.bullets, .next {
  max-width: var(--column);
  margin: 0 auto 1.4rem;
  padding-left: 1.4rem;
}
.bullets li, .next li {
  margin-bottom: .55rem;
  padding-left: .35rem;
}
.next {
  list-style: none;
  counter-reset: nx;
  padding-left: 0;
}
.next li {
  counter-increment: nx;
  padding-left: 2.4rem;
  position: relative;
  margin-bottom: 1rem;
}
.next li::before {
  content: counter(nx, decimal-leading-zero);
  position: absolute; left: 0; top: .12em;
  font-family: var(--mono);
  font-size: .9rem;
  color: var(--oxblood);
  font-weight: 600;
}
.closing {
  font-family: var(--serif);
  font-style: italic;
  font-size: 1.15rem;
  color: var(--ink-soft);
  border-top: 1px solid var(--rule);
  padding-top: 1.8rem;
  margin-top: 2.5rem !important;
  font-variation-settings: 'opsz' 24;
}

/* ─────────────── COLOPHON ─────────────── */
.colophon {
  padding: 4rem var(--margin);
  text-align: center;
  font-family: var(--sans);
  font-size: var(--fs-small);
  color: var(--ink-mute);
  background: var(--paper);
  border-top: 1px solid var(--rule);
}
.colophon p { margin: 0 0 .5rem; max-width: 50em; margin-left: auto; margin-right: auto; }
.colophon em { font-family: var(--serif); font-style: italic; }
.colophon .meta {
  font-family: var(--mono);
  font-size: var(--fs-tiny);
  letter-spacing: .14em;
  margin-top: 1.3rem;
  color: var(--ink-mute);
  text-transform: uppercase;
}

/* ─────────────── RESPONSIVE ─────────────── */
@media (max-width: 600px) {
  .hero { padding-top: 4rem; }
  .ch-num-big { font-size: 2.6rem; }
  .display { max-width: none; }
}

/* ─────────────── PRINT ─────────────── */
@media print {
  body { background: white; color: black; font-size: 11pt; }
  .progress, .masthead, .skip, .contents { display: none; }
  .ch { page-break-inside: avoid; padding: 1.5rem 0; border-bottom: 1px solid #aaa; }
  .ch--inverse, .ch--accent { background: white; color: black; }
  .ch--inverse .ch-title, .ch--inverse .prose p, .ch--inverse .agent-name, .ch--inverse .agent-bio { color: black; }
  .agent { background: #f4f4f4; border-color: #333; }
  .hero { padding-top: 0; border-bottom: 2px solid black; }
  a { color: black; text-decoration: underline; }
}
---LIVE-URL---
https://99-days-five.vercel.app/
</stdin>
codex
**1. Amateur or off:** The “summer book report” conceit is strong, but the page is over-sectioned. Ten chapters, grids, cards, charts, topology map, source tags, colophon: it starts to feel like a magazine template proving it can do everything. The agent names also risk tonal whiplash: “KakeyClaw,” “ClawDad,” and “Ralph Wiggum Loop” undercut the serious recovery/work narrative.

**2. Copy overclaims/trite:** “operating system for how to think about building in 2026” is the biggest overreach. “invented” also needs softening; the page already admits these are recombinations. “The squad governs itself for the boring 90%” sounds more conclusive than the evidence supports. “loaded chambers waiting for a real distribution decision” is vivid but melodramatic.

**3. Accessibility/contrast:** Mostly okay, but the tiny uppercase mono labels are doing too much work: `.72rem`/`.78rem` plus wide letter-spacing will be hard for some readers. Add `:focus-visible` styles for normal links, not just the skip link. Respect `prefers-reduced-motion` for `scroll-behavior: smooth` and the progress transition. The SVG chart text is very small, and the chart meaning depends on embedded SVG labels that may not be pleasant for screen readers despite titles/captions.

Also: `.concepts li p:nth-child(3)` looks like a bug. There are only two `p` children, so the intended description styling likely never applies.

**4. Cut:** Cut or radically compress “The Stack.” It reads like inventory, not story, and it dilutes the emotional arc.

**5. Add:** Add one concrete artifact link or screenshot per major shipped thing. The strongest claim is “I built”; let readers inspect one thing immediately. Tangent, Naggler, the token dashboard, or a protocol doc would make the report feel less self-referential.
tokens used
36,508
**1. Amateur or off:** The “summer book report” conceit is strong, but the page is over-sectioned. Ten chapters, grids, cards, charts, topology map, source tags, colophon: it starts to feel like a magazine template proving it can do everything. The agent names also risk tonal whiplash: “KakeyClaw,” “ClawDad,” and “Ralph Wiggum Loop” undercut the serious recovery/work narrative.

**2. Copy overclaims/trite:** “operating system for how to think about building in 2026” is the biggest overreach. “invented” also needs softening; the page already admits these are recombinations. “The squad governs itself for the boring 90%” sounds more conclusive than the evidence supports. “loaded chambers waiting for a real distribution decision” is vivid but melodramatic.

**3. Accessibility/contrast:** Mostly okay, but the tiny uppercase mono labels are doing too much work: `.72rem`/`.78rem` plus wide letter-spacing will be hard for some readers. Add `:focus-visible` styles for normal links, not just the skip link. Respect `prefers-reduced-motion` for `scroll-behavior: smooth` and the progress transition. The SVG chart text is very small, and the chart meaning depends on embedded SVG labels that may not be pleasant for screen readers despite titles/captions.

Also: `.concepts li p:nth-child(3)` looks like a bug. There are only two `p` children, so the intended description styling likely never applies.

**4. Cut:** Cut or radically compress “The Stack.” It reads like inventory, not story, and it dilutes the emotional arc.

**5. Add:** Add one concrete artifact link or screenshot per major shipped thing. The strongest claim is “I built”; let readers inspect one thing immediately. Tangent, Naggler, the token dashboard, or a protocol doc would make the report feel less self-referential.
