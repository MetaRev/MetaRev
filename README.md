##<svg viewBox="0 0 900 300" xmlns="http://www.w3.org/2000/svg" style="width:100%;height:auto;background:#0b0b12;position:relative;">
  <defs>
    <!-- Shifting dusk background: lavender -> navy -->
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#2a1f4d">
        <animate attributeName="offset" values="0;1;0" dur="10s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="#0b0b12">
        <animate attributeName="offset" values="1;0;1" dur="10s" repeatCount="indefinite" />
      </stop>
    </linearGradient>

    <!-- Soft pastel text sweep: mint -> pink -->
    <linearGradient id="textGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#a7fff5">
        <animate attributeName="offset" values="0;1;0" dur="7s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="#ffb3ec">
        <animate attributeName="offset" values="1;0;1" dur="7s" repeatCount="indefinite" />
      </stop>
    </linearGradient>

    <!-- Fine pastel grid (very subtle so it feels elegant, not hacker) -->
    <pattern id="grid" width="50" height="50" patternUnits="userSpaceOnUse">
      <path d="M50 0 L0 0 0 50" fill="none" stroke="#ffffff18" stroke-width="1"/>
    </pattern>

    <!-- Wave gradient: cotton candy teal -> peach -->
    <linearGradient id="waveGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#a7fff5"/>
      <stop offset="50%" stop-color="#ffd6e9"/>
      <stop offset="100%" stop-color="#ffebb0"/>
    </linearGradient>
  </defs>

  <!-- Background -->
  <rect width="100%" height="100%" fill="url(#bgGrad)" />

  <!-- Animated grid -->
  <rect width="100%" height="100%" fill="url(#grid)">
    <animateTransform attributeName="transform" type="translate" from="0 0" to="50 50" dur="12s" repeatCount="indefinite"/>
  </rect>

  <!-- Background wave -->
  <path fill="url(#waveGrad)" opacity="0.20">
    <animate attributeName="d" dur="22s" repeatCount="indefinite"
      values="
        M0,230 Q200,200 400,230 T900,230 V300 H0 Z;
        M0,220 Q200,250 400,220 T900,220 V300 H0 Z;
        M0,230 Q200,200 400,230 T900,230 V300 H0 Z"/>
  </path>

  <!-- Foreground wave -->
  <path fill="url(#waveGrad)" opacity="0.4">
    <animate attributeName="d" dur="14s" repeatCount="indefinite"
      values="
        M0,240 Q180,260 360,240 T900,240 V300 H0 Z;
        M0,230 Q180,210 360,230 T900,230 V300 H0 Z;
        M0,240 Q180,260 360,240 T900,240 V300 H0 Z"/>
  </path>

  <!-- Title -->
  <text x="50%" y="50%" text-anchor="middle"
        font-family="Segoe UI, system-ui, sans-serif"
        font-size="64" font-weight="700"
        fill="url(#textGradient)">
    MetaRev ⚡
  </text>

  <!-- Subtitle (more approachable / creator-y) -->
  <text x="50%" y="70%" text-anchor="middle"
        font-family="Segoe UI, system-ui, sans-serif"
        font-size="20" fill="#ffffffcc">
    clean code • clean ui • chaotic energy
  </text>

  <!-- Floaters -->
  <circle cx="18%" cy="22%" r="3" fill="#ffb3ec">
    <animate attributeName="cy" values="22%;27%;22%" dur="6s" repeatCount="indefinite"/>
  </circle>
  <circle cx="77%" cy="32%" r="2" fill="#a7fff5">
    <animate attributeName="cy" values="32%;37%;32%" dur="5s" repeatCount="indefinite"/>
  </circle>
</svg>


<!--
**MetaRev/MetaRev** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
