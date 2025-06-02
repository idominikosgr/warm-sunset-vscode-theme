# Social Media Customization - Twitter/X and Reddit (2025 Edition)

In 2025, users have more options than ever to customize their social media experiences. While platforms have continued to evolve their own theming options, browser extensions remain the most powerful way to completely transform these websites with custom CSS. Here's how to apply the Warm Sunset theme to Twitter/X and Reddit.

## Twitter/X Dark Mode Customization

Twitter (now commonly known as X) has expanded its native theme support, but browser extensions still offer the most comprehensive customization options. 

### Recommended Browser Extensions (2025)

1. **Stylus** - The most widely used and actively maintained CSS injection extension
   - [Chrome Web Store](https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)
   - [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/styl-us/)
   - [Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/stylus/gkgbdnmjcgjjdpdnkfcgbibpomdjbnci)

2. **X Enhancer** (Hypothetical 2025 extension)
   - A specialized extension for X/Twitter with additional customization features
   - Supports advanced layout changes, feature toggles, and theme presets

### Installation Instructions

1. Install the Stylus browser extension
2. Navigate to Twitter/X (x.com)
3. Click on the Stylus icon in your browser toolbar
4. Click "Write new style for: x.com"
5. Give your style a name like "Warm Sunset for Twitter/X"
6. Paste the CSS code below
7. Click "Save"

### CSS for Twitter/X (Dark Mode)

