# Leon’s personal website

A simple English-language personal homepage, hosted on GitHub Pages.

## Edit

- `index.html`: introduction, about section, journal index, Now section, and contact links.
- `assets/css/personal.css`: responsive layout, colors, and typography.
- `assets/images/leon-portrait.jpg`: homepage portrait, exported as JPEG without original photo metadata. CSS frames it as a square aligned to the bottom, preserving the full image file. The previous landscape photo is retained as `assets/images/leon-lake.jpg`.

The homepage uses plain HTML and CSS, with no build step or JavaScript dependencies.
The first journal entry is in `journal/a-more-personal-space.html`. New entries can use the same HTML structure and shared stylesheet; add a link and summary to the homepage. The first entry is drafted copy for review before publication.
Older template assets are retained but are no longer loaded by the homepage.

## Preview

Run from the repository root:

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

Open http://localhost:8765. Check both narrow and wide windows before publishing.

## Map

`assets/images/places-lived.svg` is a static SVG derived from us-atlas v3 (`states-albers-10m.json`), using its Albers USA projection. Solid green states indicate places lived in; striped ochre states indicate places visited. There are no route lines, numbers, or chronological ordering. The two HTML state lists provide a readable mobile and screen-reader equivalent. California, Pennsylvania, Virginia, and Washington are lived-in states; Arizona, Connecticut, Delaware, Florida, Georgia, Idaho, Illinois, Maine, Maryland, Massachusetts, Montana, Nevada, New Hampshire, New Jersey, New York, Ohio, Oregon, Utah, and Wyoming are visited states.

Source: https://github.com/topojson/us-atlas (ISC license; see `assets/images/us-atlas-LICENSE.txt`).

## World map and coffee chats

The Places section uses native radio controls to switch between U.S. and World views. Keyboard users can Tab to the control and use arrow keys to switch; no JavaScript is required. Reduced-motion preferences disable the transition.

`assets/images/world-travels.svg` is derived from world-atlas v2 `countries-110m.json` (https://github.com/topojson/world-atlas). It marks the United States in solid green as the current home, and highlights visited places in striped ochre: the United Kingdom, Japan, South Korea, United Arab Emirates, Kenya, Canada, China, Taiwan, and Mexico. Its dots help locate visited places, not specific cities. The map excludes Antarctica. See `assets/images/world-atlas-LICENSE.txt`.

The coffee-chat call to action links to the public Google Calendar booking page at https://calendar.app.google/TR19LBY3GGt2pSzY7. It offers 30-minute Saturday appointments from 2–5 p.m. America/Los_Angeles through December 17, 2026, excluding October 31. Google Meet links are generated automatically; a required booking question lets guests request an in-person meeting within about a 10-minute drive of Cannery Park, San Jose, with the venue confirmed separately. Calendar conflicts are checked. Update the site copy and schedule when this booking window ends. No private calendar or credentials are embedded.
