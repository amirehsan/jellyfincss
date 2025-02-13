# JellyfinCSS

A modern dark theme for Jellyfin Media Server with lime green accents and Persian/Arabic font support.

![Version](https://img.shields.io/badge/version-1.0.0-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)

## Features

- 🎨 Modern dark theme with lime green accents
- 🖌️ Refined UI elements and improved visual hierarchy
- 🔤 Built-in Persian/Arabic font support (IRAN font family)
- 📱 Responsive design for all screen sizes
- 🌙 Enhanced dark mode for better viewing experience
- ⚡ Lightweight CSS with minimal performance impact

## Preview

![Home Screen](screenshots/homepage.png)
![Movie Details](screenshots/details.png)
![TV Shows](screenshots/shows.png)


## Quick Start

### Basic Theme Installation

1. Go to Jellyfin dashboard: `Site > Dashboard > General > Custom CSS`
2. Add the following line:
```css
@import url("https://cdn.jsdelivr.net/gh/amirehsan/jellyfincss@main/jellyfin-styles.css");
```

### With Persian/Arabic Support

1. Go to Jellyfin dashboard: `Site > Dashboard > General > Custom CSS`
2. Add both lines:
```css
@import url("https://cdn.jsdelivr.net/gh/amirehsan/jellyfincss@main/jellyfin-styles.css");
html, body { font-family: 'IRAN', sans-serif !important; }
```

## Customization

### Color Scheme

All colors are defined as CSS variables at the top of the stylesheet. To modify any color in the theme, you only need to change it in one place. For example, to change the tab hover color (currently #00a4dc), find this section at the top of the CSS:

```css
:root {
    --color-primary: #ccff00;
    /* other color variables */
}
```

### Logo Customization

To change the Jellyfin logo, add one of these options to `Site > Dashboard > General > Custom CSS`:

#### Option 1: Load External Image
```css
.pageTitleWithDefaultLogo, .loginLogo {
    background-image: url("path_to_your_logo");
}
```

#### Option 2: Use Base64 Encoded Image
```css
.pageTitleWithDefaultLogo, .loginLogo {
    background-image: url(data:image/png;base64,/* Your base64 image data */);
}
```

## Font Details

The theme includes the following Persian/Arabic font variants:
- IRAN (Normal) - For regular text
- IRAN Black - For extra bold headlines
- IRAN Bold - For emphasized text
- IRAN SemiBold - For medium emphasis

## Browser Compatibility

Tested and working on:
- Google Chrome
- Mozilla Firefox
- Microsoft Edge
- Safari

## Known Issues

Currently no known issues. If you find any, please report them in the Issues section.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## Support

If you encounter any problems or have suggestions:
1. Check the [Issues](../../issues) page for known problems
2. Create a new issue if your problem is not yet reported

## License

MIT Licens

This CSS theme is free to use, modify, and distribute. You can:
- Use it in personal and commercial projects
- Modify it to suit your needs
- Share it with others

No attribution required, though it's appreciated!
