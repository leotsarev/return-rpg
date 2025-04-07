+++
title="Танчико"
weight=1100
+++
<svg width="982" height="1600" xmlns="http://www.w3.org/2000/svg">
    <style>
        .group text { visibility: hidden; }
        .group:hover text { visibility: visible; }
    </style>
  <!-- Фоновое изображение -->
  <image href="https://return-avatars.leotsarev.ru/maps/tanchico.png" x="0" y="0" width="982" height="1600" />

  <defs>
    <filter id="text-bg" x="-5" y="-5" width="200" height="50">
      <feFlood flood-color="black" flood-opacity="0.8"/>
      <feComposite in2="SourceGraphic" operator="in"/>
      <feMorphology in="SourceAlpha" result="DILATED" operator="dilate" radius="2"/>
      <feMerge>
        <feMergeNode/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- Пример вставки сторонней SVG-иконки (здесь — простая звезда) 
  <g transform="translate(494, 313)" class="group">
    <polygon points="10,0 12,7 20,7 13.5,11.5 16,18 10,14 4,18 6.5,11.5 0,7 8,7"
             fill="gold" />
    <text x="10" y="30" font-size="12" text-anchor="middle" fill="white" filter="url(#text-bg)">Лагерь белоплащников</text>
    
  </g> -->

  <g class="group" transform="translate(494, 313)">
    <polygon points="0,10 20,10 10,0" fill="brown" />
    <rect x="2" y="10" width="16" height="10" fill="saddlebrown" />
    <text x="10" y="30" font-size="16" text-anchor="middle" fill="white" filter="url(#text-bg)">Лагерь белоплащников</text>
  </g>

  <g class="group" transform="translate(132, 532)">
    <rect x="4" y="4" width="12" height="12" fill="black" />
    <polygon points="4,16 16,16 10,24" fill="black"/>
    <text x="10" y="30" font-size="16" text-anchor="middle" fill="white" filter="url(#text-bg)">Вход в каменоломни</text>
  </g>

  <g class="group" transform="translate(440, 947)">
    <rect x="3" y="6" width="14" height="12" fill="peru" />
    <circle cx="10" cy="12" r="3" fill="burlywood" />
    <text x="10" y="30" font-size="16" text-anchor="middle" fill="white" filter="url(#text-bg)">Таверна «Три сливы»</text>
  </g>

  <g class="group" transform="translate(232, 990)">
    <rect x="3" y="6" width="14" height="12" fill="peru" />
    <circle cx="10" cy="12" r="3" fill="burlywood" />
    <text x="10" y="30" font-size="16" text-anchor="middle" fill="white" filter="url(#text-bg)">Таверна «Затмение»</text>
  </g>

  <g class="group" transform="translate(266, 686)">
        <rect x="4" y="8" width="12" height="10" fill="goldenrod" />
    <polygon points="4,8 10,0 16,8" fill="gold" />
    <text x="10" y="30" font-size="16" text-anchor="middle" fill="white" filter="url(#text-bg)">Особняк марат`дамани</text>
  </g>

  <g class="group" transform="translate(122, 1198)">
    <polygon points="0,10 20,10 10,0" fill="brown" />
    <rect x="2" y="10" width="16" height="10" fill="saddlebrown" />
  </g>

  <g class="group" transform="translate(142, 1218)">
    <polygon points="0,10 20,10 10,0" fill="brown" />
    <rect x="2" y="10" width="16" height="10" fill="saddlebrown" />
    <text x="10" y="30" font-size="16" text-anchor="middle" fill="white" filter="url(#text-bg)">Основной лагерь Предвестников</text>
  </g>

  <g class="group" transform="translate(108, 1214)">
    <polygon points="0,10 20,10 10,0" fill="brown" />
    <rect x="2" y="10" width="16" height="10" fill="saddlebrown" />
    <text x="10" y="30" font-size="16" text-anchor="middle" fill="white" filter="url(#text-bg)">Основной лагерь Предвестников</text>
  </g>

  <g class="group" transform="translate(442, 700)">
        <rect x="4" y="8" width="12" height="10" fill="goldenrod" />
    <polygon points="4,8 10,0 16,8" fill="gold" />
    <text x="10" y="30" font-size="16" text-anchor="middle" fill="white" filter="url(#text-bg)">Дворец панарха</text>
  </g>

  <g class="group" transform="translate(412, 847)">
        <rect x="4" y="8" width="12" height="10" fill="goldenrod" />
    <polygon points="4,8 10,0 16,8" fill="gold" />
    <text x="10" y="30" font-size="16" text-anchor="middle" fill="white" filter="url(#text-bg)">Дворец короля</text>
  </g>

  <g class="group" transform="translate(342, 847)">
    <rect x="4" y="4" width="12" height="12" fill="black" />
    <line x1="4" y1="10" x2="16" y2="10" stroke="white" stroke-width="1" />
    <text x="10" y="30" font-size="16" text-anchor="middle" fill="white" filter="url(#text-bg)">Подвал с выходом</text>
  </g>
</svg>