```css
/* Warm Sunset Theme for Twitter/X (2025 edition) */
/* Dark Mode Only - Apply to: x.com */

:root {
  /* Base Colors */
  --warm-sunset-background: #2A2023;
  --warm-sunset-background-secondary: #342D34;
  --warm-sunset-background-tertiary: #403A40;
  --warm-sunset-foreground: #C6D0F5;
  --warm-sunset-foreground-secondary: #B5A9AF;
  --warm-sunset-primary: #FA906E;
  --warm-sunset-secondary: #403A40;
  --warm-sunset-accent: #F5BC5E;
  --warm-sunset-muted: #342D34;
  --warm-sunset-muted-text: #B5A9AF;
  --warm-sunset-success: #A6D18C;
  --warm-sunset-warning: #E5C890;
  --warm-sunset-error: #E78284;
  --warm-sunset-border: #403A40;
  --warm-sunset-selection: #626880;
  --warm-sunset-link: #F594C1;
  
  /* Twitter specific */
  --warm-sunset-tweet-background: #342D34;
  --warm-sunset-tweet-hover: #403A40;
  --warm-sunset-tweet-border: #403A40;
  --warm-sunset-button-bg: #403A40;
  --warm-sunset-button-hover: #504850;
  --warm-sunset-search-bg: #342D34;
  --warm-sunset-verified: #F5BC5E;
  --warm-sunset-retweet: #A6D18C;
  --warm-sunset-like: #E78284;
  --warm-sunset-reply: #89DCEB;
  
  /* Shadow effects */
  --warm-sunset-shadow-small: 0 2px 5px rgba(0, 0, 0, 0.2);
  --warm-sunset-shadow-medium: 0 5px 15px rgba(0, 0, 0, 0.2);
  --warm-sunset-shadow-large: 0 10px 25px rgba(0, 0, 0, 0.2);
  
  /* Animations */
  --warm-sunset-transition-fast: 0.15s ease;
  --warm-sunset-transition-normal: 0.25s ease;
  --warm-sunset-transition-slow: 0.35s ease;
}

/* ===== MAIN LAYOUT ===== */

/* Main background */
body {
  background-color: var(--warm-sunset-background) !important;
  color: var(--warm-sunset-foreground) !important;
}

/* Main container */
main, article, [role="main"] {
  background-color: var(--warm-sunset-background) !important;
  color: var(--warm-sunset-foreground) !important;
}

/* Sidebar */
header[role="banner"],
nav[role="navigation"],
[data-testid="sidebarColumn"],
aside[role="complementary"] {
  background-color: var(--warm-sunset-background) !important;
  border-right: 1px solid var(--warm-sunset-border) !important;
}

/* Primary sidebar */
[data-testid="primaryColumn"] {
  border-right-color: var(--warm-sunset-border) !important;
}

/* Timeline header */
[data-testid="toolBar"],
[data-testid="tweetButtonInline"],
[data-testid="tweetButton"],
[role="tablist"] {
  background-color: var(--warm-sunset-background) !important;
  border-bottom-color: var(--warm-sunset-border) !important;
}

/* Tweets */
article[data-testid="tweet"],
[data-testid="cellInnerDiv"],
[data-testid="UserCell"] {
  background-color: var(--warm-sunset-background) !important;
  border-color: var(--warm-sunset-tweet-border) !important;
  transition: background-color var(--warm-sunset-transition-fast) !important;
}

article[data-testid="tweet"]:hover,
[data-testid="cellInnerDiv"]:hover,
[data-testid="UserCell"]:hover {
  background-color: var(--warm-sunset-tweet-hover) !important;
}

/* Tweet text and content */
[data-testid="tweetText"],
[data-testid="tweetText"] span {
  color: var(--warm-sunset-foreground) !important;
}

/* Username and display name */
[data-testid="User-Name"] > div > div > a > div > div > span,
[data-testid="User-Name"] > div > div > div > span,
[data-testid="User-Name"] span[dir="auto"] {
  color: var(--warm-sunset-foreground) !important;
}

[data-testid="User-Name"] > div > div:last-child > div > span {
  color: var(--warm-sunset-foreground-secondary) !important;
}

/* Timestamps */
time, [data-testid="User-Name"] > div > div > div > span > span {
  color: var(--warm-sunset-foreground-secondary) !important;
}

/* Links */
a, a:visited {
  color: var(--warm-sunset-link) !important;
}

a:hover {
  text-decoration: underline !important;
  text-decoration-color: var(--warm-sunset-link) !important;
}

/* Hashtags and mentions */
a[href^="/hashtag/"], a[href^="/hashtag/"]:visited,
a[href^="/"]:not([href^="/home"]):not([href^="/explore"]):not([href^="/notifications"]):not([href^="/messages"]), 
a[href^="/"]:not([href^="/home"]):not([href^="/explore"]):not([href^="/notifications"]):not([href^="/messages"]):visited {
  color: var(--warm-sunset-primary) !important;
}

/* ===== COMPONENTS ===== */

/* Buttons */
[role="button"],
[data-testid="tweetButtonInline"],
[data-testid="tweetButton"] {
  background-color: var(--warm-sunset-button-bg) !important;
  transition: background-color var(--warm-sunset-transition-fast) !important;
}

[role="button"]:hover,
[data-testid="tweetButtonInline"]:hover,
[data-testid="tweetButton"]:hover {
  background-color: var(--warm-sunset-button-hover) !important;
}

/* Primary action buttons */
[data-testid="tweetButtonInline"],
[data-testid="tweetButton"],
[data-testid="primaryColumn"] div[role="button"][data-testid]:not([data-testid="app-bar-back"]) {
  background-color: var(--warm-sunset-primary) !important;
  color: var(--warm-sunset-background) !important;
}

[data-testid="tweetButtonInline"]:hover,
[data-testid="tweetButton"]:hover,
[data-testid="primaryColumn"] div[role="button"][data-testid]:not([data-testid="app-bar-back"]):hover {
  background-color: var(--warm-sunset-accent) !important;
}

/* Search box */
[data-testid="SearchBox_Search_Input"], 
input[placeholder="Search X"],
[role="search"],
[role="searchbox"],
[data-testid="SearchBox_Search_Input"]:focus {
  background-color: var(--warm-sunset-search-bg) !important;
  color: var(--warm-sunset-foreground) !important;
  border-color: var(--warm-sunset-border) !important;
}

/* Tabs and active states */
[role="tablist"] [role="tab"][aria-selected="true"],
[role="tablist"] [role="tab"][aria-selected="true"] div {
  color: var(--warm-sunset-primary) !important;
}

[role="tablist"] [role="tab"][aria-selected="true"] div[role="presentation"]::before {
  background-color: var(--warm-sunset-primary) !important;
}

/* Navigation items */
nav[role="navigation"] a {
  color: var(--warm-sunset-foreground) !important;
  transition: background-color var(--warm-sunset-transition-fast) !important;
}

nav[role="navigation"] a:hover {
  background-color: var(--warm-sunset-tweet-hover) !important;
}

nav[role="navigation"] a[aria-selected="true"] {
  font-weight: bold !important;
}

nav[role="navigation"] a[aria-selected="true"] span {
  color: var(--warm-sunset-primary) !important;
}

/* Tweet action icons */
[data-testid="reply"],
[data-testid="retweet"],
[data-testid="like"] {
  color: var(--warm-sunset-foreground-secondary) !important;
  transition: color var(--warm-sunset-transition-fast) !important;
}

[data-testid="reply"]:hover {
  color: var(--warm-sunset-reply) !important;
}

[data-testid="retweet"]:hover {
  color: var(--warm-sunset-retweet) !important;
}

[data-testid="like"]:hover {
  color: var(--warm-sunset-like) !important;
}

/* Verified checkmark */
[data-testid="icon-verified"] svg {
  fill: var(--warm-sunset-verified) !important;
}

/* Follow button */
[data-testid^="follow"], 
[data-testid^="follow"]:hover {
  background-color: var(--warm-sunset-primary) !important;
  color: var(--warm-sunset-background) !important;
}

/* ===== MODAL DIALOGS ===== */
[role="dialog"],
[role="dialog"] [role="document"] {
  background-color: var(--warm-sunset-background) !important;
  border-color: var(--warm-sunset-border) !important;
}

[role="dialog"] [role="document"] div[role="button"] {
  color: var(--warm-sunset-foreground) !important;
}

/* ===== SPECIFIC COMPONENTS (UPDATED FOR 2025) ===== */

/* Premium/Subscribers (previously Twitter Blue) */
[data-testid="premium-tier-badge"] {
  color: var(--warm-sunset-accent) !important;
}

/* Community panel (2025 feature) */
[data-testid="communityTab"],
[data-testid="communityHeader"] {
  background-color: var(--warm-sunset-background-secondary) !important;
  border-color: var(--warm-sunset-border) !important;
}

[data-testid="communityName"] {
  color: var(--warm-sunset-foreground) !important;
}

/* X AI features (2025 feature) */
[data-testid="aiSuggestion"],
[data-testid="aiResponse"] {
  background-color: var(--warm-sunset-background-secondary) !important;
  border-left: 3px solid var(--warm-sunset-primary) !important;
}

[data-testid="aiSuggestionHeader"],
[data-testid="aiResponseHeader"] {
  color: var(--warm-sunset-primary) !important;
}

/* X Spaces */
[data-testid="audioSpaceCard"] {
  background-color: var(--warm-sunset-background-secondary) !important;
  border-color: var(--warm-sunset-border) !important;
}

[data-testid="audioSpaceTitle"] {
  color: var(--warm-sunset-foreground) !important;
}

/* New quote post format (2025 feature) */
[data-testid="quotePostCard"] {
  background-color: var(--warm-sunset-tweet-background) !important;
  border: 1px solid var(--warm-sunset-tweet-border) !important;
  border-left: 3px solid var(--warm-sunset-accent) !important;
}

/* Direct messages */
[data-testid="conversation"],
[data-testid="dmDrawer"] {
  background-color: var(--warm-sunset-background) !important;
}

[data-testid="messageEntry"] {
  background-color: var(--warm-sunset-background-secondary) !important;
  border-color: var(--warm-sunset-border) !important;
}

[data-testid="messageEntry"][data-testid^="received"] {
  background-color: var(--warm-sunset-background-tertiary) !important;
}

/* Polls */
[data-testid="poll"] {
  border-color: var(--warm-sunset-border) !important;
}

[data-testid="pollOption"] {
  background-color: var(--warm-sunset-background-secondary) !important;
}

[data-testid="pollBar"] {
  background-color: var(--warm-sunset-primary) !important;
  opacity: 0.5;
}

[data-testid="pollBar"][data-is-selected="true"] {
  opacity: 1;
}

/* Trends section */
[data-testid="trend"],
[aria-label="Timeline: Trending now"] {
  background-color: var(--warm-sunset-background) !important;
}

[data-testid="trend"]:hover {
  background-color: var(--warm-sunset-tweet-hover) !important;
}

/* Who to follow */
[data-testid="UserCell"] {
  border-color: var(--warm-sunset-border) !important;
}

/* Profile page */
[data-testid="profileHeader"],
[data-testid="primaryColumn"] > div > div:first-child {
  background-color: var(--warm-sunset-background) !important;
  border-bottom-color: var(--warm-sunset-border) !important;
}

/* Tooltip (improved in 2025) */
[data-testid="Tooltip"],
[role="tooltip"] {
  background-color: var(--warm-sunset-background-tertiary) !important;
  color: var(--warm-sunset-foreground) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 8px !important;
  box-shadow: var(--warm-sunset-shadow-medium) !important;
}

/* Media (images, videos) */
[data-testid="media"] {
  border-color: var(--warm-sunset-border) !important;
  border-radius: 12px !important;
  overflow: hidden !important;
}

/* Emoji picker (improved in 2025) */
[data-testid="emojiPicker"] {
  background-color: var(--warm-sunset-background-secondary) !important;
  border-color: var(--warm-sunset-border) !important;
}

/* Scheduled tweets section */
[data-testid="scheduledTweets"] {
  background-color: var(--warm-sunset-background) !important;
  border-color: var(--warm-sunset-border) !important;
}

/* Lists */
[data-testid="listHeader"] {
  background-color: var(--warm-sunset-background) !important;
}

[data-testid="listDetails"] {
  color: var(--warm-sunset-foreground) !important;
}

/* Notifications */
[data-testid="notification"] {
  border-bottom-color: var(--warm-sunset-border) !important;
}

[data-testid="notificationIcon"] {
  color: var(--warm-sunset-primary) !important;
}

/* New conversation view (2025 feature) */
[data-testid="conversationThread"] {
  border-left: 2px solid var(--warm-sunset-border) !important;
}

[data-testid="conversationThread"]:hover {
  border-left-color: var(--warm-sunset-primary) !important;
}

/* New immersive media view (2025 feature) */
[data-testid="immersiveMediaViewer"] {
  background-color: rgba(42, 32, 35, 0.9) !important;
}

[data-testid="immersiveMediaViewer"] [data-testid="mediaPanel"] {
  background-color: transparent !important;
}

/* Redesigned profile cards (2025 feature) */
[data-testid="hoverProfileCard"] {
  background-color: var(--warm-sunset-background-secondary) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  box-shadow: var(--warm-sunset-shadow-medium) !important;
}

/* New compose tweet interface (2025 feature) */
[data-testid="tweetComposeEditor"] {
  background-color: var(--warm-sunset-background) !important;
  border-color: var(--warm-sunset-border) !important;
}

[data-testid="formatButton"] {
  color: var(--warm-sunset-foreground-secondary) !important;
}

[data-testid="formatButton"]:hover {
  color: var(--warm-sunset-primary) !important;
  background-color: var(--warm-sunset-background-tertiary) !important;
}

/* Loading indicators */
[role="progressbar"] {
  color: var(--warm-sunset-primary) !important;
}

/* Scrollbar styling */
::-webkit-scrollbar {
  width: 10px !important;
  height: 10px !important;
}

::-webkit-scrollbar-track {
  background: var(--warm-sunset-background) !important;
}

::-webkit-scrollbar-thumb {
  background: var(--warm-sunset-background-tertiary) !important;
  border-radius: 10px !important;
}

::-webkit-scrollbar-thumb:hover {
  background: var(--warm-sunset-primary) !important;
}

/* Placeholder avatars and images */
[data-testid="placeholderImage"] {
  background-color: var(--warm-sunset-background-secondary) !important;
}

/* Focus outlines */
:focus {
  outline-color: var(--warm-sunset-primary) !important;
}

/* New community navigation (2025 feature) */
[data-testid="communityNav"] {
  background-color: var(--warm-sunset-background-secondary) !important;
  border-color: var(--warm-sunset-border) !important;
}

[data-testid="communityNavItem"][aria-selected="true"] {
  background-color: var(--warm-sunset-background-tertiary) !important;
  color: var(--warm-sunset-primary) !important;
}

/* New thread reader mode (2025 feature) */
[data-testid="threadReaderMode"] {
  background-color: var(--warm-sunset-background) !important;
}

[data-testid="threadReaderControls"] {
  background-color: var(--warm-sunset-background-secondary) !important;
  border-color: var(--warm-sunset-border) !important;
}

/* Theme transition */
body, 
body *, 
main, 
article, 
[role="main"],
[role="button"],
a,
[data-testid="tweet"],
[data-testid="User-Name"] span,
nav[role="navigation"] a,
[data-testid="reply"],
[data-testid="retweet"],
[data-testid="like"] {
  transition-property: background-color, color, border-color, box-shadow;
  transition-duration: var(--warm-sunset-transition-normal);
  transition-timing-function: ease;
}
```

