```svg
<svg width="1200" height="420" viewBox="0 0 1200 420"
     xmlns="http://www.w3.org/2000/svg">

  <defs>

    <!-- Background -->
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#020617"/>
      <stop offset="55%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#061A2E"/>
    </linearGradient>

    <!-- Glass -->
    <linearGradient id="glass" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#FFFFFF" stop-opacity=".10"/>
      <stop offset="100%" stop-color="#FFFFFF" stop-opacity=".025"/>
    </linearGradient>

    <!-- Blue glow -->
    <radialGradient id="glowBlue">
      <stop offset="0%" stop-color="#38BDF8" stop-opacity=".45"/>
      <stop offset="100%" stop-color="#38BDF8" stop-opacity="0"/>
    </radialGradient>

    <!-- Cyan glow -->
    <radialGradient id="glowCyan">
      <stop offset="0%" stop-color="#06B6D4" stop-opacity=".35"/>
      <stop offset="100%" stop-color="#06B6D4" stop-opacity="0"/>
    </radialGradient>

    <!-- Grid -->
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M40 0H0V40"
            fill="none"
            stroke="#38BDF8"
            stroke-opacity=".055"/>
    </pattern>

    <!-- Blur -->
    <filter id="blur">
      <feGaussianBlur stdDeviation="35"/>
    </filter>

    <filter id="smallBlur">
      <feGaussianBlur stdDeviation="8"/>
    </filter>

    <!-- Glass shadow -->
    <filter id="shadow">
      <feDropShadow dx="0" dy="18" stdDeviation="25"
                    flood-color="#000000"
                    flood-opacity=".35"/>
    </filter>

    <!-- Clip -->
    <clipPath id="rounded">
      <rect x="20" y="20" width="1160" height="380" rx="28"/>
    </clipPath>

  </defs>


  <!-- ================================= -->
  <!-- BACKGROUND -->
  <!-- ================================= -->

  <rect width="1200" height="420"
        fill="#020617"/>

  <rect x="20" y="20"
        width="1160"
        height="380"
        rx="28"
        fill="url(#bg)"/>

  <g clip-path="url(#rounded)">

    <!-- Grid -->
    <rect x="20" y="20"
          width="1160"
          height="380"
          fill="url(#grid)"/>

    <!-- Ambient glows -->
    <circle cx="1050" cy="80"
            r="230"
            fill="url(#glowBlue)"
            filter="url(#blur)">
      <animate attributeName="cx"
               values="1050;980;1050"
               dur="9s"
               repeatCount="indefinite"/>
    </circle>

    <circle cx="120" cy="360"
            r="200"
            fill="url(#glowCyan)"
            filter="url(#blur)">
      <animate attributeName="cy"
               values="360;320;360"
               dur="11s"
               repeatCount="indefinite"/>
    </circle>


    <!-- ================================= -->
    <!-- GLASS PANELS -->
    <!-- ================================= -->

    <rect x="60" y="60"
          width="1080"
          height="300"
          rx="24"
          fill="url(#glass)"
          stroke="#FFFFFF"
          stroke-opacity=".10"/>

    <rect x="80" y="80"
          width="620"
          height="260"
          rx="20"
          fill="#020617"
          fill-opacity=".20"
          stroke="#38BDF8"
          stroke-opacity=".08"/>


    <!-- ================================= -->
    <!-- ARCHITECTURE NETWORK -->
    <!-- ================================= -->

    <g stroke="#38BDF8"
       stroke-opacity=".22"
       fill="none">

      <path d="M780 110 L900 165 L1040 120"/>
      <path d="M900 165 L1010 240 L1100 195"/>
      <path d="M780 110 L820 270 L1010 240"/>
      <path d="M820 270 L930 315 L1100 195"/>

    </g>


    <!-- Nodes -->

    <g fill="#38BDF8">

      <circle cx="780" cy="110" r="4">
        <animate attributeName="r"
                 values="3;6;3"
                 dur="2.2s"
                 repeatCount="indefinite"/>
      </circle>

      <circle cx="900" cy="165" r="5">
        <animate attributeName="r"
                 values="4;8;4"
                 dur="2.7s"
                 repeatCount="indefinite"/>
      </circle>

      <circle cx="1040" cy="120" r="4">
        <animate attributeName="r"
                 values="3;7;3"
                 dur="2.4s"
                 repeatCount="indefinite"/>
      </circle>

      <circle cx="1010" cy="240" r="5">
        <animate attributeName="r"
                 values="4;8;4"
                 dur="3s"
                 repeatCount="indefinite"/>
      </circle>

      <circle cx="820" cy="270" r="4">
        <animate attributeName="r"
                 values="3;7;3"
                 dur="2.5s"
                 repeatCount="indefinite"/>
      </circle>

      <circle cx="930" cy="315" r="4"/>

      <circle cx="1100" cy="195" r="5">
        <animate attributeName="r"
                 values="4;8;4"
                 dur="2.8s"
                 repeatCount="indefinite"/>
      </circle>

    </g>


    <!-- ================================= -->
    <!-- LEFT CONTENT -->
    <!-- ================================= -->

    <text x="110"
          y="125"
          font-family="Inter, Arial, sans-serif"
          font-size="14"
          letter-spacing="4"
          fill="#38BDF8">
      SOFTWARE / SYSTEMS
    </text>

    <text x="105"
          y="185"
          font-family="Inter, Arial, sans-serif"
          font-size="48"
          font-weight="700"
          letter-spacing="-2"
          fill="#F8FAFC">
      YOUSSEF ERRAMI
    </text>

    <rect x="110"
          y="205"
          width="70"
          height="3"
          rx="2"
          fill="#38BDF8">
      <animate attributeName="width"
               values="40;100;70"
               dur="3s"
               repeatCount="indefinite"/>
    </rect>

    <text x="110"
          y="245"
          font-family="Inter, Arial, sans-serif"
          font-size="19"
          font-weight="600"
          fill="#CBD5E1">
      ERP ARCHITECT
    </text>

    <text x="110"
          y="275"
          font-family="Inter, Arial, sans-serif"
          font-size="17"
          fill="#94A3B8">
      Software Engineer · Full-Stack · Robotics
    </text>

    <text x="110"
          y="315"
          font-family="JetBrains Mono, monospace"
          font-size="13"
          fill="#64748B">
      Enterprise Systems → Automation → Intelligent Machines
    </text>


    <!-- ================================= -->
    <!-- TECH LABELS -->
    <!-- ================================= -->

    <g font-family="JetBrains Mono, monospace"
       font-size="11"
       fill="#64748B">

      <text x="760" y="365">ERP</text>
      <text x="820" y="365">AI</text>
      <text x="865" y="365">IoT</text>
      <text x="915" y="365">API</text>
      <text x="970" y="365">SQL</text>
      <text x="1025" y="365">C++</text>
      <text x="1080" y="365">DOCKER</text>

    </g>

  </g>


  <!-- Border -->

  <rect x="20" y="20"
        width="1160"
        height="380"
        rx="28"
        fill="none"
        stroke="#38BDF8"
        stroke-opacity=".15"/>

</svg>
```
