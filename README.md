# Netflix Landing Page Clone (Practice Project)

A responsive recreation of a streaming-service landing page, built with plain **HTML and CSS** (no JavaScript, no frameworks). It includes a hero section with a sign-up form, feature sections with an animated TV video, an FAQ list and a multi-column footer.

> **Disclaimer:** This is a non-commercial learning project. It is not affiliated with, endorsed by or connected to Netflix, Inc. "Netflix" and its logo are trademarks of Netflix, Inc. Don't deploy this publicly as if it were the real service or use it to collect real user data.

---

## Preview

| Section | What it shows |
|---|---|
| Hero | Full-width background image with a dark overlay, logo, language and Sign In buttons, headline text and an email sign-up field |
| Feature sections | Alternating text and image blocks (TV, offline downloads, watch everywhere, kids profiles) |
| FAQ | Four expandable-style question boxes with a hover effect |
| Footer | Four columns of links that become two columns on smaller screens |

## Tech Stack

- **HTML5**: semantic structure (`nav`, `section`, `footer`)
- **CSS3**: Flexbox, CSS Grid, absolute and relative positioning, media queries, transitions
- **Google Fonts**: Poppins and Martel Sans

## Project Structure

```
Video 53/
├── index.html
├── style.css
├── favicon.ico
└── assets/
    ├── images/
    │   ├── bg.jpg        # hero background
    │   └── logo.svg      # navbar logo
    └── videos/
        └── video1.m4v    # local sample video
```

## Getting Started

1. **Download or clone** this repository.
2. Open the `Video 53` folder.
3. Double-click `index.html` to open it in your browser.

No build step or installation is needed.

**Optional:** to run it on a local server, use the VS Code *Live Server* extension, or run this from inside the project folder:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

> **Internet connection needed:** the fonts, the feature-section images and the TV videos load from external URLs, so those parts won't appear when you're offline.

## Responsive Design

The layout adapts with a media query at **1300px**:

- The navbar widens to 90% of the viewport.
- Feature sections stack vertically (`flex-wrap`).
- Images and videos shrink from 555px to 305px wide.
- Headline sizes decrease (48px to 32px).
- The email field and button stack vertically.
- The footer grid changes from 4 columns to 2.

## Key CSS Concepts Practised

- Layering a dark overlay on a background image using `position: absolute` and `opacity`
- Placing a video inside a TV frame image with `position: absolute` and `z-index`
- Centering content with Flexbox and `margin: auto`
- Building a 4-column footer with CSS Grid
- Smooth hover transitions on the FAQ boxes
- Mobile-friendly layouts with `max-width: 60vw` and media queries

## Known Limitations

- The FAQ boxes only change colour on hover; they don't expand to show answers (this would need a little JavaScript).
- The email input and "Get Started" button have no functionality.
- Footer links point to placeholder `faq` addresses.
- The local `assets/videos/video1.m4v` file is included but not currently used in `index.html`.

## Ideas for Improvement

- [ ] Add JavaScript to expand and collapse the FAQ answers
- [ ] Validate the email field before submitting
- [ ] Add a language dropdown
- [ ] Add a browse page with movie rows
- [ ] Replace external images and videos with local assets so it works offline
- [ ] Replace the branding with your own original name and logo for a portfolio version

## Author

**Yuganter Veerwal**

Built while learning front-end web development with HTML and CSS.

## License

For educational use only. Brand names, logos and media belong to their respective owners.
