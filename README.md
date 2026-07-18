<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
  viewBox="0 0 1180 610" width="1180" height="610" role="img" aria-label="Developer Profile Banner">

  <defs>
    <!-- Clip paths -->
    <clipPath id="l-main-clip">
      <rect width="1180" height="610" rx="20" ry="20"/>
    </clipPath>
    <clipPath id="l-left-clip">
      <rect x="0" y="0" width="448" height="610"/>
    </clipPath>
    <clipPath id="l-right-clip">
      <rect x="448" y="0" width="732" height="610"/>
    </clipPath>
    <clipPath id="l-terminal-clip">
      <rect x="468" y="20" width="692" height="570" rx="14" ry="14"/>
    </clipPath>

    <!-- Background gradients — light mode -->
    <radialGradient id="l-bg-glow1" cx="20%" cy="25%" r="50%">
      <stop offset="0%" stop-color="#dbeafe" stop-opacity="0.8"/>
      <stop offset="100%" stop-color="#ffffff" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="l-bg-glow2" cx="80%" cy="75%" r="45%">
      <stop offset="0%" stop-color="#cffafe" stop-opacity="0.6"/>
      <stop offset="100%" stop-color="#ffffff" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="l-bg-glow3" cx="50%" cy="50%" r="55%">
      <stop offset="0%" stop-color="#d1fae5" stop-opacity="0.4"/>
      <stop offset="100%" stop-color="#ffffff" stop-opacity="0"/>
    </radialGradient>

    <!-- ASCII gradient light mode -->
    <linearGradient id="l-ascii-grad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#2563eb">
        <animate attributeName="stop-color" values="#2563eb;#0891b2;#059669;#2563eb" dur="4s" repeatCount="indefinite"/>
      </stop>
      <stop offset="50%" stop-color="#06b6d4">
        <animate attributeName="stop-color" values="#06b6d4;#2563eb;#0891b2;#06b6d4" dur="4s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" stop-color="#10b981">
        <animate attributeName="stop-color" values="#10b981;#06b6d4;#2563eb;#10b981" dur="4s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>

    <!-- Terminal gradient light -->
    <linearGradient id="l-terminal-grad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#f8fafc"/>
      <stop offset="100%" stop-color="#f1f5f9"/>
    </linearGradient>

    <!-- Border shimmer light -->
    <linearGradient id="l-border-shimmer" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(37,99,235,0)"/>
      <stop offset="30%" stop-color="rgba(6,182,212,0.5)"/>
      <stop offset="60%" stop-color="rgba(37,99,235,0.5)"/>
      <stop offset="100%" stop-color="rgba(16,185,129,0)"/>
      <animateTransform attributeName="gradientTransform" type="translate" from="-1 0" to="1 0" dur="3s" repeatCount="indefinite"/>
    </linearGradient>

    <!-- Glow filter for ASCII — softer in light mode -->
    <filter id="l-ascii-glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="1.5" result="blur1"/>
      <feGaussianBlur stdDeviation="3" result="blur2"/>
      <feMerge>
        <feMergeNode in="blur2"/>
        <feMergeNode in="blur1"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Glow filter for panels -->
    <filter id="l-panel-shadow" x="-5%" y="-5%" width="115%" height="115%">
      <feGaussianBlur stdDeviation="12" result="blur"/>
      <feFlood flood-color="rgba(15,23,42,0.08)" result="color"/>
      <feComposite in="color" in2="blur" operator="in" result="shadow"/>
      <feMerge>
        <feMergeNode in="shadow"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Pill glow filter -->
    <filter id="l-pill-glow" x="-10%" y="-20%" width="120%" height="140%">
      <feGaussianBlur stdDeviation="2" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Scanline pattern light -->
    <pattern id="l-scanlines" x="0" y="0" width="1" height="4" patternUnits="userSpaceOnUse">
      <line x1="0" y1="0" x2="1" y2="0" stroke="rgba(15,23,42,0.03)" stroke-width="1"/>
    </pattern>

    <!-- Glass reflection -->
    <linearGradient id="l-glass-reflect" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.7)"/>
      <stop offset="40%" stop-color="rgba(255,255,255,0.3)"/>
      <stop offset="100%" stop-color="rgba(255,255,255,0)"/>
    </linearGradient>

    <!-- Left panel gradient light -->
    <linearGradient id="l-left-panel-grad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#f0f4ff"/>
      <stop offset="100%" stop-color="#e8f4f8"/>
    </linearGradient>

    <!-- Accent gradient light -->
    <linearGradient id="l-accent-grad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#2563eb"/>
      <stop offset="50%" stop-color="#06b6d4"/>
      <stop offset="100%" stop-color="#10b981"/>
    </linearGradient>

    <!-- Skill pill gradients light -->
    <linearGradient id="l-pill-blue" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(37,99,235,0.12)"/>
      <stop offset="100%" stop-color="rgba(37,99,235,0.04)"/>
    </linearGradient>
    <linearGradient id="l-pill-cyan" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(6,182,212,0.12)"/>
      <stop offset="100%" stop-color="rgba(6,182,212,0.04)"/>
    </linearGradient>
    <linearGradient id="l-pill-green" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(16,185,129,0.12)"/>
      <stop offset="100%" stop-color="rgba(16,185,129,0.04)"/>
    </linearGradient>

    <!-- Particle glow light -->
    <radialGradient id="l-particle-glow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#2563eb" stop-opacity="0.5"/>
      <stop offset="100%" stop-color="#2563eb" stop-opacity="0"/>
    </radialGradient>

    <!-- Masks for line reveals -->
    <mask id="l-ascii-line1"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="0.3s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line2"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="0.45s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line3"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="0.6s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line4"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="0.75s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line5"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="0.9s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line6"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.05s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line7"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.2s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line8"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.35s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line9"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.5s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line10"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.65s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line11"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.8s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line12"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.95s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line13"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.1s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line14"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.25s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line15"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.4s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line16"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.55s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line17"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.7s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line18"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.85s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line19"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.0s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line20"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.15s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line21"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.3s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line22"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.45s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line23"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.6s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line24"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.75s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line25"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.9s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line26"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="4.05s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line27"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="4.2s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line28"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="4.35s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line29"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="4.5s" fill="freeze"/></rect></mask>
    <mask id="l-ascii-line30"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="4.65s" fill="freeze"/></rect></mask>

  </defs>

  <!-- ═══════════════════════════════════════════ -->
  <!-- MAIN CANVAS                                  -->
  <!-- ═══════════════════════════════════════════ -->
  <g clip-path="url(#l-main-clip)">

    <!-- Base background white -->
    <rect width="1180" height="610" fill="#ffffff"/>

    <!-- Background glows (subtle) -->
    <rect width="1180" height="610" fill="url(#l-bg-glow1)">
      <animateTransform attributeName="transform" type="translate" values="0,0;20,10;0,0" dur="8s" repeatCount="indefinite"/>
    </rect>
    <rect width="1180" height="610" fill="url(#l-bg-glow2)">
      <animateTransform attributeName="transform" type="translate" values="0,0;-15,8;0,0" dur="10s" repeatCount="indefinite"/>
    </rect>
    <rect width="1180" height="610" fill="url(#l-bg-glow3)">
      <animateTransform attributeName="transform" type="translate" values="0,0;10,-12;0,0" dur="12s" repeatCount="indefinite"/>
    </rect>

    <!-- Scanlines (very subtle on light) -->
    <rect width="1180" height="610" fill="url(#l-scanlines)" opacity="0.5"/>

    <!-- Animated particles (light mode) -->
    <g opacity="0.5">
      <circle r="2" fill="url(#l-particle-glow)" opacity="0">
        <animate attributeName="cx" values="120;140;120" dur="7s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="80;60;80" dur="7s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.5;0" dur="7s" repeatCount="indefinite"/>
      </circle>
      <circle r="1.5" fill="#06b6d4" opacity="0">
        <animate attributeName="cx" values="300;280;300" dur="9s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="150;130;150" dur="9s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.4;0" dur="9s" repeatCount="indefinite"/>
      </circle>
      <circle r="1" fill="#10b981" opacity="0">
        <animate attributeName="cx" values="200;220;200" dur="11s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="400;380;400" dur="11s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.4;0" dur="11s" repeatCount="indefinite"/>
      </circle>
      <circle r="2" fill="#2563eb" opacity="0">
        <animate attributeName="cx" values="80;100;80" dur="6s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="450;470;450" dur="6s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.3;0" dur="6s" repeatCount="indefinite"/>
      </circle>
      <circle r="1.5" fill="#06b6d4" opacity="0">
        <animate attributeName="cx" values="800;820;800" dur="8s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="100;80;100" dur="8s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.4;0" dur="8s" repeatCount="indefinite"/>
      </circle>
      <circle r="1" fill="#2563eb" opacity="0">
        <animate attributeName="cx" values="1050;1030;1050" dur="10s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="200;220;200" dur="10s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.3;0" dur="10s" repeatCount="indefinite"/>
      </circle>
      <circle r="2" fill="#10b981" opacity="0">
        <animate attributeName="cx" values="950;970;950" dur="13s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="500;480;500" dur="13s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.3;0" dur="13s" repeatCount="indefinite"/>
      </circle>
    </g>

    <!-- ═══════════════════════════════════════════ -->
    <!-- LEFT PANEL — ASCII Terminal (Light)         -->
    <!-- ═══════════════════════════════════════════ -->
    <g clip-path="url(#l-left-clip)">

      <!-- Left panel background -->
      <rect x="0" y="0" width="448" height="610" fill="url(#l-left-panel-grad)"/>

      <!-- Left panel border right -->
      <line x1="447" y1="0" x2="447" y2="610" stroke="rgba(15,23,42,0.08)" stroke-width="1"/>

      <!-- Animated shimmer on border -->
      <line x1="447" y1="0" x2="447" y2="610" stroke="url(#l-border-shimmer)" stroke-width="1.5" opacity="0.4">
        <animate attributeName="opacity" values="0.15;0.5;0.15" dur="3s" repeatCount="indefinite"/>
      </line>

      <!-- Glass reflection overlay -->
      <rect x="0" y="0" width="448" height="200" fill="url(#l-glass-reflect)"/>

      <!-- Terminal header bar -->
      <rect x="0" y="0" width="448" height="36" fill="rgba(15,23,42,0.03)"/>
      <line x1="0" y1="36" x2="448" y2="36" stroke="rgba(15,23,42,0.08)" stroke-width="1"/>

      <!-- Terminal dots -->
      <circle cx="22" cy="18" r="5" fill="#ff5f57"/>
      <circle cx="40" cy="18" r="5" fill="#febc2e"/>
      <circle cx="58" cy="18" r="5" fill="#28c840"/>

      <!-- Terminal title -->
      <text x="224" y="22" font-family="'SF Mono', 'Fira Code', monospace" font-size="11" fill="rgba(15,23,42,0.3)" text-anchor="middle">~/ascii-portrait.sh</text>

      <!-- Moving scanline sweep (light) -->
      <rect x="0" y="36" width="448" height="2" fill="rgba(37,99,235,0.06)">
        <animate attributeName="y" values="36;610;36" dur="6s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.4;0" dur="6s" repeatCount="indefinite"/>
      </rect>

      <!-- ASCII Portrait -->
      <g font-family="'SF Mono', 'Fira Code', 'Courier New', monospace" font-size="8.2" filter="url(#l-ascii-glow)">
        <g>
          <animateTransform attributeName="transform" type="translate" values="0,0;0,-5;0,0" dur="5s" repeatCount="indefinite"/>

          <text x="24" y="64" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line1)">  ██████╗ ███████╗██╗   ██╗</text>
          <text x="24" y="76" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line2)">  ██╔══██╗██╔════╝██║   ██║</text>
          <text x="24" y="88" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line3)">  ██║  ██║█████╗  ██║   ██║</text>
          <text x="24" y="100" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line4)">  ██║  ██║██╔══╝  ╚██╗ ██╔╝</text>
          <text x="24" y="112" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line5)">  ██████╔╝███████╗ ╚████╔╝</text>
          <text x="24" y="124" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line6)">  ╚═════╝ ╚══════╝  ╚═══╝</text>
          <text x="24" y="148" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line7)">   ░░░░░░░░░░░░░░░░░░░░░░░</text>
          <text x="24" y="160" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line8)">  ╔═══════════════════════╗</text>
          <text x="24" y="172" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line9)">  ║  ╭──────────────────╮  ║</text>
          <text x="24" y="184" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line10)">  ║  │  ◉  ◉           │  ║</text>
          <text x="24" y="196" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line11)">  ║  │    ╭──╮          │  ║</text>
          <text x="24" y="208" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line12)">  ║  │    │  │          │  ║</text>
          <text x="24" y="220" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line13)">  ║  │  ╰────╯          │  ║</text>
          <text x="24" y="232" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line14)">  ║  │ ╭──────────────╮ │  ║</text>
          <text x="24" y="244" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line15)">  ║  ╰──────────────────╯  ║</text>
          <text x="24" y="268" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line16)">  ╚═══════════════════════╝</text>
          <text x="24" y="292" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line17)">  ▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄</text>
          <text x="24" y="316" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line18)">  ▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀</text>
          <text x="24" y="340" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line19)">  ┌───────────────────────┐</text>
          <text x="24" y="352" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line20)">  │  &gt; developer.exe       │</text>
          <text x="24" y="364" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line21)">  │  &gt; loading modules...  │</text>
          <text x="24" y="376" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line22)">  │  &gt; [████████████] 100% │</text>
          <text x="24" y="388" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line23)">  │  &gt; ready               │</text>
          <text x="24" y="400" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line24)">  └───────────────────────┘</text>
          <text x="24" y="424" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line25)">  ·  ·  ·  ·  ·  ·  ·  ·</text>
          <text x="24" y="448" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line26)">  ◆  open to opportunities</text>
          <text x="24" y="472" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line27)">  ◆  building the future</text>
          <text x="24" y="496" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line28)">  ◆  one commit at a time</text>
          <text x="24" y="520" fill="url(#l-ascii-grad)" mask="url(#l-ascii-line29)">  ·  ·  ·  ·  ·  ·  ·  ·</text>
          <text x="24" y="544" fill="#2563eb" mask="url(#l-ascii-line30)">  $<tspan fill="#06b6d4"> ▌</tspan>
            <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>
          </text>
        </g>
      </g>

      <!-- Fade bottom -->
      <rect x="0" y="540" width="448" height="70" fill="url(#l-left-panel-grad)" opacity="0.9"/>

    </g>

    <!-- ═══════════════════════════════════════════ -->
    <!-- RIGHT PANEL — Terminal (Light)              -->
    <!-- ═══════════════════════════════════════════ -->
    <g clip-path="url(#l-right-clip)">

      <!-- Terminal window shadow -->
      <rect x="470" y="24" width="692" height="570" rx="14" ry="14" fill="rgba(15,23,42,0.06)" filter="url(#l-panel-shadow)"/>

      <!-- Terminal window body -->
      <rect x="468" y="20" width="692" height="570" rx="14" ry="14" fill="url(#l-terminal-grad)"/>

      <!-- Terminal border light -->
      <rect x="468" y="20" width="692" height="570" rx="14" ry="14" fill="none" stroke="rgba(15,23,42,0.08)" stroke-width="1"/>

      <!-- Border shimmer -->
      <rect x="468" y="20" width="692" height="1.5" rx="1" ry="1" fill="url(#l-border-shimmer)" opacity="0.5"/>

      <!-- Glass reflection -->
      <rect x="468" y="20" width="692" height="200" rx="14" ry="14" fill="url(#l-glass-reflect)" clip-path="url(#l-terminal-clip)"/>

      <!-- Terminal header -->
      <rect x="468" y="20" width="692" height="42" rx="14" ry="14" fill="rgba(15,23,42,0.02)" clip-path="url(#l-terminal-clip)"/>
      <rect x="468" y="50" width="692" height="12" fill="rgba(15,23,42,0.02)" clip-path="url(#l-terminal-clip)"/>
      <line x1="468" y1="62" x2="1160" y2="62" stroke="rgba(15,23,42,0.08)" stroke-width="1"/>

      <!-- Window dots -->
      <circle cx="490" cy="41" r="5.5" fill="#ff5f57"/>
      <circle cx="508" cy="41" r="5.5" fill="#febc2e"/>
      <circle cx="526" cy="41" r="5.5" fill="#28c840"/>

      <!-- Terminal title -->
      <text x="814" y="46" font-family="'SF Mono','Fira Code',monospace" font-size="12" fill="rgba(15,23,42,0.25)" text-anchor="middle">~/portfolio — zsh</text>

      <!-- ─── CONTENT ─── -->
      <g clip-path="url(#l-terminal-clip)">

        <!-- Prompt -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.1s" begin="1.0s" fill="freeze"/>
          <text x="492" y="92" font-family="'SF Mono','Fira Code',monospace" font-size="12" fill="#2563eb">❯</text>
          <text x="506" y="92" font-family="'SF Mono','Fira Code',monospace" font-size="12" fill="#06b6d4">whoami</text>
        </g>

        <!-- Greeting -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.1s" begin="1.3s" fill="freeze"/>
          <text x="492" y="120" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="14" fill="rgba(71,85,105,0.85)" letter-spacing="0.05em">Hi 👋  Welcome to my terminal</text>
        </g>

        <!-- Name -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.1s" begin="1.6s" fill="freeze"/>
          <text x="492" y="158" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="34" font-weight="700" fill="url(#l-accent-grad)" letter-spacing="-0.02em">Alex Chen</text>
        </g>

        <!-- Animated subtitle -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.1s" begin="2.0s" fill="freeze"/>
          <text x="492" y="190" font-family="'SF Mono','Fira Code',monospace" font-size="15" fill="#2563eb" opacity="1">
            <animate attributeName="opacity" values="1;1;0;0;0;0;0;0;0;0" dur="10s" repeatCount="indefinite" begin="2.0s"/>Frontend Engineer</text>
          <text x="492" y="190" font-family="'SF Mono','Fira Code',monospace" font-size="15" fill="#0891b2" opacity="0">
            <animate attributeName="opacity" values="0;0;1;1;0;0;0;0;0;0" dur="10s" repeatCount="indefinite" begin="2.0s"/>Full Stack Developer</text>
          <text x="492" y="190" font-family="'SF Mono','Fira Code',monospace" font-size="15" fill="#059669" opacity="0">
            <animate attributeName="opacity" values="0;0;0;0;1;1;0;0;0;0" dur="10s" repeatCount="indefinite" begin="2.0s"/>Open Source Contributor</text>
          <text x="492" y="190" font-family="'SF Mono','Fira Code',monospace" font-size="15" fill="#d97706" opacity="0">
            <animate attributeName="opacity" values="0;0;0;0;0;0;1;1;0;0" dur="10s" repeatCount="indefinite" begin="2.0s"/>UI / AI Enthusiast</text>
          <text x="492" y="190" font-family="'SF Mono','Fira Code',monospace" font-size="15" fill="#2563eb" opacity="0">
            <animate attributeName="opacity" values="0;0;0;0;0;0;0;0;1;1" dur="10s" repeatCount="indefinite" begin="2.0s"/>Frontend Engineer</text>

          <!-- Typing cursor -->
          <rect x="696" y="175" width="2" height="18" fill="#06b6d4">
            <animate attributeName="opacity" values="1;0;1" dur="0.8s" repeatCount="indefinite"/>
          </rect>
        </g>

        <!-- Divider -->
        <line x1="492" y1="206" x2="1148" y2="206" stroke="rgba(15,23,42,0.07)" stroke-width="1" opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="2.4s" fill="freeze"/>
        </line>

        <!-- Info items -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="2.6s" fill="freeze"/>
          <text x="492" y="232" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#2563eb">📍</text>
          <text x="516" y="232" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#475569">San Francisco, CA</text>
        </g>
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="2.9s" fill="freeze"/>
          <text x="492" y="254" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#06b6d4">🎓</text>
          <text x="516" y="254" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#475569">CS @ MIT</text>
        </g>
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="3.2s" fill="freeze"/>
          <text x="492" y="276" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#059669">⚡</text>
          <text x="516" y="276" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#475569">Building AI-powered dev tools</text>
        </g>
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="3.5s" fill="freeze"/>
          <text x="492" y="298" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#7c3aed">🌐</text>
          <text x="516" y="298" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#475569">alexchen.dev</text>
        </g>
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="3.8s" fill="freeze"/>
          <text x="492" y="320" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#d97706">✉</text>
          <text x="516" y="320" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#475569">alex@alexchen.dev</text>
        </g>

        <!-- Divider 2 -->
        <line x1="492" y1="340" x2="1148" y2="340" stroke="rgba(15,23,42,0.07)" stroke-width="1" opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="4.1s" fill="freeze"/>
        </line>

        <!-- Skills label -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="4.3s" fill="freeze"/>
          <text x="492" y="364" font-family="'SF Mono','Fira Code',monospace" font-size="10" fill="rgba(71,85,105,0.5)" letter-spacing="0.15em">SKILLS</text>
        </g>

        <!-- Skill Pills Row 1 (light) -->
        <g filter="url(#l-pill-glow)" opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.6s" fill="freeze"/>

          <rect x="492" y="374" width="60" height="24" rx="12" fill="url(#l-pill-cyan)" stroke="rgba(6,182,212,0.35)" stroke-width="1"/>
          <text x="522" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#0891b2" text-anchor="middle">React</text>

          <rect x="560" y="374" width="64" height="24" rx="12" fill="url(#l-pill-blue)" stroke="rgba(37,99,235,0.35)" stroke-width="1"/>
          <text x="592" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#2563eb" text-anchor="middle">Next.js</text>

          <rect x="632" y="374" width="64" height="24" rx="12" fill="url(#l-pill-green)" stroke="rgba(16,185,129,0.35)" stroke-width="1"/>
          <text x="664" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#059669" text-anchor="middle">Node.js</text>

          <rect x="704" y="374" width="82" height="24" rx="12" fill="url(#l-pill-cyan)" stroke="rgba(6,182,212,0.35)" stroke-width="1"/>
          <text x="745" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#0891b2" text-anchor="middle">TypeScript</text>

          <rect x="794" y="374" width="70" height="24" rx="12" fill="url(#l-pill-blue)" stroke="rgba(37,99,235,0.35)" stroke-width="1"/>
          <text x="829" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#2563eb" text-anchor="middle">Tailwind</text>

          <rect x="872" y="374" width="60" height="24" rx="12" fill="url(#l-pill-green)" stroke="rgba(16,185,129,0.35)" stroke-width="1"/>
          <text x="902" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#059669" text-anchor="middle">Python</text>
        </g>

        <!-- Skill Pills Row 2 (light) -->
        <g filter="url(#l-pill-glow)" opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.9s" fill="freeze"/>

          <rect x="492" y="406" width="62" height="24" rx="12" fill="url(#l-pill-cyan)" stroke="rgba(6,182,212,0.3)" stroke-width="1"/>
          <text x="523" y="422" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#0891b2" text-anchor="middle">Docker</text>

          <rect x="562" y="406" width="70" height="24" rx="12" fill="url(#l-pill-blue)" stroke="rgba(37,99,235,0.3)" stroke-width="1"/>
          <text x="597" y="422" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#2563eb" text-anchor="middle">Postgres</text>

          <rect x="640" y="406" width="50" height="24" rx="12" fill="url(#l-pill-green)" stroke="rgba(16,185,129,0.3)" stroke-width="1"/>
          <text x="665" y="422" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#059669" text-anchor="middle">AWS</text>

          <rect x="698" y="406" width="44" height="24" rx="12" fill="url(#l-pill-cyan)" stroke="rgba(6,182,212,0.3)" stroke-width="1"/>
          <text x="720" y="422" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#0891b2" text-anchor="middle">Git</text>

          <rect x="750" y="406" width="56" height="24" rx="12" fill="url(#l-pill-blue)" stroke="rgba(37,99,235,0.3)" stroke-width="1"/>
          <text x="778" y="422" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#2563eb" text-anchor="middle">Figma</text>
        </g>

        <!-- Divider 3 -->
        <line x1="492" y1="448" x2="1148" y2="448" stroke="rgba(15,23,42,0.07)" stroke-width="1" opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="5.3s" fill="freeze"/>
        </line>

        <!-- Connect label -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="5.5s" fill="freeze"/>
          <text x="492" y="472" font-family="'SF Mono','Fira Code',monospace" font-size="10" fill="rgba(71,85,105,0.5)" letter-spacing="0.15em">CONNECT</text>
        </g>

        <!-- Social Icons (light) -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.7s" fill="freeze"/>

          <g filter="url(#l-pill-glow)">
            <rect x="492" y="484" width="100" height="36" rx="18" fill="rgba(15,23,42,0.03)" stroke="rgba(15,23,42,0.1)" stroke-width="1"/>
            <text x="508" y="505" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="#475569">⬡ GitHub</text>
          </g>
          <g filter="url(#l-pill-glow)">
            <rect x="600" y="484" width="100" height="36" rx="18" fill="rgba(15,23,42,0.03)" stroke="rgba(15,23,42,0.1)" stroke-width="1"/>
            <text x="613" y="505" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="#475569">⬡ LinkedIn</text>
          </g>
          <g filter="url(#l-pill-glow)">
            <rect x="708" y="484" width="100" height="36" rx="18" fill="rgba(15,23,42,0.03)" stroke="rgba(15,23,42,0.1)" stroke-width="1"/>
            <text x="728" y="505" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="#475569">⬡ Twitter</text>
          </g>
          <g filter="url(#l-pill-glow)">
            <rect x="816" y="484" width="100" height="36" rx="18" fill="rgba(37,99,235,0.06)" stroke="rgba(37,99,235,0.25)" stroke-width="1"/>
            <text x="826" y="505" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="#2563eb">⬡ Portfolio</text>
          </g>
        </g>

        <!-- Bottom prompt (light) -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="6.0s" fill="freeze"/>
          <text x="492" y="544" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="#2563eb">❯ </text>
          <text x="506" y="544" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="#06b6d4">git commit -m </text>
          <text x="680" y="544" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="#059669">"always be building"</text>
          <!-- Cursor -->
          <rect x="860" y="531" width="2" height="14" fill="#06b6d4">
            <animate attributeName="opacity" values="1;0;1" dur="0.8s" repeatCount="indefinite"/>
          </rect>
        </g>

        <!-- Moving scanline (light) -->
        <rect x="468" y="62" width="692" height="1.5" fill="rgba(37,99,235,0.04)" clip-path="url(#l-terminal-clip)">
          <animate attributeName="y" values="62;590;62" dur="8s" repeatCount="indefinite"/>
        </rect>

      </g><!-- end terminal clip -->
    </g><!-- end right clip -->

    <!-- ═══════════════════════════════════════════ -->
    <!-- OUTER BORDER                                -->
    <!-- ═══════════════════════════════════════════ -->
    <rect width="1180" height="610" rx="20" ry="20" fill="none" stroke="rgba(15,23,42,0.08)" stroke-width="1.5"/>
    <rect x="0" y="0" width="1180" height="1.5" rx="1" fill="url(#l-border-shimmer)" opacity="0.6"/>
    <rect x="0" y="608.5" width="1180" height="1.5" rx="1" fill="url(#l-border-shimmer)" opacity="0.3"/>

  </g><!-- end main clip -->

