# Obsidian Theme (2025 Edition)

Obsidian has evolved significantly since its early days, and in 2025 it offers a robust theming system with support for advanced CSS features, animations, and component-level customization. The Warm Sunset theme for Obsidian provides a cozy and visually pleasing experience for both light and dark modes.

## Installation Instructions

### Method 1: Community Themes

1. Open Obsidian
2. Go to `Settings` > `Appearance` > `Themes`
3. Click `Browse` to open the community themes browser
4. Search for "Warm Sunset"
5. Click `Install` and then `Use`

### Method 2: Manual Installation

1. Download the theme files (`theme.css` and `manifest.json`)
2. Locate your Obsidian vault's theme folder:
   - Windows: `%APPDATA%\Obsidian\Themes`
   - macOS: `~/Library/Application Support/Obsidian/Themes`
   - Linux: `~/.config/Obsidian/Themes`
3. Create a folder named `warm-sunset` in the themes directory
4. Place the downloaded files in the folder
5. Open Obsidian and go to `Settings` > `Appearance` > `Themes`
6. Select "Warm Sunset" from the dropdown menu

## Theme Files

### manifest.json

```json
{
  "name": "Warm Sunset",
  "version": "1.0.0",
  "minAppVersion": "1.5.0",
  "author": "Your Name",
  "authorUrl": "https://your-website.com",
  "description": "A warm and cozy theme with sunset colors for both light and dark modes",
  "fundingUrl": "https://your-funding-link.com",
  "isDesktopOnly": false,
  "features": {
    "customCSS": true,
    "customPropertyFolding": true,
    "customThemeComponents": true,
    "animatedTransitions": true,
    "responsiveDesign": true,
    "darkMode": true,
    "lightMode": true,
    "canvas": true,
    "graphView": true,
    "nestedTabs": true,
    "tableEnhancements": true,
    "colorfulHeadings": true,
    "colorfulFolders": true
  },
  "themeColors": {
    "dark": {
      "primary": "#FA906E",
      "secondary": "#403A40",
      "accent": "#F5BC5E",
      "background": "#2A2023",
      "foreground": "#C6D0F5"
    },
    "light": {
      "primary": "#FA906E",
      "secondary": "#FDE6DE",
      "accent": "#F5BC5E",
      "background": "#FAF4F2",
      "foreground": "#384242"
    }
  },
  "screenshots": [
    "assets/screenshot-dark.png",
    "assets/screenshot-light.png"
  ]
}
```

### theme.css

