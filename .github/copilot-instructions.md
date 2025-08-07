# Saynomoncher GitHub Pages Website
Saynomoncher.github.io is a static HTML website with retro 70s minimalist design hosted on GitHub Pages. The site features a single-page design with inline CSS styling, no build process required, and automatic deployment from the main branch.

Always reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.

## Working Effectively
- Clone and setup the repository:
  - `git clone https://github.com/saynomoncher/saynomoncher.github.io.git`
  - `cd saynomoncher.github.io`
- Serve the site locally for development:
  - `python3 -m http.server 8000 --bind 127.0.0.1` -- starts immediately (< 1 second). NEVER CANCEL.
  - Access at: http://127.0.0.1:8000
  - Stop with Ctrl+C or `kill` command
- Alternative local server options:
  - `php -S 127.0.0.1:8000` (if PHP available)
  - `npx serve .` (if Node.js available)
  - Any static file server will work

## Repository Structure
- `index.html` -- Main page with retro 70s design and inline styles
- `README.md` -- Basic repository description
- `.git/` -- Git repository data
- No build files, no dependencies, no configuration files

## Validation
- ALWAYS manually validate any changes by serving the site locally and testing in a browser.
- ALWAYS test the complete user experience after making changes:
  1. Start local server: `python3 -m http.server 8000 --bind 127.0.0.1`
  2. Open http://127.0.0.1:8000 in browser
  3. Verify page loads with retro styling (pale golden background, chocolate brown "RETRO VIBES" heading)
  4. Test button hover effects work properly
  5. Click "Explore More" button to ensure it responds to user interaction
  6. Verify copyright footer is visible at bottom
  7. Test responsive behavior by resizing browser window
- Basic HTML validation:
  - `python3 -c "import html.parser; parser = html.parser.HTMLParser(); parser.feed(open('index.html').read()); print('HTML validation: PASSED')"`
- No linting tools required - this is pure HTML/CSS with no JavaScript framework
- No CI/CD workflows exist - GitHub Pages deploys automatically from main branch

## Common Tasks

### Editing the Site
- Edit `index.html` directly - all styles are inline CSS
- No compilation or build process required
- Changes are immediately visible when refreshing browser after saving

### Testing Changes
- Always serve locally first: `python3 -m http.server 8000 --bind 127.0.0.1`
- Test all interactive elements (button hover effects, responsive design)
- Verify color scheme matches retro 70s theme:
  - Background: #ffefd5 (pale golden)
  - Heading: #d2691e (chocolate brown) 
  - Button: #8b4513 (saddle brown)
  - Text: #2c2c2c (deep gray)

### Deployment
- GitHub Pages automatically deploys from main branch
- No manual deployment steps required
- Changes appear live within 1-2 minutes after pushing to main
- Site URL: https://saynomoncher.github.io

## File Reference

### Repository Root Contents
```
.
├── .git/              # Git repository data
├── README.md          # Basic repository description (3 lines)
└── index.html         # Main webpage (1761 bytes, single file application)
```

### index.html Structure
- DOCTYPE html5 declaration
- Complete CSS styles in `<head>` section (retro 70s color scheme)
- Centered layout with flexbox
- Single h1 "RETRO VIBES" heading
- Descriptive paragraph
- Interactive "Explore More" button (no JavaScript functionality)
- Copyright footer

### README.md Content
```
# saynomoncher.github.io
Do mein
```

## Timing Expectations
- Local server startup: < 1 second
- File operations: < 0.01 seconds  
- Page load in browser: < 0.5 seconds
- No build process - changes are immediate
- GitHub Pages deployment: 1-2 minutes after push to main

## Important Notes
- This is a GitHub Pages repository - the .github.io suffix indicates automatic hosting
- No package.json, no dependencies, no build tools required
- All styling is inline CSS within the HTML file
- Button has hover effects but no click functionality (no JavaScript)
- Site is fully responsive using CSS flexbox and viewport meta tag
- No frameworks, libraries, or external dependencies
- Content is static - no server-side processing or database