</svg>

![Header Wave](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=280&section=header&text=Welcome%20to%20My%20Profile&fontSize=50&fontColor=ffffff&animation=twinkling&fontAlignY=35)
 
<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=36BCF7&width=700&lines=Hi+there%2C+I'm+Md.+Rafiul+Islam+%F0%9F%91%8B;%F0%9F%A4%96+IoT+%26+Robotics+Engineer+%7C+Embedded+Systems;%E2%9A%A1+C%2FC%2B%2B+%7C+Python+%7C+React+%7C+Flask;%F0%9F%9A%80+Building+Smart+Connected+Systems;%F0%9F%94%A5+Bridging+Hardware%2C+Software+%26+AI" alt="Typing SVG" />
</div>
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=6,11,20&height=2"/>
</div>

 
<div align="center">
## 🌟 About Me
 
</div>

 
<img align="right" alt="IoT Robot Animation" width="320" src="https://user-images.githubusercontent.com/74038190/229223263-cf2e4b07-2615-4f87-9c38-e37600f8381a.gif"/>

## 👨‍💻 About Me

- 🎓 **B.Sc. in IoT & Robotics Engineering** — University of Frontier Technology, Bangladesh
- 💼 **ML Intern** @ SYNTECXHUB (completed) | **Intern** @ BYSDO Ignite Program Batch-04 (completed) 
- 🤖 Passionate about **AI + IoT + Robotics integration**
- 🧠 Working on **IoT**, **Embedded systems**, **Machine Learning**, **Explainable AI** & **Computer Vision**
- 📸 Photographer @ UFTB Robotics Club | Social Media manager @ UFTB AI community