```css
/* 
 * Warm Sunset Theme for Obsidian
 * Created by: Your Name
 * 2025 Edition
 */

/* Import Obsidian API 2.0 (2025 feature) */
@import url('obsidian://api/styles/2.0');

/* ===== Variable definitions ===== */
:root {
  /* Light Mode */
  --warm-sunset-light-background: #FAF4F2;
  --warm-sunset-light-background-secondary: #F5F1EB;
  --warm-sunset-light-background-tertiary: #FDE6DE;
  --warm-sunset-light-foreground: #384242;
  --warm-sunset-light-foreground-secondary: #95726A;
  --warm-sunset-light-primary: #FA906E;
  --warm-sunset-light-secondary: #FDE6DE;
  --warm-sunset-light-accent: #F5BC5E;
  --warm-sunset-light-muted: #F5F1EB;
  --warm-sunset-light-muted-text: #95726A;
  --warm-sunset-light-success: #A6D18C;
  --warm-sunset-light-warning: #F4BC5F;
  --warm-sunset-light-error: #E06053;
  --warm-sunset-light-border: #EADBCC;
  --warm-sunset-light-selection: #FBD6B9;
  --warm-sunset-light-link: #FA906E;
  
  /* Dark Mode */
  --warm-sunset-dark-background: #2A2023;
  --warm-sunset-dark-background-secondary: #342D34;
  --warm-sunset-dark-background-tertiary: #403A40;
  --warm-sunset-dark-foreground: #C6D0F5;
  --warm-sunset-dark-foreground-secondary: #B5A9AF;
  --warm-sunset-dark-primary: #FA906E;
  --warm-sunset-dark-secondary: #403A40;
  --warm-sunset-dark-accent: #F5BC5E;
  --warm-sunset-dark-muted: #342D34;
  --warm-sunset-dark-muted-text: #B5A9AF;
  --warm-sunset-dark-success: #A6D18C;
  --warm-sunset-dark-warning: #E5C890;
  --warm-sunset-dark-error: #E78284;
  --warm-sunset-dark-border: #403A40;
  --warm-sunset-dark-selection: #626880;
  --warm-sunset-dark-link: #F594C1;
}

/* ===== Light Theme ===== */
.theme-light {
  --background-primary: var(--warm-sunset-light-background);
  --background-primary-alt: var(--warm-sunset-light-background-secondary);
  --background-secondary: var(--warm-sunset-light-background-secondary);
  --background-secondary-alt: var(--warm-sunset-light-background-tertiary);
  --background-modifier-border: var(--warm-sunset-light-border);
  --background-modifier-form-field: var(--warm-sunset-light-background);
  --background-modifier-form-field-highlighted: var(--warm-sunset-light-secondary);
  --background-modifier-box-shadow: rgba(0, 0, 0, 0.05);
  --background-modifier-success: var(--warm-sunset-light-success);
  --background-modifier-error: var(--warm-sunset-light-error);
  --background-modifier-error-rgb: 224, 96, 83;
  --background-modifier-error-hover: var(--warm-sunset-light-error);
  --background-modifier-cover: rgba(250, 244, 242, 0.8);
  
  --text-normal: var(--warm-sunset-light-foreground);
  --text-muted: var(--warm-sunset-light-foreground-secondary);
  --text-faint: var(--warm-sunset-light-muted-text);
  --text-accent: var(--warm-sunset-light-primary);
  --text-accent-hover: var(--warm-sunset-light-accent);
  --text-on-accent: #FAF4F2;
  --text-error: var(--warm-sunset-light-error);
  --text-error-hover: var(--warm-sunset-light-error);
  --text-highlight-bg: var(--warm-sunset-light-selection);
  --text-selection: var(--warm-sunset-light-selection);
  
  --interactive-normal: var(--warm-sunset-light-background-secondary);
  --interactive-hover: var(--warm-sunset-light-background-tertiary);
  --interactive-accent: var(--warm-sunset-light-primary);
  --interactive-accent-rgb: 250, 144, 110;
  --interactive-accent-hover: var(--warm-sunset-light-accent);
  --interactive-success: var(--warm-sunset-light-success);
  
  --scrollbar-bg: var(--warm-sunset-light-background-secondary);
  --scrollbar-thumb-bg: var(--warm-sunset-light-border);
  --scrollbar-active-thumb-bg: var(--warm-sunset-light-accent);
  
  --highlight-mix-blend-mode: darken;
  
  --border-color: var(--warm-sunset-light-border);
  
  --link-color: var(--warm-sunset-light-link);
  --link-color-hover: var(--warm-sunset-light-accent);
  --link-decoration: none;
  --link-decoration-hover: underline;
  
  --tag-color: var(--warm-sunset-light-primary);
  --tag-background: var(--warm-sunset-light-secondary);
  --tag-padding-x: 8px;
  --tag-padding-y: 2px;
  --tag-radius: 16px;
  
  --tab-background-active: var(--warm-sunset-light-background);
  --tab-text-color: var(--warm-sunset-light-foreground-secondary);
  --tab-text-color-active: var(--warm-sunset-light-primary);
  --tab-background-hover: var(--warm-sunset-light-secondary);
  
  --titlebar-background: var(--warm-sunset-light-background);
  --titlebar-text-color: var(--warm-sunset-light-foreground);
  
  --canvas-background: var(--warm-sunset-light-background-secondary);
  --canvas-node-background: var(--warm-sunset-light-background);
  --canvas-node-border: var(--warm-sunset-light-border);
  --canvas-node-selected-border: var(--warm-sunset-light-primary);
  
  --graph-background: var(--warm-sunset-light-background-secondary);
  --graph-line-color: var(--warm-sunset-light-border);
  --graph-node-color: var(--warm-sunset-light-primary);
  --graph-node-hover-color: var(--warm-sunset-light-accent);
}

/* ===== Dark Theme ===== */
.theme-dark {
  --background-primary: var(--warm-sunset-dark-background);
  --background-primary-alt: var(--warm-sunset-dark-background-secondary);
  --background-secondary: var(--warm-sunset-dark-background-secondary);
  --background-secondary-alt: var(--warm-sunset-dark-background-tertiary);
  --background-modifier-border: var(--warm-sunset-dark-border);
  --background-modifier-form-field: var(--warm-sunset-dark-background);
  --background-modifier-form-field-highlighted: var(--warm-sunset-dark-secondary);
  --background-modifier-box-shadow: rgba(0, 0, 0, 0.3);
  --background-modifier-success: var(--warm-sunset-dark-success);
  --background-modifier-error: var(--warm-sunset-dark-error);
  --background-modifier-error-rgb: 231, 130, 132;
  --background-modifier-error-hover: var(--warm-sunset-dark-error);
  --background-modifier-cover: rgba(42, 32, 35, 0.8);
  
  --text-normal: var(--warm-sunset-dark-foreground);
  --text-muted: var(--warm-sunset-dark-foreground-secondary);
  --text-faint: var(--warm-sunset-dark-muted-text);
  --text-accent: var(--warm-sunset-dark-primary);
  --text-accent-hover: var(--warm-sunset-dark-accent);
  --text-on-accent: #2A2023;
  --text-error: var(--warm-sunset-dark-error);
  --text-error-hover: var(--warm-sunset-dark-error);
  --text-highlight-bg: var(--warm-sunset-dark-selection);
  --text-selection: var(--warm-sunset-dark-selection);
  
  --interactive-normal: var(--warm-sunset-dark-background-secondary);
  --interactive-hover: var(--warm-sunset-dark-background-tertiary);
  --interactive-accent: var(--warm-sunset-dark-primary);
  --interactive-accent-rgb: 250, 144, 110;
  --interactive-accent-hover: var(--warm-sunset-dark-accent);
  --interactive-success: var(--warm-sunset-dark-success);
  
  --scrollbar-bg: var(--warm-sunset-dark-background-secondary);
  --scrollbar-thumb-bg: var(--warm-sunset-dark-border);
  --scrollbar-active-thumb-bg: var(--warm-sunset-dark-accent);
  
  --highlight-mix-blend-mode: lighten;
  
  --border-color: var(--warm-sunset-dark-border);
  
  --link-color: var(--warm-sunset-dark-link);
  --link-color-hover: var(--warm-sunset-dark-accent);
  --link-decoration: none;
  --link-decoration-hover: underline;
  
  --tag-color: var(--warm-sunset-dark-primary);
  --tag-background: var(--warm-sunset-dark-secondary);
  --tag-padding-x: 8px;
  --tag-padding-y: 2px;
  --tag-radius: 16px;
  
  --tab-background-active: var(--warm-sunset-dark-background);
  --tab-text-color: var(--warm-sunset-dark-foreground-secondary);
  --tab-text-color-active: var(--warm-sunset-dark-primary);
  --tab-background-hover: var(--warm-sunset-dark-secondary);
  
  --titlebar-background: var(--warm-sunset-dark-background);
  --titlebar-text-color: var(--warm-sunset-dark-foreground);
  
  --canvas-background: var(--warm-sunset-dark-background-secondary);
  --canvas-node-background: var(--warm-sunset-dark-background);
  --canvas-node-border: var(--warm-sunset-dark-border);
  --canvas-node-selected-border: var(--warm-sunset-dark-primary);
  
  --graph-background: var(--warm-sunset-dark-background-secondary);
  --graph-line-color: var(--warm-sunset-dark-border);
  --graph-node-color: var(--warm-sunset-dark-primary);
  --graph-node-hover-color: var(--warm-sunset-dark-accent);
}

/* ===== Typography ===== */
body {
  --font-text: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  --font-editor: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  --font-monospace: 'Fira Code', 'Source Code Pro', monospace;
  --font-ui: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  
  /* Font weights */
  --font-normal: 400;
  --font-medium: 500;
  --font-semibold: 600;
  --font-bold: 700;
  
  /* Line heights */
  --line-height-normal: 1.5;
  --line-height-tight: 1.3;
  --line-height-loose: 1.8;
  
  /* Font size */
  --font-scale: 1.0;
  --font-smaller: calc(0.8rem * var(--font-scale));
  --font-small: calc(0.9rem * var(--font-scale));
  --font-normal: calc(1.0rem * var(--font-scale));
  --font-large: calc(1.1rem * var(--font-scale));
  --font-larger: calc(1.3rem * var(--font-scale));
  --font-largest: calc(1.5rem * var(--font-scale));
}

/* ===== UI Component Styling ===== */

/* Sidebar & Navigation */
.nav-folder-title {
  color: var(--text-muted);
  font-weight: var(--font-medium);
  padding: 4px 12px;
  border-radius: 4px;
  transition: all 0.2s ease;
}

.nav-folder-title:hover {
  color: var(--text-normal);
  background-color: var(--interactive-hover);
}

.nav-file-title {
  padding: 4px 12px 4px 20px;
  border-radius: 4px;
  transition: all 0.2s ease;
}

.nav-file-title:hover {
  background-color: var(--interactive-hover);
}

.nav-file-title.is-active {
  background-color: var(--interactive-hover);
  color: var(--text-accent);
  font-weight: var(--font-medium);
  border-left: 2px solid var(--interactive-accent);
}

/* Tabs */
.workspace-tab-header-container {
  background-color: var(--background-secondary);
  border-bottom: 1px solid var(--border-color);
}

.workspace-tab-header {
  position: relative;
  transition: all 0.2s ease;
}

.workspace-tab-header.is-active {
  color: var(--tab-text-color-active);
}

.workspace-tab-header.is-active::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 2px;
  background-color: var(--interactive-accent);
}

/* Buttons */
.clickable-icon {
  color: var(--text-muted);
  transition: all 0.2s ease;
}

.clickable-icon:hover {
  color: var(--text-accent);
  background-color: var(--interactive-hover);
}

button {
  border-radius: 4px;
  transition: all 0.2s ease;
}

button:hover {
  transform: translateY(-1px);
}

.mod-cta {
  background-color: var(--interactive-accent) !important;
  color: var(--text-on-accent) !important;
}

.mod-cta:hover {
  background-color: var(--interactive-accent-hover) !important;
}

.suggestion-item.is-selected {
  background-color: var(--interactive-hover);
}

/* Editor */
.cm-s-obsidian {
  font-family: var(--font-editor);
  font-size: var(--font-normal);
  line-height: var(--line-height-normal);
}

.cm-header-1,
.cm-header-2,
.cm-header-3,
.cm-header-4,
.cm-header-5,
.cm-header-6 {
  font-weight: var(--font-bold);
  line-height: var(--line-height-tight);
}

.cm-header-1 {
  font-size: var(--font-largest);
  color: var(--text-accent);
}

.cm-header-2 {
  font-size: var(--font-larger);
  color: var(--text-accent);
}

.cm-header-3 {
  font-size: var(--font-large);
  color: var(--text-accent);
}

.cm-formatting-header-1,
.cm-formatting-header-2,
.cm-formatting-header-3,
.cm-formatting-header-4,
.cm-formatting-header-5,
.cm-formatting-header-6 {
  color: var(--text-accent);
}

.cm-formatting-list-ul,
.cm-formatting-list-ol {
  color: var(--text-accent);
}

.cm-formatting-code,
.cm-formatting-code-block {
  color: var(--text-muted);
}

.cm-inline-code {
  font-family: var(--font-monospace);
  color: var(--text-accent);
  background-color: var(--interactive-normal);
  padding: 0.1em 0.4em;
  border-radius: 3px;
}

.CodeMirror-cursor {
  border-left: 2px solid var(--text-accent);
}

.cm-fat-cursor .CodeMirror-cursor {
  background-color: var(--text-accent);
}

.cm-searching {
  background-color: var(--text-highlight-bg);
  outline: 1px solid var(--background-modifier-border);
}

/* Code blocks */
.markdown-preview-view pre[class*="language-"],
.markdown-preview-view code[class*="language-"],
.HyperMD-codeblock {
  font-family: var(--font-monospace);
  font-size: var(--font-small);
}

.markdown-preview-view pre {
  padding: 16px;
  border-radius: 8px;
  background-color: var(--background-secondary-alt);
  border: 1px solid var(--border-color);
}

.theme-dark .token.comment,
.theme-dark .token.prolog,
.theme-dark .token.doctype,
.theme-dark .token.cdata {
  color: var(--warm-sunset-dark-muted-text);
}

.theme-dark .token.punctuation {
  color: var(--warm-sunset-dark-foreground);
}

.theme-dark .token.property,
.theme-dark .token.tag,
.theme-dark .token.boolean,
.theme-dark .token.number,
.theme-dark .token.constant,
.theme-dark .token.symbol {
  color: var(--warm-sunset-dark-accent);
}

.theme-dark .token.selector,
.theme-dark .token.attr-name,
.theme-dark .token.string,
.theme-dark .token.char,
.theme-dark .token.builtin {
  color: var(--warm-sunset-dark-success);
}

.theme-dark .token.operator,
.theme-dark .token.entity,
.theme-dark .token.url,
.theme-dark .token.variable {
  color: var(--warm-sunset-dark-foreground);
}

.theme-dark .token.atrule,
.theme-dark .token.attr-value,
.theme-dark .token.function {
  color: var(--warm-sunset-dark-primary);
}

.theme-dark .token.keyword {
  color: var(--warm-sunset-dark-link);
}

.theme-dark .token.regex,
.theme-dark .token.important {
  color: var(--warm-sunset-dark-warning);
}

.theme-light .token.comment,
.theme-light .token.prolog,
.theme-light .token.doctype,
.theme-light .token.cdata {
  color: var(--warm-sunset-light-muted-text);
}

.theme-light .token.punctuation {
  color: var(--warm-sunset-light-foreground);
}

.theme-light .token.property,
.theme-light .token.tag,
.theme-light .token.boolean,
.theme-light .token.number,
.theme-light .token.constant,
.theme-light .token.symbol {
  color: var(--warm-sunset-light-accent);
}

.theme-light .token.selector,
.theme-light .token.attr-name,
.theme-light .token.string,
.theme-light .token.char,
.theme-light .token.builtin {
  color: var(--warm-sunset-light-success);
}

.theme-light .token.operator,
.theme-light .token.entity,
.theme-light .token.url,
.theme-light .token.variable {
  color: var(--warm-sunset-light-foreground);
}

.theme-light .token.atrule,
.theme-light .token.attr-value,
.theme-light .token.function {
  color: var(--warm-sunset-light-primary);
}

.theme-light .token.keyword {
  color: var(--warm-sunset-light-link);
}

.theme-light .token.regex,
.theme-light .token.important {
  color: var(--warm-sunset-light-warning);
}

/* Tags */
a.tag {
  font-size: var(--font-small);
  background-color: var(--tag-background);
  color: var(--tag-color);
  padding: var(--tag-padding-y) var(--tag-padding-x);
  border-radius: var(--tag-radius);
  text-decoration: none;
  transition: all 0.2s ease;
}

a.tag:hover {
  background-color: var(--interactive-accent);
  color: var(--text-on-accent);
  transform: translateY(-1px);
}

/* Tables */
.markdown-preview-view table {
  width: 100%;
  border-collapse: collapse;
  margin: 1em 0;
  overflow: hidden;
  border-radius: 8px;
  border: 1px solid var(--border-color);
}

.markdown-preview-view th {
  background-color: var(--interactive-hover);
  font-weight: var(--font-medium);
  border-bottom: 1px solid var(--border-color);
}

.markdown-preview-view td,
.markdown-preview-view th {
  padding: 8px 12px;
  border: none;
}

.markdown-preview-view tr:nth-child(even) {
  background-color: var(--background-primary-alt);
}

.markdown-preview-view tr:hover {
  background-color: var(--interactive-hover);
}

/* Blockquotes */
.markdown-preview-view blockquote {
  border-left: 4px solid var(--interactive-accent);
  background-color: var(--background-primary-alt);
  padding: 1em;
  margin: 1em 0;
  border-radius: 0 8px 8px 0;
}

/* Checkboxes */
.task-list-item-checkbox {
  border: 1px solid var(--text-muted);
  border-radius: 3px;
  margin-right: 8px;
  transition: all 0.2s ease;
}

.task-list-item-checkbox:checked {
  background-color: var(--interactive-accent);
  border-color: var(--interactive-accent);
}

input.task-list-item-checkbox:checked::before {
  color: var(--text-on-accent);
}

/* Graph View */
.graph-view.color-fill {
  color: var(--graph-node-color);
}

.graph-view.color-line {
  color: var(--graph-line-color);
}

.graph-view.color-text {
  color: var(--text-normal);
}

.graph-view.color-fill-highlight {
  color: var(--graph-node-hover-color);
}

.graph-view.color-line-highlight {
  color: var(--interactive-accent);
}

/* Canvas */
.canvas {
  background-color: var(--canvas-background);
}

.canvas-node {
  background-color: var(--canvas-node-background);
  border: 1px solid var(--canvas-node-border);
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  transition: all 0.2s ease;
}

.canvas-node.is-selected {
  border-color: var(--canvas-node-selected-border);
  box-shadow: 0 0 0 2px var(--canvas-node-selected-border);
}

/* Callouts (2023+ Feature) */
.callout {
  border-radius: 8px;
  padding: 16px;
  margin: 16px 0;
  border-left: 4px solid var(--callout-color);
  background-color: var(--background-primary-alt);
}

.callout-title {
  display: flex;
  align-items: center;
  margin-bottom: 8px;
  color: var(--callout-color);
  font-weight: var(--font-medium);
}

.callout-icon {
  margin-right: 8px;
}

.callout-content {
  color: var(--text-normal);
}

.callout[data-callout="note"] {
  --callout-color: var(--text-accent);
}

.callout[data-callout="info"] {
  --callout-color: var(--warm-sunset-light-link);
}

.callout[data-callout="warning"] {
  --callout-color: var(--warm-sunset-light-warning);
}

.callout[data-callout="error"] {
  --callout-color: var(--warm-sunset-light-error);
}

.callout[data-callout="success"] {
  --callout-color: var(--warm-sunset-light-success);
}

.theme-dark .callout[data-callout="info"] {
  --callout-color: var(--warm-sunset-dark-link);
}

.theme-dark .callout[data-callout="warning"] {
  --callout-color: var(--warm-sunset-dark-warning);
}

.theme-dark .callout[data-callout="error"] {
  --callout-color: var(--warm-sunset-dark-error);
}

.theme-dark .callout[data-callout="success"] {
  --callout-color: var(--warm-sunset-dark-success);
}

/* ===== Animations & Transitions ===== */
.workspace-leaf {
  transition: width 0.2s ease, opacity 0.2s ease;
}

.workspace-leaf.mod-active {
  transition: width 0.2s ease, opacity 0.2s ease;
}

/* ===== Responsive Design ===== */
@media (max-width: 768px) {
  body {
    --font-scale: 0.95;
  }
  
  .markdown-preview-view {
    padding: 10px !important;
  }
}

/* ===== Modern Obsidian Features (2025) ===== */

/* Custom property folding */
.property-folding-indicator {
  color: var(--text-muted);
  transition: all 0.2s ease;
}

.property-folding-indicator:hover {
  color: var(--text-accent);
}

/* New tab enhancements */
.workspace-tab-header-container-inner {
  padding-bottom: 1px;
}

.workspace-tab-header.is-active {
  position: relative;
  overflow: visible;
}

.workspace-tab-header.is-active::before {
  content: "";
  position: absolute;
  bottom: -1px;
  left: 0;
  right: 0;
  height: 2px;
  background-color: var(--interactive-accent);
  border-radius: 2px 2px 0 0;
  z-index: 1;
}

/* Advanced Tables */
.table-view-table {
  border-collapse: collapse;
  width: 100%;
  overflow: hidden;
  border-radius: 8px;
  border: 1px solid var(--border-color);
}

.table-view-table th {
  background-color: var(--interactive-hover);
  padding: 8px 12px;
  font-weight: var(--font-medium);
  text-align: left;
  border-bottom: 1px solid var(--border-color);
  position: relative;
}

.table-view-table td {
  padding: 8px 12px;
  border: none;
  transition: all 0.1s ease;
}

.table-view-table tr:nth-child(even) {
  background-color: var(--background-primary-alt);
}

.table-view-table tr:hover td {
  background-color: var(--interactive-hover);
}

/* Colorful headings (2025 feature) */
.markdown-preview-view h1 {
  color: var(--warm-sunset-light-primary);
  border-bottom: 2px solid var(--warm-sunset-light-primary);
  padding-bottom: 0.2em;
}

.markdown-preview-view h2 {
  color: var(--warm-sunset-light-accent);
}

.markdown-preview-view h3 {
  color: var(--warm-sunset-light-link);
}

.theme-dark .markdown-preview-view h1 {
  color: var(--warm-sunset-dark-primary);
  border-bottom: 2px solid var(--warm-sunset-dark-primary);
}

.theme-dark .markdown-preview-view h2 {
  color: var(--warm-sunset-dark-accent);
}

.theme-dark .markdown-preview-view h3 {
  color: var(--warm-sunset-dark-link);
}

/* Colorful folders (2025 feature) */
.nav-folder.mod-root > .nav-folder-children > .nav-folder > .nav-folder-title {
  color: var(--warm-sunset-light-primary);
  font-weight: var(--font-semibold);
}

.nav-folder.mod-root > .nav-folder-children > .nav-folder:nth-child(3n+1) > .nav-folder-title {
  color: var(--warm-sunset-light-primary);
}

.nav-folder.mod-root > .nav-folder-children > .nav-folder:nth-child(3n+2) > .nav-folder-title {
  color: var(--warm-sunset-light-accent);
}

.nav-folder.mod-root > .nav-folder-children > .nav-folder:nth-child(3n+3) > .nav-folder-title {
  color: var(--warm-sunset-light-link);
}

.theme-dark .nav-folder.mod-root > .nav-folder-children > .nav-folder > .nav-folder-title {
  color: var(--warm-sunset-dark-primary);
}

.theme-dark .nav-folder.mod-root > .nav-folder-children > .nav-folder:nth-child(3n+1) > .nav-folder-title {
  color: var(--warm-sunset-dark-primary);
}

.theme-dark .nav-folder.mod-root > .nav-folder-children > .nav-folder:nth-child(3n+2) > .nav-folder-title {
  color: var(--warm-sunset-dark-accent);
}

.theme-dark .nav-folder.mod-root > .nav-folder-children > .nav-folder:nth-child(3n+3) > .nav-folder-title {
  color: var(--warm-sunset-dark-link);
}

/* AI features support (hypothetical 2025 feature) */
.ai-suggestion {
  background-color: var(--background-primary-alt);
  border-left: 4px solid var(--interactive-accent);
  padding: 12px;
  margin: 16px 0;
  border-radius: 0 8px 8px 0;
  position: relative;
}

.ai-suggestion::before {
  content: "✨";
  position: absolute;
  top: 8px;
  right: 12px;
  font-size: 16px;
}

.ai-suggestion-header {
  font-weight: var(--font-medium);
  color: var(--text-accent);
  margin-bottom: 8px;
}

.ai-suggestion-content {
  color: var(--text-normal);
}

.ai-suggestion-actions {
  margin-top: 8px;
  display: flex;
  gap: 8px;
}

.ai-suggestion-action {
  font-size: var(--font-smaller);
  padding: 2px 8px;
  border-radius: 4px;
  background-color: var(--background-secondary);
  color: var(--text-muted);
  cursor: pointer;
  transition: all 0.2s ease;
}

.ai-suggestion-action:hover {
  background-color: var(--interactive-hover);
  color: var(--text-normal);
}

.ai-suggestion-action.primary {
  background-color: var(--interactive-accent);
  color: var(--text-on-accent);
}

.ai-suggestion-action.primary:hover {
  background-color: var(--interactive-accent-hover);
}
```

