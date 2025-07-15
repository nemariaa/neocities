You can visit the site at [nemaria.neocities.org](https://nemaria.neocities.org/).

This site uses modified versions of [kingdra.net](https://kingdra.net/fan/)'s [fic masterlist template](https://kingdra.net/masterlist-template/) and [css styling for fics downloaded from AO3](https://kingdra.net/fan/ao3css/).
The main changes I've made are:
1. adding a dark mode button on both the masterlist and each individual fic
2. adding a link to the masterlist in each fic
3. modifying the padding in `style.css`, and padding and borders in `ao3-style.css` so that the text/borders aren't right up against the edge of the screen at some window widths

Please feel free to use/modify however you'd like.


***


If you do use this as a template for your own site, here's how to add the darkmode button and masterlist link to the top of a new fic. This presumes you have downloaded all the files from this repository and are using the same file structure.

1. Paste the following code into the html file downloaded from AO3, right underneath the opening ``<body>`` tag and before the ``<div id="preface">`` section.
  
```
    <header>
      <div id="masterlist-link">
        <a href="../index.html">🡐back to masterlist</a>
      </div>
      <button id="theme-switch">
        <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px"><path d="M480-120q-150 0-255-105T120-480q0-150 105-255t255-105q14 0 27.5 1t26.5 3q-41 29-65.5 75.5T444-660q0 90 63 153t153 63q55 0 101-24.5t75-65.5q2 13 3 26.5t1 27.5q0 150-105 255T480-120Z"/></svg>
        <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px"><path d="M480-280q-83 0-141.5-58.5T280-480q0-83 58.5-141.5T480-680q83 0 141.5 58.5T680-480q0 83-58.5 141.5T480-280ZM200-440H40v-80h160v80Zm720 0H760v-80h160v80ZM440-760v-160h80v160h-80Zm0 720v-160h80v160h-80ZM256-650l-101-97 57-59 96 100-52 56Zm492 496-97-101 53-55 101 97-57 59Zm-98-550 97-101 59 57-100 96-56-52ZM154-212l101-97 55 53-97 101-59-57Z"/></svg>
      </button>
    </header>
```

2. Paste the following code into the `<head>` section of the fic html file (I put it at the bottom right before the closing `</head>` tag).

    `<script type="text/javascript" src="../darkmode.js" defer></script>`