An **IoT & Robotics engineer** with a driving passion for **smart systems**, **IoT integration**, and **AI Engineer**.

---

Currently exploring **Embedded C/C++ systems**, **Computer Vision with OpenCV**, **Machine Learning** and **AI Engineering**,

## 🚀 Core Expertise
- 🔌 Embedded Systems (ESP32, Arduino, Raspberry Pi, PCB Design)
- 🤖 Robotics & Automation (LFR, Fire Fighting, Edge Detection Bots, Bike security systems)
- 🧠 Machine Learning, Weather agents & AI Voice Agents
- 👁️ Computer Vision (OpenCV)
- 🌐 Full-Stack Development (React, Flask, Node.js, Next.js)
- 📡 IoT Sensor Integration (IR, Ultrasonic, Flame, Soil, LDR, Temperature, Vibration)

<br clear="both"/>

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=11,6,20&height=2"/>
</div>

## 🛠️ Tech Stack

<div align="center">

### Languages
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### Frameworks & Tools
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-6DA55F?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=Arduino&logoColor=white)

### AI & ML
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![IBM Watson](https://img.shields.io/badge/IBM%20Watson-052FAD?style=for-the-badge&logo=ibmwatson&logoColor=white)

### Databases
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![Firebase](https://img.shields.io/badge/firebase-ffca28?style=for-the-badge&logo=firebase&logoColor=black)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)

### Hardware & OS
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=for-the-badge&logo=Raspberry%20Pi&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![PlatformIO](https://img.shields.io/badge/PlatformIO-FF7F00?style=for-the-badge&logo=platformio&logoColor=white)

</div>

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=20,11,6&height=2"/>
</div>

## 🚀 Featured Projects

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=FF6B6B&width=650&lines=Check+out+my+amazing+projects!;Building+the+future+with+code+%26+circuits!" alt="Projects Typing SVG" />
</div>

<table width="100%">
<tr>
<td width="50%">

### 🎬 CineMatch AI
**AI-powered movie recommendation engine** — Movie DNA Analysis, Hybrid Scoring (content 65% + Bayesian 28% + popularity 7%), mood-based discovery & Cinematic Analytics Dashboard.

[![Repo](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)](https://github.com/rafiul254/Cinemach-Ai)
[![Live](https://img.shields.io/badge/Live%20Demo-Hugging%20Face-FF9D00?style=for-the-badge&logo=huggingface&logoColor=white)](https://huggingface.co/spaces/Rafi-ul/cinematch-ai)

</td>
<td width="50%">

### 📸 SnapSage
**AI screenshot learning tracker** — Upload a screenshot, write your intent, AI returns topic name, explanation, key points & real-world applications. Personal knowledge vault.

[![Repo](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)](https://github.com/rafiul254/Snapsage)
[![Live](https://img.shields.io/badge/Live-Demo-success?style=for-the-badge&logo=vercel)](https://snap-sage-ashy.vercel.app/)

</td>
</tr>
<tr>
<td width="50%">

### 🌐 3D Portfolio Website
**Personal IoT-themed portfolio** — 3D floating Arduino boards, circuit traces, aurora animations built with Three.js r128. 14 certifications, fully responsive.

[![Repo](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)](https://github.com/rafiul254/Portfolio_website)
[![Live](https://img.shields.io/badge/Live-Demo-success?style=for-the-badge&logo=vercel)](https://portfolio-website-rafiul.vercel.app)

</td>
<td width="50%">

### 🔩 OopsStopper Robot v1.0
**DIY edge detection robot** — Autonomous table safety bot with IR sensors and real-time L298N motor control. Prevents falling off elevated surfaces.

[![Repo](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)](https://github.com/rafiul254/OopsStopper-v1.0)
[![Demo](https://img.shields.io/badge/YouTube-Demo-red?style=for-the-badge&logo=youtube)](https://youtube.com/shorts/E52RMUhqKQ4?si=1vqFae3mr7ajRSZh)

</td>
</tr>
<tr>
<td width="50%">

### 📊 HabitTracker 
**Modern JavaFX desktop app** — Habit tracking with analytics, 6 themes, monthly calendar, streak system & smart notifications. MVC architecture.

[![Repo](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)](https://github.com/rafiul254/HabitTracker)

</td>
<td width="50%">

### 🎬 ESP32 GIF Player
**Fullscreen GIF player on ESP32** — Animated GIFs on ST7735 TFT, stored in PROGMEM Flash (no SD card). 6 Marvel/Anime animations auto-cycling every 8s.

[![Repo](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)](https://github.com/rafiul254/ESP32-GIF-Player)
[![Demo](https://img.shields.io/badge/YouTube-Demo-red?style=for-the-badge&logo=youtube)](https://youtube.com/shorts/jHeiL1j6YvM)

</td>
</tr>
<tr>
<td colspan="2" align="center">

### 🛡️ System Argus AI
**AI-powered server failure prediction** — Real-time monitoring, anomaly detection & predictive analytics dashboard.

[![Repo](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)](https://github.com/rafiul254/System-Argus-AI)
[![Demo](https://img.shields.io/badge/YouTube-Demo-red?style=for-the-badge&logo=youtube)](https://youtu.be/KJxn4bfKvMA?si=tCHKFCotYkbVVAVa)

</td>
</tr>
</table>

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=6,20,11&height=2"/>
</div>

## 📊 GitHub Stats & Analytics
 
<div align="center">
<img src="https://github-readme-stats.vercel.app/api?username=rafiul254&show_icons=true&theme=radical&hide_border=true&bg_color=0D1117&title_color=F85D7F&icon_color=F8D866&text_color=a8b2d1" width="48%"/>
&nbsp;
<img src="https://streak-stats.demolab.com/?user=rafiul254&theme=radical&hide_border=true&background=0D1117&stroke=F85D7F&ring=F8D866&fire=F85D7F&currStreakLabel=F8D866" width="48%"/>
</div>
---
 
<div align="center">
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=rafiul254&layout=compact&theme=radical&hide_border=true&bg_color=0D1117&title_color=F85D7F&text_color=a8b2d1" width="60%"/>
</div>
<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=rafiul254&theme=react-dark&hide_border=true&bg_color=0D1117&area=true" width="98%"/>
</div>
---
 
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=11,20,6&height=2"/>
</div>

## 🏆 Achievements & Certifications

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=FFD700&width=700&lines=%F0%9F%8F%85+ICT+Olympiad+Bangladesh+%E2%80%94+Semi-Final+Round;%F0%9F%8F%86+ILC+National+Top+100+Winner;%F0%9F%A4%96+IoT+%26+Robotics+Contest+Third+Place" alt="Achievements Typing SVG" />
</div>

---

<div align="center">

| 🏅 **Achievement** | 🏢 **Institution** |
|:---|:---|
| 🥇 ICT Olympiad Bangladesh S3 — Semi-Final (Engineering) | ICT Olympiad BD |
| 🏆 International Leadership Competition — National Top 100 | ILC 1.0 |
| 🎓 ILC Champions Round — Certificate of Achievement | ILC 1.0 |
| 🧠 Machine Learning Internship | SYNTECXHUB | 
| 🤖 Master AI Voice Agents | Udemy |
| 💬 Build Your Own Chatbot | IBM Watson |
| ☁️ Innovating with Google Cloud AI | Simplilearn |
| 🔐 Certified Cybersecurity Educator (CCEP) | Red Team Leaders |
| 🐍 Python for Data Science | IBM |
| 🥉 IoT & Robotics Contest — Third Place | UFTB |
| 📐 3D Mechanical Design & Modeling | UFTB |
| 📊 Data Analysis (Excel & Power BI) | Data Solution-360 |
| 📡 Introduction to IoT | Cisco |
| 🛡️ Introduction to Data Science | Cisco |
| 🔌 PCB Designing Workshop | IEEE RAS IUT |
| 🤖 Prompt Engineering, AI & ML | GP Academy |
| ⚡ AI Automation | Ostad |
| 📈 Excel Mastery | GP Academy |
| 📚 Research Training | BARTC |
| ✍️ Essay Competition — Third Place | Islamic Foundation |

</div>

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=20,6,11&height=2"/>
</div>

## 🌐 Connect With Me

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=4ECDC4&width=500&lines=Let's+connect+and+collaborate!;Always+open+to+new+opportunities!+%F0%9F%9A%80" alt="Connect Typing SVG" />

<br/><br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rafiul-islam-25sep92004)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=firefox&logoColor=white)](https://portfolio-website-rafiul.vercel.app)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@rafiulislam25)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@pintocloud)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/share/1A37R9eh5H/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rafuulislam2004@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/rafiul254)

<br/>

### 💭 Quote
*"Code the mind. Build the circuit. Connect the world."*

<br/>

<img src="https://komarev.com/ghpvc/?username=rafiul254&color=blueviolet&style=for-the-badge&label=Profile+Views" alt="Profile Views" />

</div>

<br/>

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=36BCF7&width=560&lines=Thanks+for+visiting+my+profile!;Happy+coding+%26+building+smart+systems!+%F0%9F%9A%80" alt="Thanks Typing SVG" />
</div>

![Footer Wave](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer)