## Advanced Features and Customization

### Theme Snippets

For further customization, you can add CSS snippets in Obsidian. Go to `Settings` > `Appearance` > `CSS Snippets` and create a new snippet with custom modifications:

```css
/* Example snippet for extra customization */
.theme-light,
.theme-dark {
  --custom-accent: #F5BC5E;  /* Override accent color */
}

/* Custom link animations */
.internal-link {
  position: relative;
}

.internal-link::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 0;
  height: 2px;
  background-color: var(--interactive-accent);
  transition: width 0.3s ease;
}

.internal-link:hover::after {
  width: 100%;
}

/* Custom animated checkbox */
.task-list-item-checkbox {
  position: relative;
  overflow: hidden;
}

.task-list-item-checkbox:checked::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: var(--interactive-accent);
  clip-path: circle(0% at center);
  animation: checkbox-check 0.3s ease forwards;
}

@keyframes checkbox-check {
  0% {
    clip-path: circle(0% at center);
  }
  100% {
    clip-path: circle(100% at center);
  }
}
```

### Style Settings Support (2025 Feature)

Obsidian's Style Settings plugin has evolved in 2025 to support advanced theme customization. Here's how to add Style Settings support to your theme:

1. Add a `theme-settings.css` file to your theme folder:

```css
/* @settings
name: Warm Sunset Theme Settings
id: warm-sunset-theme
settings:
  - 
    id: warm-sunset-theme-heading
    title: Warm Sunset Theme Settings
    type: heading
    level: 1
    description: Customize the Warm Sunset theme to your liking
  - 
    id: warm-sunset-color-scheme
    title: Color Scheme
    type: heading
    level: 2
    description: Customize the theme colors
  - 
    id: warm-sunset-primary-color
    title: Primary Color
    type: variable-color
    format: hex
    default: '#FA906E'
    description: Main accent color used throughout the theme
  - 
    id: warm-sunset-accent-color
    title: Accent Color
    type: variable-color
    format: hex
    default: '#F5BC5E'
    description: Secondary accent color used for highlights
  - 
    id: warm-sunset-typography
    title: Typography
    type: heading
    level: 2
    description: Customize the fonts and typography
  - 
    id: warm-sunset-font-scale
    title: Font Size Scale
    type: variable-number
    default: 1
    min: 0.8
    max: 1.5
    step: 0.05
    description: Adjust the overall font size (requires restart)
  - 
    id: warm-sunset-line-height
    title: Line Height
    type: variable-number
    default: 1.5
    min: 1.1
    max: 2
    step: 0.1
    description: Adjust the line height for the editor
  - 
    id: warm-sunset-ui-settings
    title: UI Settings
    type: heading
    level: 2
    description: Customize the user interface
  - 
    id: warm-sunset-border-radius
    title: Border Radius
    type: variable-number
    default: 8
    min: 0
    max: 20
    step: 1
    description: Adjust the border radius for UI elements
  - 
    id: warm-sunset-animation-speed
    title: Animation Speed
    type: variable-number
    default: 0.2
    min: 0
    max: 1
    step: 0.05
    description: Adjust the speed of UI animations (in seconds)
  - 
    id: warm-sunset-features
    title: Special Features
    type: heading
    level: 2
    description: Enable or disable special theme features
  - 
    id: warm-sunset-colorful-headings
    title: Colorful Headings
    type: class-toggle
    default: true
    description: Use different colors for headings
  - 
    id: warm-sunset-colorful-folders
    title: Colorful Folders
    type: class-toggle
    default: true
    description: Use different colors for folders
  - 
    id: warm-sunset-link-animations
    title: Link Animations
    type: class-toggle
    default: true
    description: Enable animated underlines for links
  - 
    id: warm-sunset-custom-callouts
    title: Custom Callouts
    type: class-toggle
    default: true
    description: Use theme-styled callouts
*/
```

