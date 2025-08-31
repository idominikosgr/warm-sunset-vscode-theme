# Warm Sunset VSCode Theme - Dedicated Landing Page

*A carefully crafted color theme that brings warmth and focus to your coding environment*

## Hero Section

**Main Tagline:** *"Code in comfort with colors that actually make sense"*

**Subheading:** Warm, accessible theme for developers who spend long hours in their editor

**Visual Preview:** Side-by-side screenshots of light and dark themes showing real code

### Key Features at a Glance
- **Dual themes:** Light and dark variants with consistent color relationships  
- **Eye comfort:** Warm color palette designed for extended coding sessions
- **Accessibility focused:** High contrast ratios, colorblind-friendly choices
- **Language support:** Thoughtful syntax highlighting for 20+ programming languages
- **Active development:** Part of the entro314 labs design system research

## The Story Behind Warm Sunset

### Why Another VSCode Theme?

Most coding themes fall into two camps: 
1. **Ultra-minimal** (boring gray on gray)
2. **RGB rainbow explosion** (your retinas need sunglasses)

We wanted something different - a theme that feels like coding during golden hour. Warm enough to feel inviting, but never distracting from your code.

### Design Philosophy

**Warm but Professional**
- Base colors inspired by sunset gradients and natural wood tones
- Orange accents (`#FA906E`) that draw attention without screaming
- Neutral backgrounds that don't compete with your code

**Accessibility First**
- WCAG 2.1 AA compliance for all color combinations
- Colorblind-friendly palette tested with multiple types of color vision
- High contrast options without sacrificing the warm aesthetic

**Long Session Comfort**
- Reduced blue light in the color palette
- Balanced contrast that doesn't cause eye strain
- Consistent color relationships between light and dark modes

## Technical Details

### Color Palette Breakdown

**Light Theme (Warm Sunrise)**
```
Primary Background: #FAF4F2 (warm off-white)
Text: #384242 (deep forest green-gray)
Accent: #FA906E (sunset orange)
Selection: #FBD6B9 (soft peach)
Sidebar: #F5F1EB (warm cream)
```

**Dark Theme (Golden Hour)**
```
Primary Background: #2B2520 (rich dark brown)
Text: #E8DDD4 (warm cream)
Accent: #FA906E (sunset orange - consistent across themes)
Selection: #4A3D35 (warm dark selection)
Sidebar: #352B26 (darker warm brown)
```

### Syntax Highlighting Strategy

**Keywords & Control Flow**
- `if`, `for`, `function`: Warm orange (`#FA906E`) - draws attention to structure
- `return`, `break`: Slightly muted orange - important but not overwhelming

**Strings & Data**
- String literals: Warm yellow (`#F5BC5E`) - easy to scan, distinct from keywords
- Numbers: Soft coral (`#E8A87C`) - visible but not jarring

**Comments & Documentation**
- Comments: Muted brown (`#95726A`) - present but unobtrusive
- Documentation: Slightly brighter than comments for better readability

**Variables & Functions**
- Variables: Default text color - clean, readable
- Function names: Slightly emphasized with warm tones
- Parameters: Distinct but harmonious coloring

## Installation & Usage

### From VSCode Marketplace
1. Open VSCode Extensions panel (`Ctrl+Shift+X`)
2. Search for "Warm Sunset Theme"
3. Install by entro314labs
4. Go to Settings → Color Theme → Select "Warm Sunset - Light" or "Warm Sunset - Dark"

### Manual Installation
```bash
# Clone the repository
git clone https://github.com/idominikosgr/warm-sunset-vscode-theme

# Package the extension
cd warm-sunset-vscode-theme
npm run package

# Install the .vsix file in VSCode
```

### Theme Switching Tips
- **Morning coding:** Start with Warm Sunset Light for natural daylight harmony
- **Evening sessions:** Switch to Warm Sunset Dark as ambient light decreases
- **Pair with:** Warm white monitor lighting (3000K-4000K color temperature)
- **Font recommendations:** Work great with Fira Code, JetBrains Mono, or SF Mono

## Language Support & Screenshots

### Fully Tested Languages
- **Web:** JavaScript, TypeScript, HTML, CSS, React JSX
- **Backend:** Python, Node.js, Go, Rust, Java
- **Data:** SQL, JSON, YAML, Markdown
- **Config:** .env files, Docker, shell scripts
- **Documentation:** Comments, JSDoc, Python docstrings