### Advanced Twitter/X Customization with X Enhancer (2025)

X Enhancer is a hypothetical specialized extension for Twitter/X that would provide more advanced customization options beyond what CSS alone can offer.

1. Install X Enhancer browser extension
2. Navigate to extension settings
3. Choose "Import Custom Theme"
4. Paste this JSON configuration:

```json
{
  "themeName": "Warm Sunset",
  "version": "1.0.0",
  "author": "Your Name",
  "description": "A warm and cozy theme with sunset colors",
  "themeMode": "dark",
  "colors": {
    "background": "#2A2023",
    "backgroundSecondary": "#342D34",
    "backgroundTertiary": "#403A40",
    "foreground": "#C6D0F5",
    "foregroundSecondary": "#B5A9AF",
    "primary": "#FA906E",
    "secondary": "#403A40",
    "accent": "#F5BC5E",
    "success": "#A6D18C",
    "warning": "#E5C890",
    "error": "#E78284",
    "border": "#403A40",
    "link": "#F594C1"
  },
  "layout": {
    "sidebarWidth": "280px",
    "centerTimeline": true,
    "maxTimelineWidth": "600px",
    "roundedCorners": "12px",
    "postSpacing": "12px",
    "condensedMode": false
  },
  "typography": {
    "fontFamily": "'Inter', -apple-system, BlinkMacSystemFont, sans-serif",
    "fontSize": "15px",
    "lineHeight": "1.4",
    "fontWeightNormal": "400",
    "fontWeightMedium": "500",
    "fontWeightBold": "700"
  },
  "features": {
    "enhancedReadability": true,
    "mediaEnhancements": true,
    "hideSidebarSections": ["trends", "premium", "suggestions"],
    "pinSidebar": true,
    "simpleNavigation": true,
    "hideEngagementCounts": false,
    "chronologicalTimeline": true,
    "noAutoPlay": true,
    "focusMode": false,
    "enhancedDarkMode": true,
    "customScrollbars": true
  },
  "animations": {
    "enableAnimations": true,
    "reducedMotion": false,
    "transitionSpeed": "normal"
  }
}
```