2. Link this file to your `theme.css`:

```css
@import url('theme-settings.css');
```

### Theme Variants

You can also provide variant styles for your theme. Create a `variants` folder in your theme directory and add different variant CSS files:

#### High Contrast Variant

Create `variants/high-contrast.css`:

```css
/* High contrast variant */
.theme-light {
  --warm-sunset-light-foreground: #000000;
  --warm-sunset-light-foreground-secondary: #333333;
  --warm-sunset-light-background: #FFFFFF;
  --warm-sunset-light-background-secondary: #F0F0F0;
  --warm-sunset-light-primary: #E05A36;
  --warm-sunset-light-accent: #D78C28;
}

.theme-dark {
  --warm-sunset-dark-foreground: #FFFFFF;
  --warm-sunset-dark-foreground-secondary: #CCCCCC;
  --warm-sunset-dark-background: #000000;
  --warm-sunset-dark-background-secondary: #1A1A1A;
  --warm-sunset-dark-primary: #FF7F50;
  --warm-sunset-dark-accent: #FFB62F;
}
```

To enable theme variants, add a variant picker to your theme settings.

## Compatibility with Obsidian Mobile (2025)

Obsidian's mobile app has improved significantly in 2025, with better support for custom themes. The Warm Sunset theme is fully compatible with Obsidian Mobile, with responsive design for various screen sizes.

### Mobile-Specific Styles

Add these to your `theme.css`:

```css
/* Mobile improvements */
@media (max-width: 450px) {
  body {
    --font-scale: 0.9;
  }
  
  .workspace-leaf {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
  }
  
  /* Optimize touch targets */
  .nav-file-title,
  .nav-folder-title {
    padding: 8px 16px;
    min-height: 36px;
  }
  
  .clickable-icon {
    padding: 8px;
    min-height: 36px;
    min-width: 36px;
  }
  
  /* Improve mobile toolbar */
  .mobile-toolbar {
    background-color: var(--background-primary);
    border-top: 1px solid var(--border-color);
  }
  
  .mobile-toolbar-option {
    color: var(--text-muted);
  }
  
  .mobile-toolbar-option.selected {
    color: var(--text-accent);
  }
}
```
