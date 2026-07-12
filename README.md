<div align="center">

<svg width="100%" height="400" viewBox="0 0 800 400" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Neon glow filter -->
    <filter id="neonGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur in="SourceGraphic" stdDeviation="3" result="blur"/>
      <feColorMatrix in="blur" type="matrix" values="0 0 0 0 0  0 0 0 0 1  0 0 0 0 0.96  0 0 0 1 0" result="cyanBlur"/>
      <feGaussianBlur in="SourceGraphic" stdDeviation="6" result="blur2"/>
      <feColorMatrix in="blur2" type="matrix" values="0 0 0 0 1  0 0 0 0 0  0 0 0 0 1  0 0 0 0.6 0" result="magentaBlur"/>
      <feMerge>
        <feMergeNode in="magentaBlur"/>
        <feMergeNode in="cyanBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    
    <!-- Glitch displacement filter -->
    <filter id="glitchFilter">
      <feTurbulence type="fractalNoise" baseFrequency="0.01 0.001" numOctaves="1" seed="1" result="noise">
        <animate attributeName="baseFrequency" values="0.01 0.001;0.05 0.001;0.01 0.001;0.08 0.002;0.01 0.001" dur="4s" repeatCount="indefinite"/>
      </feTurbulence>
      <feDisplacementMap in="SourceGraphic" in2="noise" scale="0" xChannelSelector="R" yChannelSelector="G">
        <animate attributeName="scale" values="0;0;0;15;0;0;0;8;0;0;0;0" dur="4s" repeatCount="indefinite"/>
      </feDisplacementMap>
    </filter>

    <!-- Scanline pattern -->
    <pattern id="scanlines" patternUnits="userSpaceOnUse" width="800" height="4">
      <rect width="800" height="1" fill="#00fff5" opacity="0.08"/>
      <rect y="2" width="800" height="1" fill="#00fff5" opacity="0.04"/>
    </pattern>
  </defs>

  <!-- Background -->
  <rect width="800" height="400" fill="#0a0a0f"/>
  
  <!-- Animated scanlines -->
  <rect width="800" height="400" fill="url(#scanlines)">
    <animateTransform attributeName="transform" type="translate" values="0,0;0,-4" dur="0.5s" repeatCount="indefinite"/>
  </rect>

  <!-- Main name with glitch + neon glow -->
  <g filter="url(#glitchFilter)">
    <text x="400" y="160" text-anchor="middle" font-family="'Courier New', monospace" font-size="56" font-weight="bold" fill="#00fff5" stroke="#ff00ff" stroke-width="1" filter="url(#neonGlow)">
      Nattapat Ritter
      <animate attributeName="opacity" values="1;1;1;1;0.3;1;1;1;1;1;1;1;0.5;1;1" dur="3s" repeatCount="indefinite"/>
    </text>
  </g>

  <!-- Alias -->
  <text x="400" y="200" text-anchor="middle" font-family="'Courier New', monospace" font-size="20" fill="#ff00ff" opacity="0.9">
    also known as Backpack
    <animate attributeName="opacity" values="0.9;0.9;0.9;0.4;0.9;0.9;0.9;0.9;0.6;0.9" dur="4s" repeatCount="indefinite"/>
  </text>

  <!-- Subtitle -->
  <text x="400" y="240" text-anchor="middle" font-family="'Courier New', monospace" font-size="18" fill="#00fff5" opacity="0.8">
    Developer · Tech Explorer · Music Producer
  </text>

  <!-- Decorative lines -->
  <line x1="100" y1="280" x2="700" y2="280" stroke="#ff00ff" stroke-width="1" opacity="0.3">
    <animate attributeName="opacity" values="0.3;0.6;0.3" dur="2s" repeatCount="indefinite"/>
  </line>
  <line x1="200" y1="290" x2="600" y2="290" stroke="#00fff5" stroke-width="1" opacity="0.2">
    <animate attributeName="opacity" values="0.2;0.5;0.2" dur="2.5s" repeatCount="indefinite"/>
  </line>
</svg>