### Real Developer Feedback

*"Finally, a theme that doesn't make my eyes hurt during late-night coding sessions."* - JavaScript developer

*"The warm colors actually help me focus. Feels less clinical than other themes."* - Python backend engineer

*"Both light and dark variants work perfectly. No jarring transitions when switching."* - Full-stack developer

## Part of Warm Sunset Design System

This VSCode theme is the first implementation of the broader **Warm Sunset Design System** being developed at entro314 labs.

### Design System Features
- **Color palette:** Consistent warm tones across all applications
- **Accessibility:** WCAG 2.1 AA compliant color combinations
- **Multi-platform:** VSCode theme, web components, design tokens
- **Framework agnostic:** Works with React, Vue, vanilla CSS, Tailwind

### Future Implementations
- **Web components:** React/Vue component library with Warm Sunset colors
- **Design tokens:** CSS custom properties and Tailwind config
- **Terminal themes:** iTerm2 and other terminal color schemes
- **Browser extensions:** Consistent theming across development tools

## Technical Implementation

### Theme Architecture
```
warm-sunset-theme/
├── themes/
│   ├── warm-sunset-light-color-theme.json    # Light variant
│   └── warm-sunset-dark-color-theme.json     # Dark variant
├── images/
│   └── icon.png                              # VSCode marketplace icon
├── package.json                              # Extension metadata
└── README.md                                 # Installation instructions
```

### Color Token System
All colors use consistent naming across light/dark themes:
- `primary-bg`: Main editor background
- `secondary-bg`: Sidebar and panel backgrounds  
- `accent-orange`: Interactive elements and highlights
- `text-primary`: Main code text
- `text-muted`: Comments and less important text

### Extension Compatibility
- **VSCode version:** Supports 1.15.0 and above
- **File size:** Lightweight at under 50KB
- **Performance:** No runtime impact, pure JSON color definitions
- **Updates:** Regular maintenance and color refinements

## Open Source & Community

### Contributing
The Warm Sunset Theme is open source and part of entro314 labs' research into accessible, inclusive design systems.

**Ways to contribute:**
- **Language support:** Test with your favorite programming languages
- **Accessibility feedback:** Report color contrast or readability issues  
- **Feature requests:** Suggest improvements to the color palette
- **Bug reports:** File issues for any display problems

### Repository Information
- **GitHub:** https://github.com/idominikosgr/warm-sunset-vscode-theme
- **License:** MIT - free for personal and commercial use
- **Maintainer:** entro314 labs
- **Issues:** Active response to community feedback

### Development Roadmap
- **v1.1:** Terminal integrated theme colors
- **v1.2:** Additional language syntax improvements
- **v2.0:** Integration with full Warm Sunset Design System
- **Community themes:** Variations based on user feedback

## Installation Troubleshooting

### Common Issues

**Theme not appearing in list:**
- Restart VSCode after installation
- Check Extensions panel to ensure installation completed

**Colors look different than screenshots:**
- Verify monitor color calibration
- Check VSCode settings for color customization overrides
- Some syntax highlighting depends on language extensions

**Accessibility concerns:**
- Report specific color contrast issues on GitHub
- Custom color overrides available through VSCode settings
- High contrast alternative being developed

### VSCode Settings Integration
```json
{
  "workbench.colorTheme": "Warm Sunset - Light",
  "editor.fontFamily": "Fira Code, monospace",
  "editor.fontSize": 14,
  "editor.lineHeight": 1.5,
  "workbench.iconTheme": "vs-seti"
}
```

---

## Content Messaging

### Key Selling Points
1. **Comfort-focused:** Designed for long coding sessions without eye strain
2. **Professionally warm:** Inviting without being unprofessional  
3. **Accessibility conscious:** WCAG compliant, colorblind-friendly
4. **Dual themes:** Consistent light/dark experience
5. **Active development:** Part of larger design system research

### Tone Guidelines
- **Welcoming but technical:** Appeal to developers who care about their tools
- **Honest about scope:** Clear about what it does well vs. limitations
- **Community-focused:** Emphasize open source and feedback welcome
- **Professional warmth:** Comfortable but not cutesy

### Call-to-Action Priority
1. **Install from VSCode Marketplace** (primary action)
2. **View GitHub repository** (for technical users)
3. **Report issues or feedback** (community building)
4. **Explore other entro314 projects** (ecosystem awareness)