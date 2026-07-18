<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
  viewBox="0 0 1180 610" width="1180" height="610" role="img" aria-label="Developer Profile Banner">

  <defs>
    <!-- Clip path for rounded corners -->
    <clipPath id="d-main-clip">
      <rect width="1180" height="610" rx="20" ry="20"/>
    </clipPath>
    <clipPath id="d-left-clip">
      <rect x="0" y="0" width="448" height="610"/>
    </clipPath>
    <clipPath id="d-right-clip">
      <rect x="448" y="0" width="732" height="610"/>
    </clipPath>
    <clipPath id="d-terminal-clip">
      <rect x="468" y="20" width="692" height="570" rx="14" ry="14"/>
    </clipPath>

    <!-- Background gradient -->
    <radialGradient id="d-bg-glow1" cx="25%" cy="30%" r="50%">
      <stop offset="0%" stop-color="#1e1065" stop-opacity="0.6"/>
      <stop offset="100%" stop-color="#030712" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="d-bg-glow2" cx="75%" cy="70%" r="45%">
      <stop offset="0%" stop-color="#0c4a6e" stop-opacity="0.5"/>
      <stop offset="100%" stop-color="#030712" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="d-bg-glow3" cx="50%" cy="50%" r="60%">
      <stop offset="0%" stop-color="#064e3b" stop-opacity="0.3"/>
      <stop offset="100%" stop-color="#030712" stop-opacity="0"/>
    </radialGradient>

    <!-- ASCII gradient (animated) -->
    <linearGradient id="d-ascii-grad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#22d3ee">
        <animate attributeName="stop-color" values="#22d3ee;#a78bfa;#34d399;#22d3ee" dur="4s" repeatCount="indefinite"/>
      </stop>
      <stop offset="50%" stop-color="#7c3aed">
        <animate attributeName="stop-color" values="#7c3aed;#22d3ee;#a78bfa;#7c3aed" dur="4s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" stop-color="#10b981">
        <animate attributeName="stop-color" values="#10b981;#7c3aed;#22d3ee;#10b981" dur="4s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>

    <!-- Terminal gradient -->
    <linearGradient id="d-terminal-grad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#0f172a"/>
      <stop offset="100%" stop-color="#080f1e"/>
    </linearGradient>

    <!-- Border shimmer gradient -->
    <linearGradient id="d-border-shimmer" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(124,58,237,0)"/>
      <stop offset="30%" stop-color="rgba(34,211,238,0.6)"/>
      <stop offset="60%" stop-color="rgba(124,58,237,0.6)"/>
      <stop offset="100%" stop-color="rgba(16,185,129,0)"/>
      <animateTransform attributeName="gradientTransform" type="translate" from="-1 0" to="1 0" dur="3s" repeatCount="indefinite"/>
    </linearGradient>

    <!-- Glow filter for ASCII -->
    <filter id="d-ascii-glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="2" result="blur1"/>
      <feGaussianBlur stdDeviation="4" result="blur2"/>
      <feMerge>
        <feMergeNode in="blur2"/>
        <feMergeNode in="blur1"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Glow filter for panels -->
    <filter id="d-panel-glow" x="-5%" y="-5%" width="110%" height="110%">
      <feGaussianBlur stdDeviation="8" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Pill glow filter -->
    <filter id="d-pill-glow" x="-10%" y="-20%" width="120%" height="140%">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Scanline pattern -->
    <pattern id="d-scanlines" x="0" y="0" width="1" height="4" patternUnits="userSpaceOnUse">
      <line x1="0" y1="0" x2="1" y2="0" stroke="rgba(0,0,0,0.15)" stroke-width="1"/>
    </pattern>

    <!-- Noise texture via turbulence -->
    <filter id="d-noise" x="0" y="0" width="100%" height="100%">
      <feTurbulence type="fractalNoise" baseFrequency="0.65" numOctaves="3" stitchTiles="stitch" result="noise"/>
      <feColorMatrix type="saturate" values="0" in="noise" result="grayNoise"/>
      <feBlend in="SourceGraphic" in2="grayNoise" mode="overlay" result="blend"/>
      <feComposite in="blend" in2="SourceGraphic" operator="in"/>
    </filter>

    <!-- Glass reflection gradient -->
    <linearGradient id="d-glass-reflect" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.06)"/>
      <stop offset="40%" stop-color="rgba(255,255,255,0.02)"/>
      <stop offset="100%" stop-color="rgba(255,255,255,0)"/>
    </linearGradient>

    <!-- Left panel gradient -->
    <linearGradient id="d-left-panel-grad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0a0f1e"/>
      <stop offset="100%" stop-color="#050b16"/>
    </linearGradient>

    <!-- Accent gradient for text -->
    <linearGradient id="d-accent-grad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#7c3aed"/>
      <stop offset="50%" stop-color="#22d3ee"/>
      <stop offset="100%" stop-color="#10b981"/>
    </linearGradient>

    <!-- Skill pill gradient -->
    <linearGradient id="d-pill-react" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(34,211,238,0.15)"/>
      <stop offset="100%" stop-color="rgba(34,211,238,0.05)"/>
    </linearGradient>
    <linearGradient id="d-pill-next" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(124,58,237,0.15)"/>
      <stop offset="100%" stop-color="rgba(124,58,237,0.05)"/>
    </linearGradient>
    <linearGradient id="d-pill-node" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(16,185,129,0.15)"/>
      <stop offset="100%" stop-color="rgba(16,185,129,0.05)"/>
    </linearGradient>

    <!-- Particle glow -->
    <radialGradient id="d-particle-glow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#22d3ee" stop-opacity="0.8"/>
      <stop offset="100%" stop-color="#22d3ee" stop-opacity="0"/>
    </radialGradient>

    <!-- Mask for sequential reveal -->
    <mask id="d-reveal-mask-1">
      <rect x="0" y="0" width="1180" height="610" fill="white">
        <animate attributeName="opacity" values="0;1" dur="0.1s" begin="0.5s" fill="freeze"/>
      </rect>
    </mask>

  </defs>

  <!-- ═══════════════════════════════════════════ -->
  <!-- MAIN CANVAS                                  -->
  <!-- ═══════════════════════════════════════════ -->
  <g clip-path="url(#d-main-clip)">

    <!-- Base background -->
    <rect width="1180" height="610" fill="#030712"/>

    <!-- Background glows -->
    <rect width="1180" height="610" fill="url(#d-bg-glow1)">
      <animateTransform attributeName="transform" type="translate" values="0,0;20,10;0,0" dur="8s" repeatCount="indefinite"/>
    </rect>
    <rect width="1180" height="610" fill="url(#d-bg-glow2)">
      <animateTransform attributeName="transform" type="translate" values="0,0;-15,8;0,0" dur="10s" repeatCount="indefinite"/>
    </rect>
    <rect width="1180" height="610" fill="url(#d-bg-glow3)">
      <animateTransform attributeName="transform" type="translate" values="0,0;10,-12;0,0" dur="12s" repeatCount="indefinite"/>
    </rect>

    <!-- Scanlines overlay -->
    <rect width="1180" height="610" fill="url(#d-scanlines)" opacity="0.4"/>

    <!-- Animated particles -->
    <g opacity="0.6">
      <!-- Particle 1 -->
      <circle r="2" fill="url(#d-particle-glow)" opacity="0">
        <animate attributeName="cx" values="120;140;120" dur="7s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="80;60;80" dur="7s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.8;0" dur="7s" repeatCount="indefinite"/>
      </circle>
      <!-- Particle 2 -->
      <circle r="1.5" fill="#a78bfa" opacity="0">
        <animate attributeName="cx" values="300;280;300" dur="9s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="150;130;150" dur="9s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.7;0" dur="9s" repeatCount="indefinite"/>
      </circle>
      <!-- Particle 3 -->
      <circle r="1" fill="#34d399" opacity="0">
        <animate attributeName="cx" values="200;220;200" dur="11s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="400;380;400" dur="11s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.6;0" dur="11s" repeatCount="indefinite"/>
      </circle>
      <!-- Particle 4 -->
      <circle r="2" fill="#22d3ee" opacity="0">
        <animate attributeName="cx" values="80;100;80" dur="6s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="450;470;450" dur="6s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.5;0" dur="6s" repeatCount="indefinite"/>
      </circle>
      <!-- More particles right side -->
      <circle r="1.5" fill="#7c3aed" opacity="0">
        <animate attributeName="cx" values="800;820;800" dur="8s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="100;80;100" dur="8s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.6;0" dur="8s" repeatCount="indefinite"/>
      </circle>
      <circle r="1" fill="#22d3ee" opacity="0">
        <animate attributeName="cx" values="1050;1030;1050" dur="10s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="200;220;200" dur="10s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.5;0" dur="10s" repeatCount="indefinite"/>
      </circle>
      <circle r="2" fill="#10b981" opacity="0">
        <animate attributeName="cx" values="950;970;950" dur="13s" repeatCount="indefinite"/>
        <animate attributeName="cy" values="500;480;500" dur="13s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.4;0" dur="13s" repeatCount="indefinite"/>
      </circle>
    </g>

    <!-- ═══════════════════════════════════════════ -->
    <!-- LEFT PANEL — ASCII Terminal                  -->
    <!-- ═══════════════════════════════════════════ -->
    <g clip-path="url(#d-left-clip)">

      <!-- Left panel background -->
      <rect x="0" y="0" width="448" height="610" fill="url(#d-left-panel-grad)"/>

      <!-- Left panel border right -->
      <line x1="447" y1="0" x2="447" y2="610" stroke="rgba(255,255,255,0.06)" stroke-width="1"/>

      <!-- Animated vertical shimmer on border -->
      <line x1="447" y1="0" x2="447" y2="610" stroke="url(#d-border-shimmer)" stroke-width="1.5" opacity="0.5">
        <animate attributeName="opacity" values="0.2;0.8;0.2" dur="3s" repeatCount="indefinite"/>
      </line>

      <!-- Glass reflection overlay -->
      <rect x="0" y="0" width="448" height="200" fill="url(#d-glass-reflect)"/>

      <!-- Terminal header bar -->
      <rect x="0" y="0" width="448" height="36" fill="rgba(255,255,255,0.03)"/>
      <line x1="0" y1="36" x2="448" y2="36" stroke="rgba(255,255,255,0.06)" stroke-width="1"/>

      <!-- Terminal dots -->
      <circle cx="22" cy="18" r="5" fill="#ff5f57"/>
      <circle cx="40" cy="18" r="5" fill="#febc2e"/>
      <circle cx="58" cy="18" r="5" fill="#28c840"/>

      <!-- Terminal title -->
      <text x="224" y="22" font-family="'SF Mono', 'Fira Code', monospace" font-size="11" fill="rgba(255,255,255,0.3)" text-anchor="middle">~/ascii-portrait.sh</text>

      <!-- Moving scanline sweep -->
      <rect x="0" y="36" width="448" height="3" fill="rgba(34,211,238,0.08)">
        <animate attributeName="y" values="36;610;36" dur="6s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0;0.5;0" dur="6s" repeatCount="indefinite"/>
      </rect>

      <!-- ASCII Portrait — Line by line reveal with gradient -->
      <!-- Using a mask approach for line reveals -->
      <g font-family="'SF Mono', 'Fira Code', 'Courier New', monospace" font-size="8.2" filter="url(#d-ascii-glow)">
        <defs>
          <mask id="d-ascii-line1"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="0.3s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line2"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="0.45s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line3"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="0.6s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line4"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="0.75s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line5"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="0.9s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line6"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.05s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line7"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.2s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line8"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.35s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line9"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.5s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line10"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.65s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line11"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.8s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line12"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="1.95s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line13"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.1s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line14"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.25s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line15"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.4s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line16"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.55s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line17"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.7s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line18"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="2.85s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line19"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.0s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line20"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.15s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line21"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.3s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line22"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.45s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line23"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.6s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line24"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.75s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line25"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="3.9s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line26"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="4.05s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line27"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="4.2s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line28"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="4.35s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line29"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="4.5s" fill="freeze"/></rect></mask>
          <mask id="d-ascii-line30"><rect x="0" y="0" width="448" height="610" fill="white" opacity="0"><animate attributeName="opacity" values="0;1" dur="0.05s" begin="4.65s" fill="freeze"/></rect></mask>
        </defs>

        <!-- Floating animation wrapper -->
        <g>
          <animateTransform attributeName="transform" type="translate" values="0,0;0,-5;0,0" dur="5s" repeatCount="indefinite"/>

          <!-- ASCII lines with gradient fill -->
          <text x="24" y="64" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line1)">  ██████╗ ███████╗██╗   ██╗</text>
          <text x="24" y="76" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line2)">  ██╔══██╗██╔════╝██║   ██║</text>
          <text x="24" y="88" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line3)">  ██║  ██║█████╗  ██║   ██║</text>
          <text x="24" y="100" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line4)">  ██║  ██║██╔══╝  ╚██╗ ██╔╝</text>
          <text x="24" y="112" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line5)">  ██████╔╝███████╗ ╚████╔╝</text>
          <text x="24" y="124" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line6)">  ╚═════╝ ╚══════╝  ╚═══╝</text>
          <text x="24" y="148" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line7)">   ░░░░░░░░░░░░░░░░░░░░░░░</text>
          <text x="24" y="160" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line8)">  ╔═══════════════════════╗</text>
          <text x="24" y="172" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line9)">  ║  ╭──────────────────╮  ║</text>
          <text x="24" y="184" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line10)">  ║  │  ◉  ◉           │  ║</text>
          <text x="24" y="196" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line11)">  ║  │    ╭──╮          │  ║</text>
          <text x="24" y="208" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line12)">  ║  │    │  │          │  ║</text>
          <text x="24" y="220" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line13)">  ║  │  ╰────╯          │  ║</text>
          <text x="24" y="232" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line14)">  ║  │ ╭──────────────╮ │  ║</text>
          <text x="24" y="244" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line15)">  ║  ╰──────────────────╯  ║</text>
          <text x="24" y="268" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line16)">  ╚═══════════════════════╝</text>
          <text x="24" y="292" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line17)">  ▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄</text>
          <text x="24" y="316" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line18)">  ▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀</text>
          <text x="24" y="340" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line19)">  ┌───────────────────────┐</text>
          <text x="24" y="352" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line20)">  │  &gt; developer.exe       │</text>
          <text x="24" y="364" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line21)">  │  &gt; loading modules...  │</text>
          <text x="24" y="376" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line22)">  │  &gt; [████████████] 100% │</text>
          <text x="24" y="388" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line23)">  │  &gt; ready               │</text>
          <text x="24" y="400" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line24)">  └───────────────────────┘</text>
          <text x="24" y="424" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line25)">  ·  ·  ·  ·  ·  ·  ·  ·</text>
          <text x="24" y="448" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line26)">  ◆  open to opportunities</text>
          <text x="24" y="472" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line27)">  ◆  building the future</text>
          <text x="24" y="496" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line28)">  ◆  one commit at a time</text>
          <text x="24" y="520" fill="url(#d-ascii-grad)" mask="url(#d-ascii-line29)">  ·  ·  ·  ·  ·  ·  ·  ·</text>
          <!-- Cursor -->
          <text x="24" y="544" fill="#22d3ee" mask="url(#d-ascii-line30)">  $<tspan fill="#22d3ee" font-size="8.2"> ▌</tspan>
            <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>
          </text>
        </g>
      </g>

      <!-- Left panel bottom gradient fade -->
      <rect x="0" y="540" width="448" height="70" fill="url(#d-left-panel-grad)" opacity="0.9"/>

    </g>

    <!-- ═══════════════════════════════════════════ -->
    <!-- RIGHT PANEL — Terminal Window               -->
    <!-- ═══════════════════════════════════════════ -->
    <g clip-path="url(#d-right-clip)">

      <!-- Terminal window outer glow -->
      <rect x="462" y="14" width="704" height="582" rx="16" ry="16" fill="none" stroke="rgba(124,58,237,0.3)" stroke-width="1" filter="url(#d-panel-glow)">
        <animate attributeName="stroke-opacity" values="0.2;0.5;0.2" dur="4s" repeatCount="indefinite"/>
      </rect>

      <!-- Terminal window body -->
      <rect x="468" y="20" width="692" height="570" rx="14" ry="14" fill="url(#d-terminal-grad)"/>

      <!-- Terminal border shimmer -->
      <rect x="468" y="20" width="692" height="570" rx="14" ry="14" fill="none" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>
      <rect x="468" y="20" width="692" height="2" rx="1" ry="1" fill="url(#d-border-shimmer)" opacity="0.6"/>

      <!-- Glass reflection on terminal -->
      <rect x="468" y="20" width="692" height="200" rx="14" ry="14" fill="url(#d-glass-reflect)" clip-path="url(#d-terminal-clip)"/>

      <!-- Terminal header -->
      <rect x="468" y="20" width="692" height="42" rx="14" ry="14" fill="rgba(255,255,255,0.03)" clip-path="url(#d-terminal-clip)"/>
      <rect x="468" y="50" width="692" height="12" fill="rgba(255,255,255,0.03)" clip-path="url(#d-terminal-clip)"/>
      <line x1="468" y1="62" x2="1160" y2="62" stroke="rgba(255,255,255,0.06)" stroke-width="1"/>

      <!-- Window control dots -->
      <circle cx="490" cy="41" r="5.5" fill="#ff5f57"/>
      <circle cx="508" cy="41" r="5.5" fill="#febc2e"/>
      <circle cx="526" cy="41" r="5.5" fill="#28c840"/>

      <!-- Terminal title -->
      <text x="814" y="46" font-family="'SF Mono','Fira Code',monospace" font-size="12" fill="rgba(255,255,255,0.25)" text-anchor="middle">~/portfolio — zsh</text>

      <!-- ─── CONTENT AREA ─── -->
      <g clip-path="url(#d-terminal-clip)">

        <!-- Prompt line -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.1s" begin="1.0s" fill="freeze"/>
          <text x="492" y="92" font-family="'SF Mono','Fira Code',monospace" font-size="12" fill="#7c3aed">❯</text>
          <text x="506" y="92" font-family="'SF Mono','Fira Code',monospace" font-size="12" fill="#22d3ee">whoami</text>
        </g>

        <!-- Greeting -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.1s" begin="1.3s" fill="freeze"/>
          <text x="492" y="120" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="14" fill="rgba(148,163,184,0.8)" letter-spacing="0.05em">Hi 👋  Welcome to my terminal</text>
        </g>

        <!-- Name -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.1s" begin="1.6s" fill="freeze"/>
          <text x="492" y="158" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="34" font-weight="700" fill="url(#d-accent-grad)" letter-spacing="-0.02em">Alex Chen</text>
        </g>

        <!-- Animated typing subtitle -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.1s" begin="2.0s" fill="freeze"/>
          <text x="492" y="190" font-family="'SF Mono','Fira Code',monospace" font-size="15" fill="#22d3ee">
            <tspan id="d-typing-text">Frontend Engineer</tspan>
          </text>
          <!-- Cycling text via animate -->
          <text x="492" y="190" font-family="'SF Mono','Fira Code',monospace" font-size="15" fill="#22d3ee">
            <animate attributeName="opacity" values="1;1;0;0;0;0;0;0;0;0" dur="10s" repeatCount="indefinite" begin="2.0s"/>Frontend Engineer</text>
          <text x="492" y="190" font-family="'SF Mono','Fira Code',monospace" font-size="15" fill="#a78bfa" opacity="0">
            <animate attributeName="opacity" values="0;0;1;1;0;0;0;0;0;0" dur="10s" repeatCount="indefinite" begin="2.0s"/>Full Stack Developer</text>
          <text x="492" y="190" font-family="'SF Mono','Fira Code',monospace" font-size="15" fill="#34d399" opacity="0">
            <animate attributeName="opacity" values="0;0;0;0;1;1;0;0;0;0" dur="10s" repeatCount="indefinite" begin="2.0s"/>Open Source Contributor</text>
          <text x="492" y="190" font-family="'SF Mono','Fira Code',monospace" font-size="15" fill="#f59e0b" opacity="0">
            <animate attributeName="opacity" values="0;0;0;0;0;0;1;1;0;0" dur="10s" repeatCount="indefinite" begin="2.0s"/>UI / AI Enthusiast</text>
          <text x="492" y="190" font-family="'SF Mono','Fira Code',monospace" font-size="15" fill="#22d3ee" opacity="0">
            <animate attributeName="opacity" values="0;0;0;0;0;0;0;0;1;1" dur="10s" repeatCount="indefinite" begin="2.0s"/>Frontend Engineer</text>

          <!-- Typing cursor for subtitle -->
          <rect x="0" y="175" width="2" height="18" fill="#22d3ee">
            <animate attributeName="opacity" values="1;0;1" dur="0.8s" repeatCount="indefinite"/>
            <animate attributeName="x" values="696;696" dur="10s" repeatCount="indefinite" begin="2.0s"/>
          </rect>
        </g>

        <!-- Divider -->
        <line x1="492" y1="206" x2="1148" y2="206" stroke="rgba(255,255,255,0.06)" stroke-width="1" opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="2.4s" fill="freeze"/>
        </line>

        <!-- Info items -->
        <!-- Location -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="2.6s" fill="freeze"/>
          <text x="492" y="232" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#7c3aed">📍</text>
          <text x="516" y="232" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#94a3b8">San Francisco, CA</text>
        </g>

        <!-- Education -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="2.9s" fill="freeze"/>
          <text x="492" y="254" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#22d3ee">🎓</text>
          <text x="516" y="254" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#94a3b8">CS @ MIT</text>
        </g>

        <!-- Current Focus -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="3.2s" fill="freeze"/>
          <text x="492" y="276" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#10b981">⚡</text>
          <text x="516" y="276" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#94a3b8">Building AI-powered dev tools</text>
        </g>

        <!-- Portfolio -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="3.5s" fill="freeze"/>
          <text x="492" y="298" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#a78bfa">🌐</text>
          <text x="516" y="298" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#94a3b8">alexchen.dev</text>
        </g>

        <!-- Email -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="3.8s" fill="freeze"/>
          <text x="492" y="320" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#f59e0b">✉</text>
          <text x="516" y="320" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="12.5" fill="#94a3b8">alex@alexchen.dev</text>
        </g>

        <!-- Divider 2 -->
        <line x1="492" y1="340" x2="1148" y2="340" stroke="rgba(255,255,255,0.06)" stroke-width="1" opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="4.1s" fill="freeze"/>
        </line>

        <!-- Skills label -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="4.3s" fill="freeze"/>
          <text x="492" y="364" font-family="'SF Mono','Fira Code',monospace" font-size="10" fill="rgba(148,163,184,0.5)" letter-spacing="0.15em">SKILLS</text>
        </g>

        <!-- Skill Pills Row 1 -->
        <g filter="url(#d-pill-glow)" opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.6s" fill="freeze"/>

          <!-- React -->
          <rect x="492" y="374" width="60" height="24" rx="12" fill="url(#d-pill-react)" stroke="rgba(34,211,238,0.3)" stroke-width="1"/>
          <text x="522" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#22d3ee" text-anchor="middle">React</text>

          <!-- Next.js -->
          <rect x="560" y="374" width="64" height="24" rx="12" fill="url(#d-pill-next)" stroke="rgba(124,58,237,0.3)" stroke-width="1"/>
          <text x="592" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#a78bfa" text-anchor="middle">Next.js</text>

          <!-- Node.js -->
          <rect x="632" y="374" width="64" height="24" rx="12" fill="url(#d-pill-node)" stroke="rgba(16,185,129,0.3)" stroke-width="1"/>
          <text x="664" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#10b981" text-anchor="middle">Node.js</text>

          <!-- TypeScript -->
          <rect x="704" y="374" width="82" height="24" rx="12" fill="url(#d-pill-react)" stroke="rgba(34,211,238,0.3)" stroke-width="1"/>
          <text x="745" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#22d3ee" text-anchor="middle">TypeScript</text>

          <!-- Tailwind -->
          <rect x="794" y="374" width="70" height="24" rx="12" fill="url(#d-pill-next)" stroke="rgba(124,58,237,0.3)" stroke-width="1"/>
          <text x="829" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#a78bfa" text-anchor="middle">Tailwind</text>

          <!-- Python -->
          <rect x="872" y="374" width="60" height="24" rx="12" fill="url(#d-pill-node)" stroke="rgba(16,185,129,0.3)" stroke-width="1"/>
          <text x="902" y="390" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#10b981" text-anchor="middle">Python</text>
        </g>

        <!-- Skill Pills Row 2 -->
        <g filter="url(#d-pill-glow)" opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.9s" fill="freeze"/>

          <!-- Docker -->
          <rect x="492" y="406" width="62" height="24" rx="12" fill="url(#d-pill-react)" stroke="rgba(34,211,238,0.25)" stroke-width="1"/>
          <text x="523" y="422" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#22d3ee" text-anchor="middle">Docker</text>

          <!-- Postgres -->
          <rect x="562" y="406" width="70" height="24" rx="12" fill="url(#d-pill-next)" stroke="rgba(124,58,237,0.25)" stroke-width="1"/>
          <text x="597" y="422" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#a78bfa" text-anchor="middle">Postgres</text>

          <!-- AWS -->
          <rect x="640" y="406" width="50" height="24" rx="12" fill="url(#d-pill-node)" stroke="rgba(16,185,129,0.25)" stroke-width="1"/>
          <text x="665" y="422" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#10b981" text-anchor="middle">AWS</text>

          <!-- Git -->
          <rect x="698" y="406" width="44" height="24" rx="12" fill="url(#d-pill-react)" stroke="rgba(34,211,238,0.25)" stroke-width="1"/>
          <text x="720" y="422" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#22d3ee" text-anchor="middle">Git</text>

          <!-- Figma -->
          <rect x="750" y="406" width="56" height="24" rx="12" fill="url(#d-pill-next)" stroke="rgba(124,58,237,0.25)" stroke-width="1"/>
          <text x="778" y="422" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="11" fill="#a78bfa" text-anchor="middle">Figma</text>
        </g>

        <!-- Pulsing glow on pills -->
        <rect x="492" y="370" width="500" height="68" rx="6" fill="none" opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.1s" begin="5.2s" fill="freeze"/>
          <animate attributeName="fill" values="rgba(34,211,238,0.02);rgba(124,58,237,0.02);rgba(34,211,238,0.02)" dur="4s" repeatCount="indefinite"/>
        </rect>

        <!-- Divider 3 -->
        <line x1="492" y1="448" x2="1148" y2="448" stroke="rgba(255,255,255,0.06)" stroke-width="1" opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="5.3s" fill="freeze"/>
        </line>

        <!-- Social label -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="5.5s" fill="freeze"/>
          <text x="492" y="472" font-family="'SF Mono','Fira Code',monospace" font-size="10" fill="rgba(148,163,184,0.5)" letter-spacing="0.15em">CONNECT</text>
        </g>

        <!-- Social Icons -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.4s" begin="5.7s" fill="freeze"/>

          <!-- GitHub icon area -->
          <g filter="url(#d-pill-glow)">
            <!-- GitHub -->
            <rect x="492" y="484" width="100" height="36" rx="18" fill="rgba(255,255,255,0.04)" stroke="rgba(255,255,255,0.1)" stroke-width="1"/>
            <text x="508" y="505" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="rgba(148,163,184,0.8)">⬡ GitHub</text>
            <animate attributeName="opacity" values="0.8;1;0.8" dur="3s" repeatCount="indefinite"/>
          </g>
          <g filter="url(#d-pill-glow)">
            <!-- LinkedIn -->
            <rect x="600" y="484" width="100" height="36" rx="18" fill="rgba(255,255,255,0.04)" stroke="rgba(255,255,255,0.1)" stroke-width="1"/>
            <text x="613" y="505" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="rgba(148,163,184,0.8)">⬡ LinkedIn</text>
            <animate attributeName="opacity" values="0.8;1;0.8" dur="3s" begin="0.5s" repeatCount="indefinite"/>
          </g>
          <g filter="url(#d-pill-glow)">
            <!-- Twitter -->
            <rect x="708" y="484" width="100" height="36" rx="18" fill="rgba(255,255,255,0.04)" stroke="rgba(255,255,255,0.1)" stroke-width="1"/>
            <text x="728" y="505" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="rgba(148,163,184,0.8)">⬡ Twitter</text>
            <animate attributeName="opacity" values="0.8;1;0.8" dur="3s" begin="1.0s" repeatCount="indefinite"/>
          </g>
          <g filter="url(#d-pill-glow)">
            <!-- Portfolio -->
            <rect x="816" y="484" width="100" height="36" rx="18" fill="rgba(255,255,255,0.04)" stroke="rgba(124,58,237,0.3)" stroke-width="1"/>
            <text x="826" y="505" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="#a78bfa">⬡ Portfolio</text>
            <animate attributeName="opacity" values="0.8;1;0.8" dur="3s" begin="1.5s" repeatCount="indefinite"/>
          </g>
        </g>

        <!-- Bottom prompt -->
        <g opacity="0">
          <animate attributeName="opacity" values="0;1" dur="0.3s" begin="6.0s" fill="freeze"/>
          <text x="492" y="544" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="#7c3aed">❯ </text>
          <text x="506" y="544" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="#22d3ee">git commit -m </text>
          <text x="680" y="544" font-family="'SF Mono','Fira Code',monospace" font-size="11" fill="#10b981">"always be building"</text>
          <!-- Cursor -->
          <rect x="860" y="531" width="2" height="14" fill="#22d3ee">
            <animate attributeName="opacity" values="1;0;1" dur="0.8s" repeatCount="indefinite"/>
          </rect>
        </g>

        <!-- Moving scanline in terminal -->
        <rect x="468" y="62" width="692" height="2" fill="rgba(34,211,238,0.05)" clip-path="url(#d-terminal-clip)">
          <animate attributeName="y" values="62;590;62" dur="8s" repeatCount="indefinite"/>
        </rect>

      </g><!-- end terminal clip -->

    </g><!-- end right clip -->

    <!-- ═══════════════════════════════════════════ -->
    <!-- OUTER BORDER SHIMMER                        -->
    <!-- ═══════════════════════════════════════════ -->
    <rect width="1180" height="610" rx="20" ry="20" fill="none" stroke="rgba(255,255,255,0.06)" stroke-width="1.5"/>
    <!-- Top border shimmer -->
    <rect x="0" y="0" width="1180" height="1.5" rx="1" fill="url(#d-border-shimmer)" opacity="0.7"/>
    <!-- Bottom border shimmer -->
    <rect x="0" y="608.5" width="1180" height="1.5" rx="1" fill="url(#d-border-shimmer)" opacity="0.4"/>

  </g><!-- end main clip -->

</svg>
