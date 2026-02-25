![header](https://github.com/user-attachments/assets/0672137b-bdc1-4487-abae-b9fc1494a232)
<svg width="800" height="290" viewBox="0 0 800 290" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="wave" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#4c5fd7"/>
      <stop offset="100%" style="stop-color:#3b4cca"/>
    </linearGradient>
    <linearGradient id="pyBg" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#1c2640"/>
      <stop offset="100%" style="stop-color:#141c30"/>
    </linearGradient>
    <linearGradient id="javaBg" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#1e2a1e"/>
      <stop offset="100%" style="stop-color:#141e14"/>
    </linearGradient>
    <filter id="ts">
      <feDropShadow dx="1" dy="2" stdDeviation="2" flood-color="rgba(0,0,0,0.4)"/>
    </filter>
    <filter id="cs" x="-5%" y="-5%" width="110%" height="120%">
      <feDropShadow dx="0" dy="3" stdDeviation="5" flood-color="rgba(0,0,0,0.35)"/>
    </filter>
    <clipPath id="wc">
      <rect x="0" y="0" width="800" height="185"/>
    </clipPath>
  </defs>

  <style>
    .sf   { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif; }
    .mono { font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace; }

    .title { font-weight:800; font-size:44px; fill:#fff; filter:url(#ts); }
    .sub   { font-weight:500; font-size:15px; fill:rgba(255,255,255,.92); letter-spacing:1.2px; }
    .sub   { animation: pulse 4s ease-in-out infinite; }
    @keyframes pulse { 0%,100%{opacity:1} 50%{opacity:.6} }

    @keyframes r1 {
      0%   { transform:translate(  0px,  0px) scale(1.0); opacity:0 }
      7%   { opacity:.80 }
      30%  { transform:translate(  7px,-32px) scale(.94); opacity:.74 }
      58%  { transform:translate( -6px,-70px) scale(.84); opacity:.38 }
      84%  { transform:translate(  4px,-106px) scale(.68); opacity:.08 }
      100% { transform:translate(  0px,-126px) scale(.50); opacity:0 }
    }
    @keyframes r2 {
      0%   { transform:translate(  0px,  0px) scale(1.0); opacity:0 }
      7%   { opacity:.86 }
      27%  { transform:translate( -9px,-28px) scale(.96); opacity:.78 }
      55%  { transform:translate(  8px,-66px) scale(.86); opacity:.43 }
      80%  { transform:translate( -5px,-102px) scale(.70); opacity:.10 }
      100% { transform:translate(  2px,-122px) scale(.52); opacity:0 }
    }
    @keyframes r3 {
      0%   { transform:translate(  0px,  0px) scale(1.0); opacity:0 }
      9%   { opacity:.76 }
      33%  { transform:translate(  6px,-36px) scale(.93); opacity:.70 }
      62%  { transform:translate( -7px,-74px) scale(.82); opacity:.36 }
      86%  { transform:translate(  3px,-110px) scale(.67); opacity:.07 }
      100% { transform:translate( -2px,-126px) scale(.50); opacity:0 }
    }
    @keyframes r4 {
      0%   { transform:translate(  0px,  0px) scale(1.0); opacity:0 }
      8%   { opacity:.83 }
      26%  { transform:translate(-10px,-30px) scale(.95); opacity:.77 }
      54%  { transform:translate(  9px,-68px) scale(.85); opacity:.42 }
      79%  { transform:translate( -4px,-104px) scale(.70); opacity:.12 }
      100% { transform:translate(  2px,-120px) scale(.52); opacity:0 }
    }
    @keyframes r5 {
      0%   { transform:translate(  0px,  0px) scale(1.0); opacity:0 }
      9%   { opacity:.78 }
      35%  { transform:translate(  8px,-38px) scale(.92); opacity:.72 }
      63%  { transform:translate( -6px,-76px) scale(.83); opacity:.38 }
      87%  { transform:translate(  4px,-112px) scale(.66); opacity:.08 }
      100% { transform:translate( -1px,-126px) scale(.50); opacity:0 }
    }
    .bub { fill:rgba(110,128,248,.50); stroke:rgba(190,200,255,.38); stroke-width:1.2; }
    .b1  { animation: r1 3.4s cubic-bezier(.25,.46,.45,.94) infinite 0.0s; }
    .b2  { animation: r2 4.1s cubic-bezier(.25,.46,.45,.94) infinite 1.4s; }
    .b3  { animation: r3 3.7s cubic-bezier(.25,.46,.45,.94) infinite 0.7s; }
    .b4  { animation: r4 4.6s cubic-bezier(.25,.46,.45,.94) infinite 2.3s; }
    .b5  { animation: r5 4.0s cubic-bezier(.25,.46,.45,.94) infinite 1.9s; }

    @keyframes ci { from{opacity:0;transform:translateY(10px)} to{opacity:1;transform:translateY(0)} }
    .cp { animation: ci .65s ease-out .25s both; }
    .cj { animation: ci .65s ease-out .50s both; }

    .kw { fill:#569cd6; }
    .fn { fill:#dcdcaa; }
    .st { fill:#ce9178; }
    .tx { fill:#d4d4d4; }
    .co { fill:#6a9955; }
    .dm { fill:#606070; }
    .c  { font-size:12.5px; }
  </style>

  <!-- Wave -->
  <path fill="url(#wave)">
    <animate attributeName="d" dur="7s" repeatCount="indefinite" calcMode="spline"
      keySplines="0.45 0 0.55 1; 0.45 0 0.55 1"
      values="
        M0,0 H800 V112 C720,132 650,182 548,152 C446,122 348,162 248,132 C148,102 52,152 0,124 Z;
        M0,0 H800 V132 C752,112 682,142 580,172 C478,142 378,122 278,152 C178,182 80,122 0,142 Z;
        M0,0 H800 V112 C720,132 650,182 548,152 C446,122 348,162 248,132 C148,102 52,152 0,124 Z"/>
  </path>

  <!-- Bubbles -->
  <g clip-path="url(#wc)">
    <circle class="bub b1" cx="108" cy="136" r="11"/>
    <circle class="bub b2" cx="225" cy="130" r="14"/>
    <circle class="bub b3" cx="390" cy="136" r="13"/>
    <circle class="bub b4" cx="558" cy="150" r="16"/>
    <circle class="bub b5" cx="688" cy="164" r="12"/>
  </g>

  <!-- Title + subtitle -->
  <text x="400" y="68"  text-anchor="middle" class="sf title">NOME</text>
  <text x="400" y="104" text-anchor="middle" class="sf sub">Back-End Developer  •  Software Architecture  •  Tech</text>

  <!-- ── Python card ── -->
  <g class="cp" filter="url(#cs)">
    <rect x="14"  y="150" width="375" height="112" rx="9" fill="url(#pyBg)" stroke="rgba(90,120,210,.28)" stroke-width="1"/>
    <rect x="14"  y="150" width="375" height="27"  rx="9" fill="#1a2438"/>
    <rect x="14"  y="163" width="375" height="14"       fill="#1a2438"/>
    <circle cx="31" cy="164" r="5" fill="#ff5f57"/>
    <circle cx="47" cy="164" r="5" fill="#febc2e"/>
    <circle cx="63" cy="164" r="5" fill="#28c840"/>
    <text x="200" y="169" text-anchor="middle" class="mono" font-size="10" fill="#7a8faa">Main.py</text>
    <rect x="319" y="155" width="62" height="16" rx="4" fill="#3572A5"/>
    <text x="350" y="167" text-anchor="middle" class="mono" font-size="9.5" fill="#fff" font-weight="700">Python</text>

    <!-- print("Hello, Nome!") -->
    <text class="mono c" x="30" y="200">
      <tspan class="fn">print</tspan><tspan class="tx">(</tspan><tspan class="st">"Hello, World!"</tspan><tspan class="tx">)</tspan>
    </text>

    <!-- output -->
    <rect x="14" y="222" width="375" height="40" fill="#0c1322"/>
    <rect x="14" y="222" width="3"   height="40" fill="#569cd6" opacity=".8"/>
    <text class="mono" font-size="10" x="24" y="236" fill="#606070">OUTPUT</text>
    <text class="mono c"              x="24" y="253" fill="#6a9955">Hello, World!</text>
  </g>

  <!-- ── Java card ── -->
  <g class="cj" filter="url(#cs)">
    <rect x="411" y="150" width="375" height="112" rx="9" fill="url(#javaBg)" stroke="rgba(90,180,90,.22)" stroke-width="1"/>
    <rect x="411" y="150" width="375" height="27"  rx="9" fill="#192219"/>
    <rect x="411" y="163" width="375" height="14"       fill="#192219"/>
    <circle cx="428" cy="164" r="5" fill="#ff5f57"/>
    <circle cx="444" cy="164" r="5" fill="#febc2e"/>
    <circle cx="460" cy="164" r="5" fill="#28c840"/>
    <text x="597" y="169" text-anchor="middle" class="mono" font-size="10" fill="#6a9b6a">Main.java</text>
    <rect x="716" y="155" width="62" height="16" rx="4" fill="#b07219"/>
    <text x="747" y="167" text-anchor="middle" class="mono" font-size="9.5" fill="#fff" font-weight="700">Java</text>

    <!-- System.out.println("Hello, Nome!"); -->
    <text class="mono c" x="425" y="200">
      <tspan class="tx">System.out.</tspan><tspan class="fn">println</tspan><tspan class="tx">(</tspan><tspan class="st">"Hello, World!"</tspan><tspan class="tx">);</tspan>
    </text>

    <!-- output -->
    <rect x="411" y="222" width="375" height="40" fill="#0a110a"/>
    <rect x="411" y="222" width="3"   height="40" fill="#28c840" opacity=".8"/>
    <text class="mono" font-size="10" x="421" y="236" fill="#606070">OUTPUT</text>
    <text class="mono c"              x="421" y="253" fill="#6a9955">Hello, World!</text>
  </g>

</svg>

<img src="header.svg" alt="Meu Cabeçalho Animado" width="100%">
