# Assignment 3 - Responsive Web Design

Mereikhan Sholanbayev, IT-2511

A one-page responsive website about the Apollo Moon landings (Space Notes).
Open `index.html` in a browser. No installation or build step is needed, but
the page needs internet access to load Bootstrap 5.3 from the CDN.

## Files

- `index.html`: the page (navbar, intro, Apollo 11, six landings, spacecraft cards, footer).
- `css/style.css`: my own styles, linked after the Bootstrap CSS.
- `images/`: two NASA photographs.

## Task 1 - media queries by hand

The "The six landings" section (`#landings`) uses only my own CSS (CSS Grid), mobile-first:

- base styles (phone): 1 item per row, heading 1.5rem and left-aligned;
- `@media (min-width: 768px)`: 2 items per row, heading 2rem and centred, bigger gap;
- `@media (min-width: 1024px)`: 3 items per row, more padding around the section.

## Task 2 - Bootstrap grid and components

- Navbar with `navbar-expand-md`: below 768px the links collapse into the menu button.
- Intro: `col-12 col-md-7` and `col-md-5`; the photo is hidden on a phone (`d-none d-md-block`).
- Apollo 11: the photo comes first in the HTML, but `order-*` puts the text first on a phone.
- Spacecraft cards: `col-12 col-md-6 col-lg-4` gives 1, 2 and 3 cards per row.
- Footer: the "Back to top" button is shown only on a phone (`d-md-none`).

## Checks

- No horizontal scroll at any width from 320px to 1920px.
- HTML and CSS pass the W3C validators with no errors or warnings.

## Sources and credits

- Facts: https://www.nasa.gov/specials/apollo50th/missions.html
- Apollo 11: https://www.nasa.gov/missions/apollo/apollo-11/apollo-11-mission-overview/
- Photos: https://www.nasa.gov/wp-content/uploads/static/history/ap11ann/kippsphotos/apollo.html
  - `launch.jpg`: Apollo 11 launch, NASA S69-39526.
  - `aldrin.jpg`: Buzz Aldrin on the Moon, NASA / Neil Armstrong, AS11-40-5903.

NASA is credited as the source; no NASA endorsement is implied.