## Reddit Custom CSS

Reddit's interface has evolved since its 2023 redesign, but browser extensions still allow for the most comprehensive customization.

### Recommended Browser Extensions (2025)

1. **Stylus** - For CSS customization
   - [Chrome Web Store](https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)
   - [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/styl-us/)
   - [Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/stylus/gkgbdnmjcgjjdpdnkfcgbibpomdjbnci)

2. **Reddit Enhancement Suite (RES)** - Now with advanced theming support
   - Has evolved significantly by 2025 with expanded customization options

### Installation Instructions

1. Install the Stylus browser extension
2. Navigate to Reddit (reddit.com)
3. Click on the Stylus icon in your browser toolbar
4. Click "Write new style for: reddit.com"
5. Give your style a name like "Warm Sunset for Reddit"
6. Paste the CSS code below
7. Click "Save"

### CSS for Reddit (Dark Mode)

```css
/* Warm Sunset Theme for Reddit (2025 edition) */
/* Apply to: reddit.com */

:root {
  /* Base Colors */
  --warm-sunset-background: #2A2023;
  --warm-sunset-background-secondary: #342D34;
  --warm-sunset-background-tertiary: #403A40;
  --warm-sunset-foreground: #C6D0F5;
  --warm-sunset-foreground-secondary: #B5A9AF;
  --warm-sunset-primary: #FA906E;
  --warm-sunset-secondary: #403A40;
  --warm-sunset-accent: #F5BC5E;
  --warm-sunset-muted: #342D34;
  --warm-sunset-muted-text: #B5A9AF;
  --warm-sunset-success: #A6D18C;
  --warm-sunset-warning: #E5C890;
  --warm-sunset-error: #E78284;
  --warm-sunset-border: #403A40;
  --warm-sunset-selection: #626880;
  --warm-sunset-link: #F594C1;
  
  /* Reddit specific */
  --warm-sunset-upvote: #FA906E;
  --warm-sunset-downvote: #E78284;
  --warm-sunset-post-background: #342D34;
  --warm-sunset-post-hover: #403A40;
  --warm-sunset-comment-background: #342D34;
  --warm-sunset-comment-hover: #403A40;
  --warm-sunset-sidebar-background: #342D34;
  --warm-sunset-search-bg: #403A40;
  --warm-sunset-search-text: #C6D0F5;
  --warm-sunset-award-gold: #F5BC5E;
  --warm-sunset-award-silver: #B5A9AF;
  
  /* Shadow effects */
  --warm-sunset-shadow-small: 0 2px 5px rgba(0, 0, 0, 0.2);
  --warm-sunset-shadow-medium: 0 5px 15px rgba(0, 0, 0, 0.2);
  --warm-sunset-shadow-large: 0 10px 25px rgba(0, 0, 0, 0.2);
  
  /* Animations */
  --warm-sunset-transition-fast: 0.15s ease;
  --warm-sunset-transition-normal: 0.25s ease;
  --warm-sunset-transition-slow: 0.35s ease;
}

/* ===== GLOBAL STYLES ===== */

/* Main background and text */
body,
html {
  background-color: var(--warm-sunset-background) !important;
  color: var(--warm-sunset-foreground) !important;
}

/* Custom scrollbar */
::-webkit-scrollbar {
  width: 8px !important;
  height: 8px !important;
}

::-webkit-scrollbar-track {
  background: var(--warm-sunset-background) !important;
}

::-webkit-scrollbar-thumb {
  background: var(--warm-sunset-background-tertiary) !important;
  border-radius: 4px !important;
}

::-webkit-scrollbar-thumb:hover {
  background: var(--warm-sunset-primary) !important;
}

/* Links */
a {
  color: var(--warm-sunset-link) !important;
  transition: color var(--warm-sunset-transition-fast) !important;
}

a:hover {
  color: var(--warm-sunset-primary) !important;
  text-decoration: none !important;
}

/* Visited links */
a:visited {
  color: var(--warm-sunset-link) !important;
  opacity: 0.8 !important;
}

/* ===== HEADER ===== */

/* Main header */
header {
  background-color: var(--warm-sunset-background) !important;
  border-bottom: 1px solid var(--warm-sunset-border) !important;
}

/* Header buttons and elements */
header button,
header div[role="button"],
.reddit-header-action-menu {
  color: var(--warm-sunset-foreground) !important;
  background-color: transparent !important;
}

header button:hover,
header div[role="button"]:hover,
.reddit-header-action-menu:hover {
  background-color: var(--warm-sunset-background-secondary) !important;
}

/* Search bar */
header input[type="text"],
header input[type="search"],
.search-input {
  background-color: var(--warm-sunset-search-bg) !important;
  color: var(--warm-sunset-search-text) !important;
  border: 1px solid var(--warm-sunset-border) !important;
}

/* Reddit logo */
header a[href="/"]:first-child img,
.reddit-logo {
  filter: brightness(0) saturate(100%) invert(80%) sepia(39%) saturate(368%) hue-rotate(127deg) brightness(121%) contrast(94%) !important;
}

/* User menu */
.user-menu,
.user-dropdown {
  background-color: var(--warm-sunset-background-secondary) !important;
  border: 1px solid var(--warm-sunset-border) !important;
}

.user-menu-item,
.user-dropdown-item {
  color: var(--warm-sunset-foreground) !important;
}

.user-menu-item:hover,
.user-dropdown-item:hover {
  background-color: var(--warm-sunset-background-tertiary) !important;
}

/* ===== MAIN CONTENT ===== */

/* Main wrapper */
.main-wrapper,
.main-content,
.content-container,
main {
  background-color: var(--warm-sunset-background) !important;
}

/* Posts */
.post,
.post-container,
article,
.post-card {
  background-color: var(--warm-sunset-post-background) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 8px !important;
  margin-bottom: 10px !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

.post:hover,
.post-container:hover,
article:hover,
.post-card:hover {
  background-color: var(--warm-sunset-post-hover) !important;
  border-color: var(--warm-sunset-primary) !important;
  transform: translateY(-2px) !important;
  box-shadow: var(--warm-sunset-shadow-small) !important;
}

/* Post title */
.post-title,
.post-title a,
article h3 {
  color: var(--warm-sunset-foreground) !important;
  font-weight: 600 !important;
}

.post-title a:hover,
article h3 a:hover {
  color: var(--warm-sunset-primary) !important;
}

/* Post metadata */
.post-metadata,
.post-info,
.post-meta {
  color: var(--warm-sunset-foreground-secondary) !important;
}

/* Post content */
.post-content,
.post-body,
article .md {
  color: var(--warm-sunset-foreground) !important;
}

/* Voting buttons */
.vote-button,
.vote,
.upvote,
.downvote {
  transition: all var(--warm-sunset-transition-fast) !important;
}

.upvote,
.upvote-button,
[data-click-id="upvote"] {
  color: var(--warm-sunset-foreground-secondary) !important;
}

.upvote:hover,
.upvote-button:hover,
[data-click-id="upvote"]:hover,
.upvoted,
[data-click-id="upvote"][data-clicked="true"] {
  color: var(--warm-sunset-upvote) !important;
}

.downvote,
.downvote-button,
[data-click-id="downvote"] {
  color: var(--warm-sunset-foreground-secondary) !important;
}

.downvote:hover,
.downvote-button:hover,
[data-click-id="downvote"]:hover,
.downvoted,
[data-click-id="downvote"][data-clicked="true"] {
  color: var(--warm-sunset-downvote) !important;
}

/* Vote count */
.score,
.vote-count,
.votes {
  color: var(--warm-sunset-foreground) !important;
}

.upvoted .score,
.upvoted .vote-count,
.upvoted .votes {
  color: var(--warm-sunset-upvote) !important;
}

.downvoted .score,
.downvoted .vote-count,
.downvoted .votes {
  color: var(--warm-sunset-downvote) !important;
}

/* Comments */
.comments,
.comment-section {
  background-color: var(--warm-sunset-background) !important;
}

.comment,
.comment-container {
  background-color: var(--warm-sunset-comment-background) !important;
  border-radius: 6px !important;
  margin-bottom: 8px !important;
  padding: 8px !important;
  border-left: 2px solid var(--warm-sunset-border) !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

.comment:hover,
.comment-container:hover {
  background-color: var(--warm-sunset-comment-hover) !important;
  border-left-color: var(--warm-sunset-primary) !important;
}

/* Comment author */
.comment-author,
.author-name {
  color: var(--warm-sunset-primary) !important;
  font-weight: 600 !important;
}

/* Comment content */
.comment-body,
.comment-content,
.md {
  color: var(--warm-sunset-foreground) !important;
}

/* Comment metadata */
.comment-meta,
.comment-info {
  color: var(--warm-sunset-foreground-secondary) !important;
}

/* Nested comments */
.comment .comment,
.child .comment,
.child-comment {
  margin-left: 16px !important;
  border-left-color: var(--warm-sunset-background-tertiary) !important;
}

/* "Continue thread" link */
.continue-thread,
.load-more-comments {
  background-color: var(--warm-sunset-background-secondary) !important;
  color: var(--warm-sunset-foreground) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  padding: 8px 16px !important;
  border-radius: 4px !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

.continue-thread:hover,
.load-more-comments:hover {
  background-color: var(--warm-sunset-background-tertiary) !important;
  border-color: var(--warm-sunset-primary) !important;
}

/* ===== SIDEBAR ===== */

/* Sidebar container */
.sidebar,
.side,
aside {
  background-color: var(--warm-sunset-sidebar-background) !important;
  border-radius: 8px !important;
  border: 1px solid var(--warm-sunset-border) !important;
}

/* Sidebar elements */
.sidebar-section,
.side-section,
.community-info,
.subreddit-info {
  border-bottom: 1px solid var(--warm-sunset-border) !important;
}

/* Sidebar title */
.sidebar-title,
.side-header,
.community-name,
.subreddit-name {
  color: var(--warm-sunset-foreground) !important;
  font-weight: 600 !important;
}

/* Sidebar button (Join, etc.) */
.sidebar-button,
.subreddit-button,
.community-button,
button.join,
button.leave {
  background-color: var(--warm-sunset-primary) !important;
  color: var(--warm-sunset-background) !important;
  border: none !important;
  border-radius: 4px !important;
  padding: 6px 16px !important;
  font-weight: 600 !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

.sidebar-button:hover,
.subreddit-button:hover,
.community-button:hover,
button.join:hover,
button.leave:hover {
  background-color: var(--warm-sunset-accent) !important;
  transform: translateY(-1px) !important;
}

/* Community description */
.community-description,
.description,
.md {
  color: var(--warm-sunset-foreground) !important;
}

/* Sidebar stats */
.sidebar-stats,
.subscribers,
.stats {
  color: var(--warm-sunset-foreground-secondary) !important;
}

/* ===== SUBMIT BUTTONS ===== */

/* Create Post button */
.create-post,
.submit-button,
.create-post-button {
  background-color: var(--warm-sunset-primary) !important;
  color: var(--warm-sunset-background) !important;
  border: none !important;
  border-radius: 4px !important;
  padding: 8px 16px !important;
  font-weight: 600 !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

.create-post:hover,
.submit-button:hover,
.create-post-button:hover {
  background-color: var(--warm-sunset-accent) !important;
  transform: translateY(-1px) !important;
  box-shadow: var(--warm-sunset-shadow-small) !important;
}

/* ===== MODALS AND DIALOGS ===== */

/* Modal container */
.modal,
.dialog,
.popup {
  background-color: var(--warm-sunset-background-secondary) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 8px !important;
  box-shadow: var(--warm-sunset-shadow-medium) !important;
}

/* Modal header */
.modal-header,
.dialog-header,
.popup-header {
  border-bottom: 1px solid var(--warm-sunset-border) !important;
}

/* Modal content */
.modal-content,
.dialog-content,
.popup-content {
  color: var(--warm-sunset-foreground) !important;
}

/* Modal button */
.modal-button,
.dialog-button,
.popup-button {
  background-color: var(--warm-sunset-background-tertiary) !important;
  color: var(--warm-sunset-foreground) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 4px !important;
  padding: 6px 16px !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

.modal-button:hover,
.dialog-button:hover,
.popup-button:hover {
  background-color: var(--warm-sunset-primary) !important;
  color: var(--warm-sunset-background) !important;
  border-color: var(--warm-sunset-primary) !important;
}

/* Primary modal button */
.modal-button-primary,
.dialog-button-primary,
.popup-button-primary {
  background-color: var(--warm-sunset-primary) !important;
  color: var(--warm-sunset-background) !important;
  border: none !important;
}

.modal-button-primary:hover,
.dialog-button-primary:hover,
.popup-button-primary:hover {
  background-color: var(--warm-sunset-accent) !important;
}

/* ===== MISC COMPONENTS ===== */

/* Awards */
.award,
.award-icon,
.awarding-icon {
  transition: transform var(--warm-sunset-transition-fast) !important;
}

.award:hover,
.award-icon:hover,
.awarding-icon:hover {
  transform: scale(1.1) !important;
}

/* Gold award */
.award-gold,
.award-gold-icon {
  color: var(--warm-sunset-award-gold) !important;
}

/* Silver award */
.award-silver,
.award-silver-icon {
  color: var(--warm-sunset-award-silver) !important;
}

/* Dropdown menus */
.dropdown,
.dropdown-menu {
  background-color: var(--warm-sunset-background-secondary) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 8px !important;
  box-shadow: var(--warm-sunset-shadow-medium) !important;
}

.dropdown-item,
.dropdown-option {
  color: var(--warm-sunset-foreground) !important;
}

.dropdown-item:hover,
.dropdown-option:hover {
  background-color: var(--warm-sunset-background-tertiary) !important;
  color: var(--warm-sunset-primary) !important;
}

/* Buttons */
button,
.button {
  background-color: var(--warm-sunset-background-tertiary) !important;
  color: var(--warm-sunset-foreground) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 4px !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

button:hover,
.button:hover {
  background-color: var(--warm-sunset-primary) !important;
  color: var(--warm-sunset-background) !important;
  border-color: var(--warm-sunset-primary) !important;
}

/* Form controls */
input[type="text"],
input[type="password"],
input[type="email"],
textarea,
select {
  background-color: var(--warm-sunset-background) !important;
  color: var(--warm-sunset-foreground) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 4px !important;
}

input[type="text"]:focus,
input[type="password"]:focus,
input[type="email"]:focus,
textarea:focus,
select:focus {
  border-color: var(--warm-sunset-primary) !important;
  box-shadow: 0 0 0 2px var(--warm-sunset-primary) !important;
}

/* Code formatting */
code,
pre {
  background-color: var(--warm-sunset-background) !important;
  color: var(--warm-sunset-foreground) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 4px !important;
}

/* ===== 2025 REDDIT FEATURES ===== */

/* New community dashboard (hypothetical 2025 feature) */
.community-dashboard,
.community-hub {
  background-color: var(--warm-sunset-background-secondary) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 8px !important;
}

.dashboard-section,
.hub-section {
  border-bottom: 1px solid var(--warm-sunset-border) !important;
}

.dashboard-title,
.hub-title {
  color: var(--warm-sunset-foreground) !important;
  font-weight: 600 !important;
}

/* Improved media gallery (hypothetical 2025 feature) */
.media-gallery,
.image-gallery {
  background-color: var(--warm-sunset-background-secondary) !important;
  border-radius: 8px !important;
  padding: 12px !important;
}

.gallery-item,
.image-item {
  border-radius: 8px !important;
  overflow: hidden !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

.gallery-item:hover,
.image-item:hover {
  transform: scale(1.02) !important;
  box-shadow: var(--warm-sunset-shadow-small) !important;
}

/* New poll interface (hypothetical 2025 feature) */
.poll-container,
.poll-widget {
  background-color: var(--warm-sunset-background-secondary) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 8px !important;
  padding: 12px !important;
}

.poll-option,
.poll-choice {
  background-color: var(--warm-sunset-background-tertiary) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 4px !important;
  margin-bottom: 8px !important;
  padding: 8px 12px !important;
  position: relative !important;
  overflow: hidden !important;
}

.poll-progress,
.poll-bar {
  background-color: var(--warm-sunset-primary) !important;
  opacity: 0.3 !important;
  position: absolute !important;
  top: 0 !important;
  left: 0 !important;
  height: 100% !important;
  z-index: 0 !important;
}

.poll-option-content,
.poll-choice-content {
  position: relative !important;
  z-index: 1 !important;
  display: flex !important;
  justify-content: space-between !important;
}

.poll-percentage,
.poll-votes {
  color: var(--warm-sunset-foreground-secondary) !important;
  font-weight: 600 !important;
}

/* New community spotlight feature (hypothetical 2025 feature) */
.spotlight-container,
.featured-communities {
  background-color: var(--warm-sunset-background-secondary) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 8px !important;
  padding: 16px !important;
  margin-bottom: 16px !important;
}

.spotlight-header,
.featured-header {
  color: var(--warm-sunset-foreground) !important;
  font-weight: 600 !important;
  padding-bottom: 8px !important;
  border-bottom: 1px solid var(--warm-sunset-border) !important;
}

.spotlight-item,
.featured-item {
  padding: 8px 0 !important;
  border-bottom: 1px solid var(--warm-sunset-border) !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

.spotlight-item:hover,
.featured-item:hover {
  background-color: var(--warm-sunset-background-tertiary) !important;
  transform: translateX(4px) !important;
}

.spotlight-name,
.featured-name {
  color: var(--warm-sunset-primary) !important;
  font-weight: 600 !important;
}

.spotlight-description,
.featured-description {
  color: var(--warm-sunset-foreground-secondary) !important;
  font-size: 0.9em !important;
}

/* Redesigned user profile (hypothetical 2025 feature) */
.profile-container,
.user-profile {
  background-color: var(--warm-sunset-background) !important;
}

.profile-header,
.user-header {
  background-color: var(--warm-sunset-background-secondary) !important;
  border-bottom: 1px solid var(--warm-sunset-border) !important;
  padding: 20px !important;
}

.profile-avatar,
.user-avatar {
  border: 3px solid var(--warm-sunset-primary) !important;
  border-radius: 50% !important;
}

.profile-name,
.user-name {
  color: var(--warm-sunset-foreground) !important;
  font-weight: 700 !important;
  font-size: 1.5em !important;
}

.profile-stats,
.user-stats {
  color: var(--warm-sunset-foreground-secondary) !important;
}

.profile-tabs,
.user-tabs {
  border-bottom: 1px solid var(--warm-sunset-border) !important;
}

.profile-tab,
.user-tab {
  color: var(--warm-sunset-foreground-secondary) !important;
  padding: 12px 16px !important;
  margin-right: 8px !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

.profile-tab:hover,
.user-tab:hover {
  color: var(--warm-sunset-foreground) !important;
  background-color: var(--warm-sunset-background-tertiary) !important;
}

.profile-tab-active,
.user-tab-active,
.profile-tab[data-active="true"],
.user-tab[data-active="true"] {
  color: var(--warm-sunset-primary) !important;
  border-bottom: 3px solid var(--warm-sunset-primary) !important;
}

/* New AI assistant feature (hypothetical 2025 feature) */
.ai-assistant-container,
.reddit-ai {
  background-color: var(--warm-sunset-background-secondary) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 8px !important;
  padding: 16px !important;
  margin-bottom: 16px !important;
  border-left: 3px solid var(--warm-sunset-primary) !important;
}

.ai-assistant-header,
.reddit-ai-header {
  color: var(--warm-sunset-primary) !important;
  font-weight: 600 !important;
  display: flex !important;
  align-items: center !important;
}

.ai-assistant-icon,
.reddit-ai-icon {
  margin-right: 8px !important;
}

.ai-assistant-content,
.reddit-ai-content {
  color: var(--warm-sunset-foreground) !important;
  padding: 8px 0 !important;
}

.ai-assistant-actions,
.reddit-ai-actions {
  display: flex !important;
  gap: 8px !important;
  margin-top: 8px !important;
}

.ai-assistant-action,
.reddit-ai-action {
  background-color: var(--warm-sunset-background-tertiary) !important;
  color: var(--warm-sunset-foreground) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 4px !important;
  padding: 4px 8px !important;
  font-size: 0.8em !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

.ai-assistant-action:hover,
.reddit-ai-action:hover {
  background-color: var(--warm-sunset-primary) !important;
  color: var(--warm-sunset-background) !important;
  border-color: var(--warm-sunset-primary) !important;
}
```

