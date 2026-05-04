<div align="center">

<!--RETRO NIGHT SKY ANIMATION-->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/placeholder/placeholder/main/night-sky-dark.svg">
  <img src="https://raw.githubusercontent.com/placeholder/placeholder/main/night-sky-light.svg" alt="night sky" />
</picture>

<!-- Inline SVG fallback for GitHub README rendering -->
<svg width="860" height="160" viewBox="0 0 860 160" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <radialGradient id="sky" cx="50%" cy="50%" r="60%">
      <stop offset="0%" stop-color="#0d1b2a"/>
      <stop offset="100%" stop-color="#020810"/>
    </radialGradient>
    <!-- Moon glow -->
    <radialGradient id="moonGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#fffde7" stop-opacity="0.9"/>
      <stop offset="60%" stop-color="#fff9c4" stop-opacity="0.4"/>
      <stop offset="100%" stop-color="#fff9c4" stop-opacity="0"/>
    </radialGradient>
    <!-- Engine glow -->
    <radialGradient id="engineGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#ff6f00" stop-opacity="1"/>
      <stop offset="100%" stop-color="#ff6f00" stop-opacity="0"/>
    </radialGradient>
    <style>
      /* Stars twinkling */
      .star { animation: twinkle 2s infinite alternate; fill: #ffffff; }
      .star:nth-child(2n) { animation-delay: 0.5s; animation-duration: 1.5s; }
      .star:nth-child(3n) { animation-delay: 1s; animation-duration: 2.5s; }
      .star:nth-child(5n) { animation-delay: 0.3s; animation-duration: 1.8s; }
      @keyframes twinkle {
        from { opacity: 0.2; }
        to   { opacity: 1; }
      }

      /* Aircraft flying across */
      .aircraft-group {
        animation: fly 9s linear infinite;
      }
      @keyframes fly {
        0%   { transform: translateX(-120px); }
        100% { transform: translateX(980px); }
      }

      /* Engine flame flicker */
      .flame {
        animation: flicker 0.18s steps(2) infinite;
        transform-origin: right center;
      }
      @keyframes flicker {
        0%   { transform: scaleX(1)   scaleY(1); opacity: 1; }
        50%  { transform: scaleX(0.8) scaleY(1.2); opacity: 0.8; }
        100% { transform: scaleX(1.1) scaleY(0.9); opacity: 0.95; }
      }

      /* Contrail / exhaust trail */
      .trail {
        animation: trail 9s linear infinite;
        opacity: 0.55;
      }
      @keyframes trail {
        0%   { stroke-dashoffset: 0; opacity: 0; }
        5%   { opacity: 0.55; }
        95%  { opacity: 0.55; }
        100% { stroke-dashoffset: -200; opacity: 0; }
      }

      /* Pixel text scanline shimmer */
      .pixel-label {
        font-family: 'Courier New', Courier, monospace;
        font-size: 11px;
        fill: #00e5ff;
        letter-spacing: 2px;
        animation: scanShimmer 3s ease-in-out infinite alternate;
      }
      @keyframes scanShimmer {
        from { opacity: 0.6; }
        to   { opacity: 1; }
      }

      /* Radar sweep (decorative) */
      .radar-sweep {
        transform-origin: 810px 128px;
        animation: sweep 4s linear infinite;
        opacity: 0.35;
      }
      @keyframes sweep {
        from { transform: rotate(0deg); }
        to   { transform: rotate(360deg); }
      }

      /* Blink dot */
      .blink {
        animation: blink 1.1s steps(1) infinite;
      }
      @keyframes blink {
        0%, 100% { opacity: 1; }
        50%       { opacity: 0; }
      }
    </style>
  </defs>

  <!-- Night sky background -->
  <rect width="860" height="160" fill="url(#sky)" rx="10"/>

  <!-- Stars — hand-placed pixel-art style dots -->
  <circle class="star" cx="12"  cy="8"   r="1"/>
  <circle class="star" cx="45"  cy="22"  r="1.2"/>
  <circle class="star" cx="78"  cy="6"   r="0.8"/>
  <circle class="star" cx="120" cy="15"  r="1"/>
  <circle class="star" cx="155" cy="4"   r="1.3"/>
  <circle class="star" cx="200" cy="19"  r="0.9"/>
  <circle class="star" cx="230" cy="9"   r="1"/>
  <circle class="star" cx="275" cy="26"  r="0.8"/>
  <circle class="star" cx="310" cy="5"   r="1.2"/>
  <circle class="star" cx="350" cy="14"  r="1"/>
  <circle class="star" cx="390" cy="3"   r="0.9"/>
  <circle class="star" cx="420" cy="22"  r="1.1"/>
  <circle class="star" cx="460" cy="10"  r="1"/>
  <circle class="star" cx="495" cy="18"  r="0.8"/>
  <circle class="star" cx="530" cy="6"   r="1.2"/>
  <circle class="star" cx="565" cy="28"  r="1"/>
  <circle class="star" cx="600" cy="11"  r="0.9"/>
  <circle class="star" cx="640" cy="4"   r="1.1"/>
  <circle class="star" cx="680" cy="20"  r="1"/>
  <circle class="star" cx="710" cy="8"   r="0.8"/>
  <circle class="star" cx="750" cy="14"  r="1.2"/>
  <circle class="star" cx="790" cy="5"   r="1"/>
  <circle class="star" cx="830" cy="17"  r="0.9"/>
  <circle class="star" cx="855" cy="25"  r="1.1"/>

  <!-- Second row stars -->
  <circle class="star" cx="30"  cy="42"  r="0.8"/>
  <circle class="star" cx="70"  cy="38"  r="1"/>
  <circle class="star" cx="110" cy="50"  r="1.1"/>
  <circle class="star" cx="175" cy="40"  r="0.9"/>
  <circle class="star" cx="240" cy="48"  r="1"/>
  <circle class="star" cx="305" cy="36"  r="0.8"/>
  <circle class="star" cx="370" cy="52"  r="1.2"/>
  <circle class="star" cx="430" cy="38"  r="1"/>
  <circle class="star" cx="490" cy="44"  r="0.9"/>
  <circle class="star" cx="550" cy="35"  r="1.1"/>
  <circle class="star" cx="615" cy="48"  r="1"/>
  <circle class="star" cx="675" cy="41"  r="0.8"/>
  <circle class="star" cx="730" cy="52"  r="1.2"/>
  <circle class="star" cx="800" cy="37"  r="1"/>
  <circle class="star" cx="848" cy="44"  r="0.9"/>

  <!-- Moon -->
  <circle cx="790" cy="30" r="18" fill="url(#moonGlow)"/>
  <circle cx="790" cy="30" r="11" fill="#fffde7"/>
  <!-- Moon craters (pixel style) -->
  <circle cx="785" cy="26" r="2.5" fill="#f5f0b0" opacity="0.6"/>
  <circle cx="795" cy="34" r="1.8" fill="#f5f0b0" opacity="0.5"/>
  <circle cx="787" cy="33" r="1.2" fill="#f5f0b0" opacity="0.4"/>

  <!-- Horizon glow (city lights) -->
  <rect x="0" y="130" width="860" height="30" rx="0" fill="#061020"/>
  <!-- Pixel-art city silhouette -->
  <!-- Buildings as pixel blocks -->
  <rect x="0"   y="120" width="18" height="40" fill="#0a1f3a"/>
  <rect x="5"   y="112" width="8"  height="8"  fill="#0a1f3a"/>
  <rect x="20"  y="108" width="14" height="52" fill="#0b2040"/>
  <rect x="36"  y="118" width="10" height="42" fill="#081830"/>
  <rect x="48"  y="104" width="16" height="56" fill="#0c2244"/>
  <rect x="66"  y="115" width="12" height="45" fill="#091930"/>
  <rect x="80"  y="110" width="10" height="50" fill="#0a2038"/>
  <rect x="92"  y="122" width="14" height="38" fill="#0b1e36"/>
  <rect x="108" y="106" width="18" height="54" fill="#0d2448"/>
  <rect x="128" y="118" width="10" height="42" fill="#081a32"/>
  <rect x="140" y="100" width="14" height="60" fill="#0c2244"/>
  <rect x="156" y="114" width="16" height="46" fill="#091c38"/>
  <rect x="174" y="120" width="10" height="40" fill="#0a1e3a"/>
  <rect x="186" y="108" width="12" height="52" fill="#0b2040"/>
  <!-- Windows lit up -->
  <rect x="25"  y="114" width="3" height="2" fill="#ffd740" opacity="0.8"/>
  <rect x="30"  y="114" width="3" height="2" fill="#ffd740" opacity="0.7"/>
  <rect x="25"  y="119" width="3" height="2" fill="#ffd740" opacity="0.6"/>
  <rect x="52"  y="110" width="3" height="2" fill="#ffd740" opacity="0.7"/>
  <rect x="58"  y="110" width="3" height="2" fill="#ffd740" opacity="0.8"/>
  <rect x="52"  y="116" width="3" height="2" fill="#00e5ff" opacity="0.6"/>
  <rect x="113" y="112" width="3" height="2" fill="#ffd740" opacity="0.7"/>
  <rect x="119" y="112" width="3" height="2" fill="#ffd740" opacity="0.6"/>
  <rect x="113" y="118" width="3" height="2" fill="#ffd740" opacity="0.8"/>
  <rect x="144" y="106" width="3" height="2" fill="#00e5ff" opacity="0.7"/>
  <rect x="150" y="106" width="3" height="2" fill="#ffd740" opacity="0.6"/>
  <rect x="144" y="112" width="3" height="2" fill="#ffd740" opacity="0.8"/>

  <!-- City on right side -->
  <rect x="590" y="112" width="16" height="48" fill="#0a1f3a"/>
  <rect x="608" y="105" width="12" height="55" fill="#0b2244"/>
  <rect x="622" y="118" width="10" height="42" fill="#091c38"/>
  <rect x="634" y="108" width="18" height="52" fill="#0c2040"/>
  <rect x="654" y="115" width="10" height="45" fill="#081a32"/>
  <rect x="666" y="100" width="14" height="60" fill="#0d2448"/>
  <rect x="682" y="114" width="12" height="46" fill="#091e3a"/>
  <rect x="696" y="120" width="16" height="40" fill="#0a2038"/>
  <rect x="714" y="106" width="10" height="54" fill="#0b2244"/>
  <rect x="726" y="118" width="14" height="42" fill="#081c36"/>
  <rect x="742" y="104" width="16" height="56" fill="#0c2040"/>
  <rect x="760" y="112" width="10" height="48" fill="#091a32"/>
  <rect x="772" y="120" width="12" height="40" fill="#0a1e3a"/>
  <!-- Windows right side -->
  <rect x="595" y="118" width="3" height="2" fill="#ffd740" opacity="0.7"/>
  <rect x="612" y="111" width="3" height="2" fill="#ffd740" opacity="0.8"/>
  <rect x="618" y="111" width="3" height="2" fill="#00e5ff" opacity="0.6"/>
  <rect x="638" y="114" width="3" height="2" fill="#ffd740" opacity="0.7"/>
  <rect x="644" y="114" width="3" height="2" fill="#ffd740" opacity="0.6"/>
  <rect x="670" y="106" width="3" height="2" fill="#00e5ff" opacity="0.8"/>
  <rect x="676" y="106" width="3" height="2" fill="#ffd740" opacity="0.7"/>
  <rect x="700" y="116" width="3" height="2" fill="#ffd740" opacity="0.6"/>
  <rect x="746" y="110" width="3" height="2" fill="#ffd740" opacity="0.8"/>
  <rect x="752" y="110" width="3" height="2" fill="#00e5ff" opacity="0.7"/>

  <!-- Radar dish (bottom right) -->
  <g transform="translate(808,128)">
    <!-- Dish base -->
    <rect x="-3" y="0" width="6" height="18" fill="#1a3a5c"/>
    <rect x="-8" y="18" width="16" height="4" fill="#1a3a5c"/>
    <!-- Dish bowl (pixel arcs) -->
    <path d="M-14,-2 Q0,-22 14,-2" fill="none" stroke="#00bcd4" stroke-width="1.5" opacity="0.8"/>
    <path d="M-10,-2 Q0,-16 10,-2" fill="none" stroke="#00bcd4" stroke-width="1" opacity="0.6"/>
    <!-- Sweep line -->
    <line class="radar-sweep" x1="0" y1="0" x2="14" y2="-14" stroke="#00e5ff" stroke-width="1.2" opacity="0.5"/>
    <!-- Center dot -->
    <circle cx="0" cy="0" r="2" fill="#00e5ff" opacity="0.9"/>
    <!-- Radar blips -->
    <circle class="blink" cx="-28" cy="-35" r="2" fill="#00ff88" opacity="0.9"/>
    <circle class="blink" cx="22" cy="-20" r="1.5" fill="#00ff88" opacity="0.8" style="animation-delay:0.5s"/>
  </g>

  <!-- ===== FLYING AIRCRAFT ===== -->
  <g class="aircraft-group">

    <!-- Exhaust trail behind aircraft -->
    <line class="trail" x1="-5" y1="76" x2="-110" y2="78"
          stroke="#ff6f00" stroke-width="2"
          stroke-dasharray="4 3"
          stroke-linecap="round"/>
    <line class="trail" x1="-5" y1="78" x2="-90" y2="82"
          stroke="#ff8f00" stroke-width="1"
          stroke-dasharray="3 5"
          stroke-linecap="round"
          style="animation-delay:0.1s"/>

    <!-- Engine flame -->
    <g class="flame">
      <ellipse cx="-8" cy="76" rx="12" ry="4" fill="#ff6f00" opacity="0.9"/>
      <ellipse cx="-14" cy="76" rx="8" ry="2.5" fill="#ffab40" opacity="0.8"/>
      <ellipse cx="-18" cy="76" rx="5" ry="1.5" fill="#fffde7" opacity="0.7"/>
    </g>

    <!-- ── Pixel-art aircraft body (side view, flying right) ── -->
    <!-- Fuselage (main body) -->
    <rect x="0"  y="70" width="56" height="12" rx="2" fill="#b0bec5"/>
    <!-- Nose cone -->
    <polygon points="56,70 56,82 72,76" fill="#cfd8dc"/>
    <!-- Cockpit window -->
    <rect x="48" y="72" width="12" height="6" rx="1" fill="#00bcd4" opacity="0.9"/>
    <!-- Cockpit frame -->
    <rect x="47" y="71" width="14" height="8" rx="1" fill="none" stroke="#546e7a" stroke-width="0.8"/>

    <!-- Main wings (swept back) -->
    <polygon points="20,76  44,76  36,104  10,104" fill="#90a4ae"/>
    <polygon points="20,76  44,76  36,50   10,50"  fill="#90a4ae"/>
    <!-- Wing detail stripes -->
    <line x1="14" y1="76" x2="22" y2="100" stroke="#607d8b" stroke-width="0.8" opacity="0.6"/>
    <line x1="14" y1="76" x2="22" y2="54"  stroke="#607d8b" stroke-width="0.8" opacity="0.6"/>

    <!-- Tail fin (vertical) -->
    <polygon points="4,70 4,58 18,70" fill="#78909c"/>
    <!-- Horizontal stabilizers -->
    <polygon points="4,76 4,82 20,76 20,76" fill="none"/>
    <polygon points="8,76 8,82 24,82 18,76" fill="#78909c" opacity="0.85"/>
    <polygon points="8,70 8,64 24,64 18,70" fill="#78909c" opacity="0.85"/>

    <!-- Engine nacelle (below fuselage) -->
    <rect x="16" y="82" width="22" height="7" rx="2" fill="#546e7a"/>
    <ellipse cx="16" cy="85" rx="4" ry="3.5" fill="#37474f"/>
    <!-- Intake grill lines -->
    <line x1="16" y1="83" x2="16" y2="89" stroke="#263238" stroke-width="0.6"/>
    <line x1="18" y1="83" x2="18" y2="89" stroke="#263238" stroke-width="0.6"/>
    <line x1="20" y1="83" x2="20" y2="89" stroke="#263238" stroke-width="0.6"/>

    <!-- Navigation lights -->
    <!-- Red (port) -->
    <circle class="blink" cx="10" cy="104" r="2.5" fill="#f44336" style="animation-delay:0s"/>
    <!-- Green (starboard) -->
    <circle class="blink" cx="10" cy="50"  r="2.5" fill="#66bb6a" style="animation-delay:0.55s"/>
    <!-- White (tail) -->
    <circle class="blink" cx="2"  cy="76"  r="2" fill="#fffde7" style="animation-delay:0.28s"/>

    <!-- Pixel decorations on fuselage -->
    <rect x="30" y="73" width="4" height="2" fill="#546e7a" opacity="0.7"/>
    <rect x="36" y="73" width="4" height="2" fill="#546e7a" opacity="0.7"/>
    <!-- Fuselage windows -->
    <rect x="24" y="73" width="5" height="4" rx="1" fill="#e0f7fa" opacity="0.8"/>
    <rect x="31" y="73" width="5" height="4" rx="1" fill="#e0f7fa" opacity="0.8"/>
    <rect x="38" y="73" width="5" height="4" rx="1" fill="#e0f7fa" opacity="0.8"/>

    <!-- Pixel scanline label below aircraft -->
    <text x="10" y="115" class="pixel-label" font-size="9" fill="#00e5ff" opacity="0.7" letter-spacing="1">FLIGHT 001</text>
  </g>

  <!-- HUD overlay elements -->
  <!-- Top-left altitude readout -->
  <text x="14" y="60" font-family="'Courier New', monospace" font-size="9" fill="#00e5ff" opacity="0.55" letter-spacing="1">ALT:35000ft</text>
  <text x="14" y="72" font-family="'Courier New', monospace" font-size="9" fill="#00ff88" opacity="0.45" letter-spacing="1">SPD:550kts</text>

  <!-- Bottom scanline -->
  <rect x="0" y="155" width="860" height="5" fill="#00e5ff" opacity="0.04" rx="0"/>
</svg>

</div>

---

<h1 align="center">Hi there 👋, I'm Naoufal Saadi</h1>
<p align="center">
  🚀 I build with Data &amp; AI &nbsp;|&nbsp; 🛠️ Turning ideas into systems
</p>

---

### 🔍 About Me

- ⚡ Building data-driven tools and AI systems  
- 🧠 Exploring models, frameworks, and workflows  
- 🌍 Always curious, always shipping  

---

### 🧰 Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/C-%2300599C.svg?&style=for-the-badge&logo=c&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-%2314354C.svg?&style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-%23007ACC.svg?&style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Java-%23ED8B00.svg?&style=for-the-badge&logo=java&logoColor=white" />
  <img src="https://img.shields.io/badge/Scala-%23DC322F.svg?&style=for-the-badge&logo=scala&logoColor=white" />
</p>
<p align="center">
  <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?&style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?&style=for-the-badge&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/MLflow-%23000000.svg?&style=for-the-badge&logo=mlflow&logoColor=white" />
  <img src="https://img.shields.io/badge/GCP-%234285F4.svg?&style=for-the-badge&logo=google-cloud&logoColor=white" />
</p>
<p align="center">
  <img src="https://img.shields.io/badge/PostgreSQL-%23336791.svg?&style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/MongoDB-%2347A248.svg?&style=for-the-badge&logo=mongodb&logoColor=white" />
</p>

---

### 📫 Connect with Me

- 📧 Email: [naoufal894@gmail.com](mailto:naoufal894@gmail.com)  
- 💼 LinkedIn: [linkedin.com/in/naoufal-saadi](https://linkedin.com/in/naoufal-saadi)
> *“Read deeply. Code clearly. Learn endlessly.”*

