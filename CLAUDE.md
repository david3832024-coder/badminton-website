# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **badminton enthusiast website** (羽毛球爱好者网站) - a static, single-page application built with vanilla HTML, CSS, and JavaScript. The site provides professional badminton knowledge including basic rules, skill tutorials, and equipment recommendations.

## Architecture

### File Structure
```
├── index.html      - Main HTML structure with semantic sections
├── styles.css      - All styling using CSS Grid/Flexbox with CSS variables
├── script.js       - Vanilla JavaScript for navigation, scroll effects, and animations
└── README.md       - Project documentation
```

### Design System
- **CSS Variables** (defined in `:root`): `--primary-color` (red #e74c3c), `--secondary-color` (blue #3498db), `--dark-color`, `--light-color`
- **Responsive Breakpoints**: 768px (tablet), 480px (mobile)
- **Layout**: CSS Grid for card layouts, Flexbox for navigation and alignment
- **Animations**: `fadeInUp` keyframe animation, smooth scroll behavior, Intersection Observer API for scroll-triggered animations

### JavaScript Functionality
- **Navigation**: Smooth scrolling between sections with `scrollTo()`
- **Active Link Highlighting**: Tracks scroll position and updates nav links
- **Mobile Menu**: Hamburger menu toggle for screens ≤ 768px
- **Scroll Animations**: Cards fade in using Intersection Observer (threshold: 0.1)

## Content Sections

1. **Home/Hero** - Landing section with gradient background
2. **Rules (基础知识)** - 3 cards: Game Rules, Scoring, Serving Rules
3. **Skills (技巧教学)** - 6 skill items: Forehand, Backhand, Footwork, Serving, Receiving, Net Play
4. **Equipment (装备推荐)** - 4 cards: Rackets, Shuttlecocks, Shoes, Apparel
5. **About** - Site description and features

## Common Development Commands

### Running the Site
```bash
# Option 1: Direct browser (double-click index.html)
# Option 2: Python HTTP server
python -m http.server 8000
# Then visit http://localhost:8000

# Option 3: Any local server (Node, PHP, etc.)
```

### Testing
- Open `index.html` in browser (Chrome, Firefox, Safari, Edge supported)
- Test responsive design by resizing browser window or using DevTools
- Verify scroll animations, navigation, and mobile menu functionality

### Development Notes
- No build process required - this is a static website
- No package manager or dependencies
- All code is vanilla HTML/CSS/JS with no frameworks
- CSS uses modern features (Grid, Flexbox, CSS variables, animations)

## Key Customization Points

1. **Colors**: Modify CSS variables in `styles.css:7-14` to change theme
2. **Content**: Edit sections in `index.html` (lines 39-166)
3. **Animations**: Adjust Intersection Observer settings in `script.js:55-75`
4. **Navigation**: Modify nav menu items in `index.html:16-22`

## README.md Content

The README provides instructions in Chinese. Key points:
- Direct usage: double-click `index.html` to open in browser
- Server usage: `python -m http.server 8000`
- Technology stack: HTML5, CSS3 (Grid/Flexbox/animations), Vanilla JavaScript
- Browser support: Chrome, Firefox, Safari, Edge
- Features: Smooth scroll nav, responsive menu, scroll animations, hover effects
- Customization: Colors in CSS variables, content in HTML, styles in CSS, interactions in JS
