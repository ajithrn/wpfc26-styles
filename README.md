# WPFC26 Styles

CSS and Sass files for the **WP Future Conclave 2026** website.

## Setup

```bash
npm install
```

## Usage

### Development (watch mode)

```bash
npm run watch
```

### Build for production

```bash
npm run build
```

The compiled CSS is output to `dist/style.css`.

## Remote CSS (Production)

The production site loads the compiled CSS from:

```
https://raw.githubusercontent.com/ajithrn/wpfc26-styles/main/dist/style.css
```

Configure this URL in the **Remote CSS** plugin or Additional CSS on the production WordPress site.

## Structure

```
src/
├── main.scss            Entry point
├── common/
│   ├── _variables.scss  Design tokens (colors, fonts, spacing)
│   └── _mixins.scss     Reusable mixins (responsive, buttons, cards)
├── base/
│   ├── _reset.scss      Minimal resets / TT4 overrides
│   └── _typography.scss Headings, body text, gradient text
├── components/
│   ├── _buttons.scss    Button styles
│   ├── _cards.scss      Card components
│   ├── _blocks.scss     WordPress block overrides
│   └── _forms.scss      Form styling
├── layout/
│   ├── _header.scss     Site header & navigation
│   ├── _footer.scss     Site footer
│   ├── _hero.scss       Hero section
│   └── _grid.scss       Grid utilities & section spacing
└── pages/
    ├── _home.scss       Home page specifics
    ├── _news.scss       News archive & home news grid
    ├── _tickets.scss    CampTix / ticket styling
    ├── _schedule.scss   Schedule page
    ├── _speakers.scss   Speakers page
    ├── _sponsors.scss   Sponsors page
    └── _faq.scss        FAQ page
```

## Theme

Base theme: **Twenty Twenty-Four** (WordPress block theme)

## License

MIT