<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&width=730&center=true&vCenter=true&multiline=true&duration=3000&pause=1000&repeat=true&width=730&lines=%22The+right+to+education+is+the+foundation+of+a+free+society.%22&center=true&vCenter=true&color=%2300fff5&bgColor=%230a0a0f)](https://git.io/typing-svg)

<br/>

<a href="https://github.com/nritter26/acadamic">
  <img src="https://img.shields.io/badge/-📦_Start_Learning-00fff5?style=for-the-badge&logo=github&logoColor=0a0a0f&labelColor=0d1117" alt="Start Learning"/>
</a>

<br/>

</div>

---

## 🧠 About Me

<div style="background-color: #0d1117; border: 1px solid #ff00ff; border-top: 3px solid #00fff5; border-radius: 8px; padding: 20px; margin: 20px 0;">

<div style="display: flex; align-items: center; gap: 8px; margin-bottom: 12px;">
  <span style="width: 12px; height: 12px; border-radius: 50%; background-color: #ff5f56; display: inline-block;"></span>
  <span style="width: 12px; height: 12px; border-radius: 50%; background-color: #ffbd2e; display: inline-block;"></span>
  <span style="width: 12px; height: 12px; border-radius: 50%; background-color: #27c93f; display: inline-block;"></span>
  <span style="color: #00fff5; font-family: 'Courier New', monospace; font-size: 14px; margin-left: 12px;">nattapat@backpack:~$</span>
</div>

```ts
const nattapat = {
  location: "Bangkok, Thailand",
  style: ["Cyberpunk", "Dark", "Minimal"],
  interests: [
    "Interactive AI Tutors",
    "UX Design",
    "Automation",
    "TypeScript",
    "Creative Coding",
    "Whatever that makes knowledge free to everyone"
  ],
  currentlyBuilding: "Futuristic tech site for free learning experiences"
};
```

</div>

---

## ⚒️ Tech Stack

<svg width="100%" height="50" viewBox="0 0 600 50" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <filter id="headerGlitch">
      <feTurbulence type="fractalNoise" baseFrequency="0.02 0.001" numOctaves="1" seed="2" result="noise">
        <animate attributeName="baseFrequency" values="0.02 0.001;0.08 0.002;0.02 0.001;0.1 0.001;0.02 0.001" dur="5s" repeatCount="indefinite"/>
      </feTurbulence>
      <feDisplacementMap in="SourceGraphic" in2="noise" scale="0" xChannelSelector="R" yChannelSelector="G">
        <animate attributeName="scale" values="0;0;0;12;0;0;0;6;0;0" dur="5s" repeatCount="indefinite"/>
      </feDisplacementMap>
    </filter>
    <filter id="headerGlow">
      <feGaussianBlur in="SourceGraphic" stdDeviation="2" result="blur"/>
      <feColorMatrix in="blur" type="matrix" values="0 0 0 0 0  0 0 0 0 1  0 0 0 0 0.96  0 0 0 1 0" result="cyanBlur"/>
      <feMerge>
        <feMergeNode in="cyanBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  <text x="300" y="35" text-anchor="middle" font-family="'Courier New', monospace" font-size="28" font-weight="bold" fill="#00fff5" filter="url(#headerGlow)" filter="url(#headerGlitch)">
    ⚒️ Tech Stack
    <animate attributeName="opacity" values="1;1;1;0.4;1;1;1;1;0.6;1" dur="4s" repeatCount="indefinite"/>
  </text>
</svg>

### Languages

<div align="center">

![TypeScript](https://img.shields.io/badge/TypeScript-00fff5?style=flat-square&logo=typescript&logoColor=0a0a0f&labelColor=0d1117)
![JavaScript](https://img.shields.io/badge/JavaScript-f7df1e?style=flat-square&logo=javascript&logoColor=0a0a0f&labelColor=0d1117)
![Python](https://img.shields.io/badge/Python-3776ab?style=flat-square&logo=python&logoColor=white&labelColor=0d1117)
![Bash](https://img.shields.io/badge/Bash-4eaa25?style=flat-square&logo=gnubash&logoColor=white&labelColor=0d1117)

</div>

### Tools & Frameworks

<div align="center">

![React](https://img.shields.io/badge/React-61dafb?style=flat-square&logo=react&logoColor=0a0a0f&labelColor=0d1117)
![Svelte](https://img.shields.io/badge/Svelte-ff3e00?style=flat-square&logo=svelte&logoColor=white&labelColor=0d1117)
![Vue](https://img.shields.io/badge/Vue-4fc08d?style=flat-square&logo=vuedotjs&logoColor=white&labelColor=0d1117)
![Tauri](https://img.shields.io/badge/Tauri-24c8db?style=flat-square&logo=tauri&logoColor=white&labelColor=0d1117)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white&labelColor=0d1117)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white&labelColor=0d1117)
![Vite](https://img.shields.io/badge/Vite-646cff?style=flat-square&logo=vite&logoColor=white&labelColor=0d1117)
![Docker](https://img.shields.io/badge/Docker-2496ed?style=flat-square&logo=docker&logoColor=white&labelColor=0d1117)
![Playwright](https://img.shields.io/badge/Playwright-2ead33?style=flat-square&logo=playwright&logoColor=white&labelColor=0d1117)

</div>

### Databases & Cloud

<div align="center">

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169e1?style=flat-square&logo=postgresql&logoColor=white&labelColor=0d1117)
![MySQL](https://img.shields.io/badge/MySQL-4479a1?style=flat-square&logo=mysql&logoColor=white&labelColor=0d1117)
![MongoDB](https://img.shields.io/badge/MongoDB-47a248?style=flat-square&logo=mongodb&logoColor=white&labelColor=0d1117)
![AWS](https://img.shields.io/badge/AWS-ff00ff?style=flat-square&logo=amazonwebservices&logoColor=white&labelColor=0d1117)

</div>

<!-- Animated neon divider -->
<svg width="100%" height="20" viewBox="0 0 800 20" xmlns="http://www.w3.org/2000/svg">
  <line x1="0" y1="10" x2="800" y2="10" stroke="#00fff5" stroke-width="1" opacity="0.4"/>
  <circle r="4" fill="#00fff5" cy="10" opacity="0.9">
    <animate attributeName="cx" values="0;800" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.9;0.3;0.9" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle r="6" fill="#ff00ff" cy="10" opacity="0.3">
    <animate attributeName="cx" values="0;800" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0.8;0.3" dur="3s" repeatCount="indefinite"/>
  </circle>
</svg>

---

## 🌌 Current Focus

<svg width="100%" height="50" viewBox="0 0 600 50" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <filter id="focusGlow">
      <feGaussianBlur in="SourceGraphic" stdDeviation="2" result="blur"/>
      <feColorMatrix in="blur" type="matrix" values="0 0 0 0 1  0 0 0 0 0  0 0 0 0 1  0 0 0 1 0" result="magentaBlur"/>
      <feMerge>
        <feMergeNode in="magentaBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  <text x="300" y="35" text-anchor="middle" font-family="'Courier New', monospace" font-size="28" font-weight="bold" fill="#ff00ff" filter="url(#focusGlow)">
    🌌 Current Focus
    <animate attributeName="opacity" values="1;1;0.5;1;1;1;0.3;1;1;1" dur="4s" repeatCount="indefinite"/>
  </text>
</svg>

<table align="center" style="margin: 20px auto; border-collapse: separate; border-spacing: 16px;">
  <tr>
    <td align="center" style="background-color: #0d1117; border: 1px solid #00fff5; border-radius: 12px; padding: 20px 24px; width: 200px;">
      <svg width="60" height="60" viewBox="0 0 60 60" xmlns="http://www.w3.org/2000/svg">
        <rect x="2" y="2" width="56" height="56" rx="8" fill="none" stroke="#00fff5" stroke-width="1.5" opacity="0.8">
          <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="2s" repeatCount="indefinite"/>
        </rect>
        <text x="30" y="38" text-anchor="middle" font-size="28">🤖</text>
      </svg>
      <br/>
      <span style="color: #00fff5; font-family: 'Courier New', monospace; font-size: 14px; font-weight: bold;">AI-Powered Tools</span>
      <br/>
      <span style="color: #e0e0e0; font-size: 12px;">Building AI-powered tools</span>
    </td>
    <td align="center" style="background-color: #0d1117; border: 1px solid #ff00ff; border-radius: 12px; padding: 20px 24px; width: 200px;">
      <svg width="60" height="60" viewBox="0 0 60 60" xmlns="http://www.w3.org/2000/svg">
        <rect x="2" y="2" width="56" height="56" rx="8" fill="none" stroke="#ff00ff" stroke-width="1.5" opacity="0.8">
          <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="2.3s" repeatCount="indefinite"/>
        </rect>
        <text x="30" y="38" text-anchor="middle" font-size="28">📚</text>
      </svg>
      <br/>
      <span style="color: #ff00ff; font-family: 'Courier New', monospace; font-size: 14px; font-weight: bold;">Learning App</span>
      <br/>
      <span style="color: #e0e0e0; font-size: 12px;">Designing a learning app</span>
    </td>
    <td align="center" style="background-color: #0d1117; border: 1px solid #bf00ff; border-radius: 12px; padding: 20px 24px; width: 200px;">
      <svg width="60" height="60" viewBox="0 0 60 60" xmlns="http://www.w3.org/2000/svg">
        <rect x="2" y="2" width="56" height="56" rx="8" fill="none" stroke="#bf00ff" stroke-width="1.5" opacity="0.8">
          <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="1.8s" repeatCount="indefinite"/>
        </rect>
        <text x="30" y="38" text-anchor="middle" font-size="28">🎨</text>
      </svg>
      <br/>
      <span style="color: #bf00ff; font-family: 'Courier New', monospace; font-size: 14px; font-weight: bold;">UX Concepts</span>
      <br/>
      <span style="color: #e0e0e0; font-size: 12px;">Creating futuristic UX concepts</span>
    </td>
  </tr>
</table>

<br/>

<!-- System Status Bar -->
<div align="center">

<svg width="100%" height="50" viewBox="0 0 800 50" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <pattern id="statusScanlines" patternUnits="userSpaceOnUse" width="800" height="4">
      <rect width="800" height="1" fill="#00fff5" opacity="0.05"/>
    </pattern>
  </defs>
  
  <!-- Background -->
  <rect width="800" height="50" rx="6" fill="#0d1117" stroke="#00fff5" stroke-width="1" opacity="0.8"/>
  
  <!-- Scanlines -->
  <rect width="800" height="50" rx="6" fill="url(#statusScanlines)">
    <animateTransform attributeName="transform" type="translate" values="0,0;0,-4" dur="0.3s" repeatCount="indefinite"/>
  </rect>
  
  <!-- Left: Status -->
  <circle cx="30" cy="25" r="5" fill="#00ff41">
    <animate attributeName="opacity" values="1;0.3;1" dur="1.5s" repeatCount="indefinite"/>
  </circle>
  <text x="45" y="29" font-family="'Courier New', monospace" font-size="14" fill="#00ff41">SYSTEM: ONLINE</text>
  
  <!-- Center: OS Name -->
  <text x="400" y="29" text-anchor="middle" font-family="'Courier New', monospace" font-size="14" fill="#00fff5" opacity="0.8">
    BACKPACK_OS v2.0
    <animate attributeName="opacity" values="0.8;1;0.8" dur="2s" repeatCount="indefinite"/>
  </text>
  
  <!-- Right: Mood -->
  <text x="620" y="29" font-family="'Courier New', monospace" font-size="14" fill="#ff00ff">
    MOOD: CODING
  </text>
  <rect x="748" y="20" width="8" height="16" fill="#ff00ff" opacity="0.8">
    <animate attributeName="opacity" values="0.8;0;0.8" dur="1s" repeatCount="indefinite"/>
  </rect>
</svg>

</div>

<br/>

## 📊 Skill Matrix

<svg width="100%" height="220" viewBox="0 0 700 220" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="barGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00fff5"/>
      <stop offset="100%" style="stop-color:#ff00ff"/>
    </linearGradient>
    <filter id="barGlow">
      <feGaussianBlur in="SourceGraphic" stdDeviation="2" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  
  <!-- TypeScript -->
  <text x="130" y="30" text-anchor="end" font-family="'Courier New', monospace" font-size="14" fill="#e0e0e0">TypeScript</text>
  <rect x="140" y="18" width="420" height="20" rx="4" fill="#1a1a2e"/>
  <rect x="140" y="18" width="0" height="20" rx="4" fill="url(#barGradient)" filter="url(#barGlow)">
    <animate attributeName="width" from="0" to="420" dur="1.5s" fill="freeze"/>
  </rect>
  <text x="570" y="33" font-family="'Courier New', monospace" font-size="14" fill="#00fff5">95%</text>
  
  <!-- React/Svelte -->
  <text x="130" y="70" text-anchor="end" font-family="'Courier New', monospace" font-size="14" fill="#e0e0e0">React / Svelte</text>
  <rect x="140" y="58" width="420" height="20" rx="4" fill="#1a1a2e"/>
  <rect x="140" y="58" width="0" height="20" rx="4" fill="url(#barGradient)" filter="url(#barGlow)">
    <animate attributeName="width" from="0" to="396" dur="1.5s" fill="freeze" begin="0.2s"/>
  </rect>
  <text x="546" y="73" font-family="'Courier New', monospace" font-size="14" fill="#00fff5">90%</text>
  
  <!-- Node.js -->
  <text x="130" y="110" text-anchor="end" font-family="'Courier New', monospace" font-size="14" fill="#e0e0e0">Node.js</text>
  <rect x="140" y="98" width="420" height="20" rx="4" fill="#1a1a2e"/>
  <rect x="140" y="98" width="0" height="20" rx="4" fill="url(#barGradient)" filter="url(#barGlow)">
    <animate attributeName="width" from="0" to="378" dur="1.5s" fill="freeze" begin="0.4s"/>
  </rect>
  <text x="528" y="113" font-family="'Courier New', monospace" font-size="14" fill="#00fff5">85%</text>
  
  <!-- Python -->
  <text x="130" y="150" text-anchor="end" font-family="'Courier New', monospace" font-size="14" fill="#e0e0e0">Python</text>
  <rect x="140" y="138" width="420" height="20" rx="4" fill="#1a1a2e"/>
  <rect x="140" y="138" width="0" height="20" rx="4" fill="url(#barGradient)" filter="url(#barGlow)">
    <animate attributeName="width" from="0" to="336" dur="1.5s" fill="freeze" begin="0.6s"/>
  </rect>
  <text x="486" y="153" font-family="'Courier New', monospace" font-size="14" fill="#00fff5">80%</text>
  
  <!-- DevOps -->
  <text x="130" y="190" text-anchor="end" font-family="'Courier New', monospace" font-size="14" fill="#e0e0e0">DevOps</text>
  <rect x="140" y="178" width="420" height="20" rx="4" fill="#1a1a2e"/>
  <rect x="140" y="178" width="0" height="20" rx="4" fill="url(#barGradient)" filter="url(#barGlow)">
    <animate attributeName="width" from="0" to="315" dur="1.5s" fill="freeze" begin="0.8s"/>
  </rect>
  <text x="465" y="193" font-family="'Courier New', monospace" font-size="14" fill="#00fff5">75%</text>
</svg>

<br/>

<!-- Animated neon divider -->
<svg width="100%" height="20" viewBox="0 0 800 20" xmlns="http://www.w3.org/2000/svg">
  <line x1="0" y1="10" x2="800" y2="10" stroke="#ff00ff" stroke-width="1" opacity="0.4"/>
  <circle r="4" fill="#ff00ff" cy="10" opacity="0.9">
    <animate attributeName="cx" values="800;0" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.9;0.3;0.9" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle r="6" fill="#00fff5" cy="10" opacity="0.3">
    <animate attributeName="cx" values="800;0" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0.8;0.3" dur="3s" repeatCount="indefinite"/>
  </circle>
</svg>

<br/>

<!-- Animated quote -->
<div align="center">

<svg width="100%" height="80" viewBox="0 0 800 80" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <filter id="quoteGlow">
      <feGaussianBlur in="SourceGraphic" stdDeviation="2" result="blur"/>
      <feColorMatrix in="blur" type="matrix" values="0 0 0 0 1  0 0 0 0 0  0 0 0 0 1  0 0 0 0.8 0" result="magentaBlur"/>
      <feMerge>
        <feMergeNode in="magentaBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  
  <text x="400" y="35" text-anchor="middle" font-family="'Courier New', monospace" font-size="16" font-style="italic" fill="#ff00ff" filter="url(#quoteGlow)">
    "The right to education is the foundation
    <animate attributeName="opacity" values="1;1;1;0.4;1;1;1;1;0.6;1" dur="5s" repeatCount="indefinite"/>
  </text>
  <text x="400" y="60" text-anchor="middle" font-family="'Courier New', monospace" font-size="16" font-style="italic" fill="#ff00ff" filter="url(#quoteGlow)">
    of a free society."
    <animate attributeName="opacity" values="1;1;1;1;0.3;1;1;1;1;1;0.5;1" dur="5s" repeatCount="indefinite"/>
  </text>
</svg>

<br/>

<!-- Social Links -->
<a href="https://github.com/nritter26">
  <img src="https://img.shields.io/badge/GitHub-00fff5?style=flat-square&logo=github&logoColor=0a0a0f&labelColor=0d1117" alt="GitHub"/>
</a>
<a href="https://linkedin.com/in/nritter26">
  <img src="https://img.shields.io/badge/LinkedIn-0a66c2?style=flat-square&logo=linkedin&logoColor=white&labelColor=0d1117" alt="LinkedIn"/>
</a>

<br/>
<br/>

<span style="color: #4a9e9e; font-family: 'Courier New', monospace; font-size: 12px;">
  ⚡ Built with neon dreams and dark code ⚡
</span>

<br/>
<br/>

</div>
