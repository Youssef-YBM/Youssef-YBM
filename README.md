```svg
<svg width="1280" height="440" viewBox="0 0 1280 440"
     xmlns="http://www.w3.org/2000/svg">

<defs>

  <!-- Background -->
  <linearGradient id="background"
                  x1="0" y1="0" x2="1" y2="1">
    <stop offset="0" stop-color="#030712"/>
    <stop offset=".45" stop-color="#0B1220"/>
    <stop offset="1" stop-color="#071A2D"/>
  </linearGradient>

  <!-- Blue atmospheric glow -->
  <radialGradient id="blueGlow">
    <stop offset="0" stop-color="#2563EB" stop-opacity=".38"/>
    <stop offset=".45" stop-color="#2563EB" stop-opacity=".12"/>
    <stop offset="1" stop-color="#2563EB" stop-opacity="0"/>
  </radialGradient>

  <!-- Cyan glow -->
  <radialGradient id="cyanGlow">
    <stop offset="0" stop-color="#06B6D4" stop-opacity=".28"/>
    <stop offset="1" stop-color="#06B6D4" stop-opacity="0"/>
  </radialGradient>

  <!-- Glass -->
  <linearGradient id="glass"
                  x1="0" y1="0" x2="1" y2="1">
    <stop offset="0" stop-color="#FFFFFF" stop-opacity=".09"/>
    <stop offset=".5" stop-color="#FFFFFF" stop-opacity=".035"/>
    <stop offset="1" stop-color="#FFFFFF" stop-opacity=".015"/>
  </linearGradient>

  <!-- Border -->
  <linearGradient id="border"
                  x1="0" y1="0" x2="1" y2="1">
    <stop offset="0" stop-color="#38BDF8" stop-opacity=".35"/>
    <stop offset=".5" stop-color="#FFFFFF" stop-opacity=".08"/>
    <stop offset="1" stop-color="#2563EB" stop-opacity=".28"/>
  </linearGradient>

  <!-- Grid -->
  <pattern id="grid"
           width="42"
           height="42"
           patternUnits="userSpaceOnUse">

    <path d="M42 0H0V42"
          fill="none"
          stroke="#38BDF8"
          stroke-opacity=".045"/>

  </pattern>

  <!-- Blur -->
  <filter id="blur">
    <feGaussianBlur stdDeviation="45"/>
  </filter>

  <filter id="softBlur">
    <feGaussianBlur stdDeviation="10"/>
  </filter>

  <!-- Shadow -->
  <filter id="shadow">

    <feDropShadow
      dx="0"
      dy="20"
      stdDeviation="25"
      flood-color="#000"
      flood-opacity=".45"/>

  </filter>

  <!-- Clip -->
  <clipPath id="clip">
    <rect x="18"
          y="18"
          width="1244"
          height="404"
          rx="30"/>
  </clipPath>

</defs>


<!-- ================================================= -->
<!-- BACKGROUND -->
<!-- ================================================= -->

<rect width="1280"
      height="440"
      rx="32"
      fill="#020617"/>

<rect x="18"
      y="18"
      width="1244"
      height="404"
      rx="30"
      fill="url(#background)"/>

<g clip-path="url(#clip)">

  <!-- Grid -->

  <rect width="1280"
        height="440"
        fill="url(#grid)"/>


  <!-- Ambient light -->

  <circle cx="1080"
          cy="80"
          r="300"
          fill="url(#blueGlow)"
          filter="url(#blur)">

    <animate attributeName="cx"
             values="1080;1000;1080"
             dur="12s"
             repeatCount="indefinite"/>

  </circle>


  <circle cx="180"
          cy="390"
          r="260"
          fill="url(#cyanGlow)"
          filter="url(#blur)">

    <animate attributeName="cy"
             values="390;350;390"
             dur="10s"
             repeatCount="indefinite"/>

  </circle>


  <!-- ================================================= -->
  <!-- MAIN GLASS CONTAINER -->
  <!-- ================================================= -->

  <rect x="52"
        y="52"
        width="1176"
        height="336"
        rx="26"
        fill="url(#glass)"
        stroke="url(#border)"
        stroke-width="1"/>


  <!-- ================================================= -->
  <!-- LEFT GLASS PANEL -->
  <!-- ================================================= -->

  <rect x="78"
        y="78"
        width="585"
        height="284"
        rx="20"
        fill="#020617"
        fill-opacity=".23"
        stroke="#FFFFFF"
        stroke-opacity=".055"/>


  <!-- Small status -->

  <circle cx="112"
          cy="112"
          r="4"
          fill="#22C55E">

    <animate attributeName="opacity"
             values=".35;1;.35"
             dur="2s"
             repeatCount="indefinite"/>

  </circle>

  <text x="126"
        y="117"
        font-family="JetBrains Mono,monospace"
        font-size="11"
        letter-spacing="2"
        fill="#64748B">

    SYSTEMS / SOFTWARE

  </text>


  <!-- NAME -->

  <text x="108"
        y="180"
        font-family="Inter,Arial,sans-serif"
        font-size="48"
        font-weight="750"
        letter-spacing="-2"
        fill="#F8FAFC">

    YOUSSEF ERRAMI

  </text>


  <!-- Accent line -->

  <rect x="110"
        y="198"
        width="90"
        height="3"
        rx="2"
        fill="#38BDF8">

    <animate attributeName="width"
             values="45;120;90"
             dur="3s"
             repeatCount="indefinite"/>

  </rect>


  <!-- ROLE -->

  <text x="108"
        y="242"
        font-family="Inter,Arial,sans-serif"
        font-size="21"
        font-weight="650"
        fill="#E2E8F0">

    ERP ARCHITECT

  </text>

  <text x="108"
        y="270"
        font-family="Inter,Arial,sans-serif"
        font-size="16"
        fill="#94A3B8">

    Software Engineer · Full-Stack · Robotics

  </text>


  <!-- Description -->

  <text x="108"
        y="310"
        font-family="JetBrains Mono,monospace"
        font-size="12"
        fill="#64748B">

    enterprise systems / automation / intelligent machines

  </text>


  <!-- ================================================= -->
  <!-- RIGHT ARCHITECTURE -->
  <!-- ================================================= -->

  <!-- connections -->

  <g fill="none"
     stroke="#38BDF8"
     stroke-opacity=".18"
     stroke-width="1.2">

    <path d="M760 135 L880 100 L1010 145 L1150 110"/>

    <path d="M760 135 L835 245 L990 225 L1150 110"/>

    <path d="M835 245 L920 315 L1090 285 L1150 110"/>

    <path d="M880 100 L920 315"/>

    <path d="M1010 145 L990 225"/>

  </g>


  <!-- animated data packet -->

  <circle r="3"
          fill="#67E8F9">

    <animateMotion
      dur="3.8s"
      repeatCount="indefinite"
      path="M760 135 L880 100 L1010 145 L1150 110"/>

  </circle>


  <circle r="3"
          fill="#60A5FA">

    <animateMotion
      dur="4.6s"
      repeatCount="indefinite"
      path="M760 135 L835 245 L990 225 L1150 110"/>

  </circle>


  <!-- nodes -->

  <g fill="#38BDF8">

    <circle cx="760" cy="135" r="4"/>

    <circle cx="880" cy="100" r="5">

      <animate attributeName="r"
               values="4;7;4"
               dur="2.5s"
               repeatCount="indefinite"/>

    </circle>

    <circle cx="1010" cy="145" r="4"/>

    <circle cx="1150" cy="110" r="6">

      <animate attributeName="r"
               values="5;9;5"
               dur="2.8s"
               repeatCount="indefinite"/>

    </circle>

    <circle cx="835" cy="245" r="4"/>

    <circle cx="990" cy="225" r="5"/>

    <circle cx="920" cy="315" r="4"/>

    <circle cx="1090" cy="285" r="4"/>

  </g>


  <!-- Node labels -->

  <g font-family="JetBrains Mono,monospace"
     font-size="10"
     fill="#64748B">

    <text x="742" y="125">API</text>

    <text x="866" y="88">ERP</text>

    <text x="995" y="132">SQL</text>

    <text x="1128" y="96">CLOUD</text>

    <text x="815" y="265">IOT</text>

    <text x="970" y="245">AI</text>

    <text x="900" y="335">ROBOT</text>

    <text x="1065" y="305">DOCKER</text>

  </g>


  <!-- ================================================= -->
  <!-- STACK STRIP -->
  <!-- ================================================= -->

  <rect x="705"
        y="345"
        width="485"
        height="30"
        rx="15"
        fill="#020617"
        fill-opacity=".45"
        stroke="#FFFFFF"
        stroke-opacity=".06"/>


  <g font-family="JetBrains Mono,monospace"
     font-size="10"
     fill="#64748B">

    <text x="730" y="365">NEXT</text>

    <text x="790" y="365">REACT</text>

    <text x="860" y="365">NEST</text>

    <text x="920" y="365">POSTGRES</text>

    <text x="1010" y="365">C++</text>

    <text x="1055" y="365">ESP32</text>

    <text x="1120" y="365">DOCKER</text>

  </g>

</g>


<!-- ================================================= -->
<!-- OUTER BORDER -->
<!-- ================================================= -->

<rect x="18"
      y="18"
      width="1244"
      height="404"
      rx="30"
      fill="none"
      stroke="#38BDF8"
      stroke-opacity=".12"/>

</svg>
```