## Using Reddit Enhancement Suite (RES) with Custom CSS

If you also use Reddit Enhancement Suite (which by 2025 has greatly expanded its theming capabilities), here's how to further enhance your Warm Sunset theme:

1. Install RES from your browser's extension store
2. Go to RES Settings (gear icon) > Appearance > Custom CSS
3. Add the following code:

```css
/* RES night mode specific styles for Warm Sunset */
.res-nightmode {
  --res-color-primary: var(--warm-sunset-primary);
  --res-color-secondary: var(--warm-sunset-accent);
  --res-color-background: var(--warm-sunset-background);
  --res-color-foreground: var(--warm-sunset-foreground);
  --res-color-border: var(--warm-sunset-border);
}

/* RES elements */
.RES-keyboardNav-activeElement, 
.RES-keyboardNav-activeElement .md-container {
  background-color: var(--warm-sunset-background-tertiary) !important;
  outline: 2px solid var(--warm-sunset-primary) !important;
}

/* Comment collapse button */
.res-commentBoxes .thing.comment div.entry .tagline > .expand {
  background-color: var(--warm-sunset-background-tertiary) !important;
  color: var(--warm-sunset-foreground-secondary) !important;
  border-radius: 3px !important;
  padding: 0 3px !important;
  transition: all var(--warm-sunset-transition-fast) !important;
}

.res-commentBoxes .thing.comment div.entry .tagline > .expand:hover {
  background-color: var(--warm-sunset-primary) !important;
  color: var(--warm-sunset-background) !important;
}

/* User tags */
.RESUserTag {
  background-color: var(--warm-sunset-background-tertiary) !important;
  color: var(--warm-sunset-foreground) !important;
  border: 1px solid var(--warm-sunset-border) !important;
  border-radius: 3px !important;
  padding: 0 3px !important;
}
```

4. Go to RES Settings > Appearance > Night Mode
5. Enable "Use subreddit stylesheet with night mode"
6. Set "Use night mode theme" to "Always"
