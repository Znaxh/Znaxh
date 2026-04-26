<?xml version="1.0" encoding="utf-8"?>
<svg width="830" height="460" viewBox="0 0 830 460" fill="none" xmlns="http://www.w3.org/2000/svg">
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Share+Tech+Mono&amp;display=swap');
    * { font-family: 'Share Tech Mono', 'Courier New', monospace; }
    .bg       { fill: #0c110c; }
    .border   { fill: none; stroke: #2a5c2a; stroke-width: 1; }
    .border2  { fill: none; stroke: #1a3a1a; stroke-width: 1; stroke-dasharray: 4 3; }
    .dim      { fill: #2a5c2a; }
    .mid      { fill: #4a8c4a; }
    .bright   { fill: #6db86b; }
    .label    { fill: #2a5c2a; font-size: 11px; letter-spacing: 0.08em; text-transform: uppercase; }
    .key      { fill: #4a8c4a; font-size: 13px; }
    .val      { fill: #6db86b; font-size: 13px; }
    .name     { fill: #6db86b; font-size: 32px; letter-spacing: 0.12em; }
    .role     { fill: #4a8c4a; font-size: 13px; letter-spacing: 0.06em; }
    .sep      { fill: none; stroke: #1a3a1a; stroke-width: 1; }
    .stat-n   { fill: #6db86b; font-size: 22px; }
    .stat-l   { fill: #2a5c2a; font-size: 10px; letter-spacing: 0.1em; text-transform: uppercase; }
    .dot-l    { fill: #2a5c2a; font-size: 13px; }
    .cursor   { fill: #6db86b; }
  </style>

  <!-- Background -->
  <rect width="830" height="460" class="bg"/>

  <!-- Outer border -->
  <rect x="16" y="16" width="798" height="428" rx="2" class="border"/>

  <!-- Top bar -->
  <rect x="16" y="16" width="798" height="36" rx="2" fill="#0e140e"/>
  <line x1="16" y1="52" x2="814" y2="52" class="sep"/>

  <!-- Window controls -->
  <circle cx="38" cy="34" r="5" fill="#1a3a1a"/>
  <circle cx="56" cy="34" r="5" fill="#1a3a1a"/>
  <circle cx="74" cy="34" r="5" fill="#2a5c2a"/>

  <!-- Title bar text -->
  <text x="415" y="38" text-anchor="middle" class="label">znaxh — profile.sh</text>

  <!-- Left panel divider -->
  <line x1="290" y1="52" x2="290" y2="444" class="sep"/>

  <!-- ─── LEFT PANEL ─── -->

  <!-- Prompt line -->
  <text x="36" y="84" class="label">session</text>
  <text x="36" y="104" class="key">~/znaxh</text>
  <text x="112" y="104" class="dim"> ❯ </text>
  <text x="136" y="104" class="bright">whoami</text>

  <!-- Separator -->
  <line x1="36" y1="118" x2="268" y2="118" class="border2"/>

  <!-- Name block -->
  <text x="36" y="152" class="name">ANURAG</text>
  <text x="36" y="172" class="role">backend engineer  /  system architect</text>

  <!-- Separator -->
  <line x1="36" y1="186" x2="268" y2="186" class="border2"/>

  <!-- Info table -->
  <text x="36"  y="210" class="key">os        </text><text x="138" y="210" class="val" id="os_data">arch linux</text>
  <text x="36"  y="230" class="key">editor    </text><text x="138" y="230" class="val" id="editor_data">neovim</text>
  <text x="36"  y="250" class="key">stack     </text><text x="138" y="250" class="val" id="stack_data">py · ts · sql</text>
  <text x="36"  y="270" class="key">location  </text><text x="138" y="270" class="val" id="loc_data">india</text>
  <text x="36"  y="290" class="key">status    </text><text x="138" y="290" class="val" id="status_data">[ building ]</text>

  <!-- Separator -->
  <line x1="36" y1="304" x2="268" y2="304" class="border2"/>

  <!-- Social links -->
  <text x="36" y="326" class="label">links</text>
  <text x="36" y="346" class="key">gh  </text><text x="70" y="346" class="val">github.com/znaxh</text>
  <text x="36" y="366" class="key">in  </text><text x="70" y="366" class="val" id="linkedin_data">linkedin.com/in/—</text>
  <text x="36" y="386" class="key">web </text><text x="70" y="386" class="val" id="web_data">znaxh.dev</text>
  <text x="36" y="406" class="key">mail</text><text x="70" y="406" class="val" id="mail_data">—@gmail.com</text>

  <!-- Blinking cursor -->
  <rect x="36" y="424" width="8" height="13" class="cursor" opacity="0.9">
    <animate attributeName="opacity" values="0.9;0;0.9" dur="1.2s" repeatCount="indefinite"/>
  </rect>

  <!-- ─── RIGHT PANEL ─── -->

  <!-- Stats header -->
  <text x="314" y="80" class="label">git log —stats</text>

  <!-- Stat boxes row 1 -->
  <!-- Commits -->
  <rect x="314" y="92" width="148" height="72" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="328" y="115" class="stat-l">commits</text>
  <text x="328" y="146" class="stat-n" id="commit_data">—,———</text>
  <text x="328" y="158" class="dot-l" id="commit_data_dots"></text>

  <!-- Stars -->
  <rect x="474" y="92" width="148" height="72" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="488" y="115" class="stat-l">stars earned</text>
  <text x="488" y="146" class="stat-n" id="star_data">——</text>

  <!-- Repos -->
  <rect x="634" y="92" width="164" height="72" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="648" y="115" class="stat-l">repositories</text>
  <text x="648" y="146" class="stat-n" id="repo_data">——</text>

  <!-- Separator -->
  <line x1="314" y1="176" x2="796" y2="176" class="border2"/>

  <!-- Lines of code -->
  <text x="314" y="200" class="label">loc  ·  lines of code written</text>

  <text x="314" y="228" class="key">total   </text>
  <text x="380" y="228" class="dot-l" id="loc_data_dots">...................</text>
  <text x="700" y="228" class="val" text-anchor="end" id="total_loc">—,———,———</text>

  <text x="314" y="250" class="key">added   </text>
  <text x="380" y="250" class="dot-l" id="loc_add_dots">...................</text>
  <text x="700" y="250" class="val" text-anchor="end" id="loc_add">+—,———,———</text>

  <text x="314" y="272" class="key">deleted </text>
  <text x="380" y="272" class="dot-l" id="loc_del_dots">...................</text>
  <text x="700" y="272" class="val" text-anchor="end" id="loc_del">-—,———,———</text>

  <!-- Separator -->
  <line x1="314" y1="288" x2="796" y2="288" class="border2"/>

  <!-- Skills section -->
  <text x="314" y="312" class="label">ls skills/  —la</text>

  <!-- Skill tags -->
  <!-- Row 1 -->
  <rect x="314" y="322" width="64"  height="20" rx="1" fill="#0e140e" stroke="#2a5c2a" stroke-width="1"/>
  <text x="346" y="336" text-anchor="middle" class="mid" style="font-size:11px">python</text>

  <rect x="386" y="322" width="80"  height="20" rx="1" fill="#0e140e" stroke="#2a5c2a" stroke-width="1"/>
  <text x="426" y="336" text-anchor="middle" class="mid" style="font-size:11px">javascript</text>

  <rect x="474" y="322" width="82"  height="20" rx="1" fill="#0e140e" stroke="#2a5c2a" stroke-width="1"/>
  <text x="515" y="336" text-anchor="middle" class="mid" style="font-size:11px">typescript</text>

  <rect x="564" y="322" width="44"  height="20" rx="1" fill="#0e140e" stroke="#2a5c2a" stroke-width="1"/>
  <text x="586" y="336" text-anchor="middle" class="mid" style="font-size:11px">bash</text>

  <rect x="616" y="322" width="34"  height="20" rx="1" fill="#0e140e" stroke="#2a5c2a" stroke-width="1"/>
  <text x="633" y="336" text-anchor="middle" class="mid" style="font-size:11px">sql</text>

  <rect x="658" y="322" width="44"  height="20" rx="1" fill="#0e140e" stroke="#2a5c2a" stroke-width="1"/>
  <text x="680" y="336" text-anchor="middle" class="mid" style="font-size:11px">go</text>

  <!-- Row 2 -->
  <rect x="314" y="350" width="62"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="345" y="364" text-anchor="middle" class="dim" style="font-size:11px">fastapi</text>

  <rect x="384" y="350" width="58"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="413" y="364" text-anchor="middle" class="dim" style="font-size:11px">node.js</text>

  <rect x="450" y="350" width="56"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="478" y="364" text-anchor="middle" class="dim" style="font-size:11px">express</text>

  <rect x="514" y="350" width="54"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="541" y="364" text-anchor="middle" class="dim" style="font-size:11px">django</text>

  <rect x="576" y="350" width="74"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="613" y="364" text-anchor="middle" class="dim" style="font-size:11px">postgresql</text>

  <rect x="658" y="350" width="44"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="680" y="364" text-anchor="middle" class="dim" style="font-size:11px">redis</text>

  <!-- Row 3 -->
  <rect x="314" y="378" width="58"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="343" y="392" text-anchor="middle" class="dim" style="font-size:11px">docker</text>

  <rect x="380" y="378" width="52"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="406" y="392" text-anchor="middle" class="dim" style="font-size:11px">nginx</text>

  <rect x="440" y="378" width="52"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="466" y="392" text-anchor="middle" class="dim" style="font-size:11px">linux</text>

  <rect x="500" y="378" width="66"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="533" y="392" text-anchor="middle" class="dim" style="font-size:11px">mongodb</text>

  <rect x="574" y="378" width="54"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="601" y="392" text-anchor="middle" class="dim" style="font-size:11px">github</text>

  <rect x="636" y="378" width="46"  height="20" rx="1" fill="#0e140e" stroke="#1a3a1a" stroke-width="1"/>
  <text x="659" y="392" text-anchor="middle" class="dim" style="font-size:11px">grpc</text>

  <!-- Separator -->
  <line x1="314" y1="408" x2="796" y2="408" class="border2"/>

  <!-- Footer -->
  <text x="314" y="430" class="label">contributors: znaxh  ·  updated daily via github actions</text>
  <text x="796" y="430" text-anchor="end" class="label" id="contrib_data">—repos contributed</text>

</svg>
