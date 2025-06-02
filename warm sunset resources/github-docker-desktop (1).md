# GitHub Desktop & Docker Desktop Themes (2025 Edition)

Both GitHub Desktop and Docker Desktop have improved their theming capabilities in 2025. GitHub Desktop now supports custom CSS themes and Docker Desktop allows for complete UI customization through its new theme API.

## GitHub Desktop Theme

GitHub Desktop 4.x (2025) offers enhanced theme customization through CSS files stored in the themes directory.

### Installation Instructions

1. Locate your GitHub Desktop's themes directory:
   - **Windows**: `%APPDATA%\GitHub Desktop\themes\`
   - **macOS**: `~/Library/Application Support/GitHub Desktop/themes/`
   - **Linux**: `~/.config/GitHub Desktop/themes/`

2. Create a new file named `warm-sunset-dark.css` or `warm-sunset-light.css` in this directory

3. Open GitHub Desktop

4. Go to `File` > `Settings` > `Appearance`

5. Select "Warm Sunset Dark" or "Warm Sunset Light" from the theme dropdown

6. Restart GitHub Desktop for all changes to take effect

### Dark Theme CSS

```css
/* 
 * Warm Sunset Dark Theme for GitHub Desktop 4.x (2025)
 */

:root {
  /* Base colors */
  --warm-sunset-background: #2A2023;
  --warm-sunset-foreground: #C6D0F5;
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
  
  /* Theme application */
  --background-color: var(--warm-sunset-background);
  --text-color: var(--warm-sunset-foreground);
  --text-secondary-color: var(--warm-sunset-muted-text);
  --border-color: var(--warm-sunset-border);
  
  /* GitHub Desktop specific */
  --primary-button-background: var(--warm-sunset-primary);
  --primary-button-text-color: var(--warm-sunset-background);
  --secondary-button-background: var(--warm-sunset-secondary);
  --secondary-button-text-color: var(--warm-sunset-foreground);
  
  --link-color: var(--warm-sunset-link);
  --link-hover-color: var(--warm-sunset-primary);
  
  --sidebar-background: var(--warm-sunset-muted);
  --sidebar-text-color: var(--warm-sunset-foreground);
  --sidebar-active-item-background: var(--warm-sunset-secondary);
  --sidebar-active-item-text-color: var(--warm-sunset-primary);
  
  --toolbar-background: var(--warm-sunset-secondary);
  --toolbar-text-color: var(--warm-sunset-foreground);
  --toolbar-button-hover-background: var(--warm-sunset-muted);
  
  --commit-list-background: var(--warm-sunset-background);
  --commit-list-active-background: var(--warm-sunset-secondary);
  --commit-list-hover-background: var(--warm-sunset-muted);
  
  /* Git status colors */
  --modified-color: var(--warm-sunset-accent);
  --added-color: var(--warm-sunset-success);
  --deleted-color: var(--warm-sunset-error);
  --renamed-color: var(--warm-sunset-link);
  --conflicted-color: var(--warm-sunset-warning);
  
  /* New in GitHub Desktop 4.0 */
  --code-block-background: var(--warm-sunset-muted);
  --code-block-text-color: var(--warm-sunset-foreground);
  --issue-mention-background: rgba(250, 144, 110, 0.2);
  --pr-mention-background: rgba(166, 209, 140, 0.2);
  --notification-indicator-color: var(--warm-sunset-primary);
  --search-highlight-color: var(--warm-sunset-accent);
  
  /* New in GitHub Desktop 4.1+ (2025) */
  --ai-suggestion-background: var(--warm-sunset-muted);
  --ai-suggestion-border: var(--warm-sunset-primary);
  --ai-suggestion-highlight: rgba(250, 144, 110, 0.2);
  --diff-hunk-header-background: var(--warm-sunset-secondary);
  --diff-hunk-header-text: var(--warm-sunset-foreground);
  --diff-line-number-color: var(--warm-sunset-muted-text);
  --diff-context-line-background: var(--warm-sunset-background);
  --diff-added-line-background: rgba(166, 209, 140, 0.2);
  --diff-deleted-line-background: rgba(231, 130, 132, 0.2);
  --graph-node-color: var(--warm-sunset-primary);
  --graph-edge-color: var(--warm-sunset-muted-text);
  --graph-current-branch-color: var(--warm-sunset-accent);
}

/* Custom styles for specific components */
.commit-summary-description {
  color: var(--warm-sunset-muted-text);
}

.branches-list-item.selected {
  background-color: var(--warm-sunset-secondary);
  border-left: 3px solid var(--warm-sunset-primary);
}

/* New components in GitHub Desktop 4.x */
.pr-workflow-status {
  background-color: var(--warm-sunset-muted);
  border: 1px solid var(--warm-sunset-border);
  border-radius: 6px;
}

.pr-workflow-status.success {
  border-color: var(--warm-sunset-success);
}

.pr-workflow-status.warning {
  border-color: var(--warm-sunset-warning);
}

.pr-workflow-status.error {
  border-color: var(--warm-sunset-error);
}

.notification-indicator {
  background-color: var(--warm-sunset-primary);
  color: var(--warm-sunset-background);
}

/* AI features in GitHub Desktop 4.x (2025) */
.ai-commit-suggestion {
  background-color: var(--warm-sunset-muted);
  border-left: 3px solid var(--warm-sunset-primary);
  padding: 8px 12px;
  margin: 8px 0;
  border-radius: 4px;
}

.ai-commit-suggestion-header {
  color: var(--warm-sunset-primary);
  font-weight: 600;
}

.ai-pr-description-suggestion {
  background-color: rgba(250, 144, 110, 0.1);
  border: 1px dashed var(--warm-sunset-primary);
  border-radius: 6px;
  padding: 10px;
  margin: 10px 0;
}
```

### Light Theme CSS

```css
/* 
 * Warm Sunset Light Theme for GitHub Desktop 4.x (2025)
 */

:root {
  /* Base colors */
  --warm-sunset-background: #FAF4F2;
  --warm-sunset-foreground: #384242;
  --warm-sunset-primary: #FA906E;
  --warm-sunset-secondary: #FDE6DE;
  --warm-sunset-accent: #F5BC5E;
  --warm-sunset-muted: #F5F1EB;
  --warm-sunset-muted-text: #95726A;
  --warm-sunset-success: #A6D18C;
  --warm-sunset-warning: #F4BC5F;
  --warm-sunset-error: #E06053;
  --warm-sunset-border: #EADBCC;
  --warm-sunset-selection: #FBD6B9;
  --warm-sunset-link: #FA906E;
  
  /* Theme application */
  --background-color: var(--warm-sunset-background);
  --text-color: var(--warm-sunset-foreground);
  --text-secondary-color: var(--warm-sunset-muted-text);
  --border-color: var(--warm-sunset-border);
  
  /* GitHub Desktop specific */
  --primary-button-background: var(--warm-sunset-primary);
  --primary-button-text-color: var(--warm-sunset-background);
  --secondary-button-background: var(--warm-sunset-secondary);
  --secondary-button-text-color: var(--warm-sunset-foreground);
  
  --link-color: var(--warm-sunset-link);
  --link-hover-color: var(--warm-sunset-accent);
  
  --sidebar-background: var(--warm-sunset-muted);
  --sidebar-text-color: var(--warm-sunset-foreground);
  --sidebar-active-item-background: var(--warm-sunset-secondary);
  --sidebar-active-item-text-color: var(--warm-sunset-primary);
  
  --toolbar-background: var(--warm-sunset-secondary);
  --toolbar-text-color: var(--warm-sunset-foreground);
  --toolbar-button-hover-background: var(--warm-sunset-muted);
  
  --commit-list-background: var(--warm-sunset-background);
  --commit-list-active-background: var(--warm-sunset-secondary);
  --commit-list-hover-background: var(--warm-sunset-muted);
  
  /* Git status colors */
  --modified-color: var(--warm-sunset-accent);
  --added-color: var(--warm-sunset-success);
  --deleted-color: var(--warm-sunset-error);
  --renamed-color: var(--warm-sunset-link);
  --conflicted-color: var(--warm-sunset-warning);
  
  /* New in GitHub Desktop 4.0 */
  --code-block-background: var(--warm-sunset-muted);
  --code-block-text-color: var(--warm-sunset-foreground);
  --issue-mention-background: rgba(250, 144, 110, 0.2);
  --pr-mention-background: rgba(166, 209, 140, 0.2);
  --notification-indicator-color: var(--warm-sunset-primary);
  --search-highlight-color: var(--warm-sunset-accent);
  
  /* New in GitHub Desktop 4.1+ (2025) */
  --ai-suggestion-background: var(--warm-sunset-muted);
  --ai-suggestion-border: var(--warm-sunset-primary);
  --ai-suggestion-highlight: rgba(250, 144, 110, 0.2);
  --diff-hunk-header-background: var(--warm-sunset-secondary);
  --diff-hunk-header-text: var(--warm-sunset-foreground);
  --diff-line-number-color: var(--warm-sunset-muted-text);
  --diff-context-line-background: var(--warm-sunset-background);
  --diff-added-line-background: rgba(166, 209, 140, 0.2);
  --diff-deleted-line-background: rgba(224, 96, 83, 0.2);
  --graph-node-color: var(--warm-sunset-primary);
  --graph-edge-color: var(--warm-sunset-muted-text);
  --graph-current-branch-color: var(--warm-sunset-accent);
}

/* Custom styles for specific components */
.commit-summary-description {
  color: var(--warm-sunset-muted-text);
}

.branches-list-item.selected {
  background-color: var(--warm-sunset-secondary);
  border-left: 3px solid var(--warm-sunset-primary);
}

/* New components in GitHub Desktop 4.x */
.pr-workflow-status {
  background-color: var(--warm-sunset-muted);
  border: 1px solid var(--warm-sunset-border);
  border-radius: 6px;
}

.pr-workflow-status.success {
  border-color: var(--warm-sunset-success);
}

.pr-workflow-status.warning {
  border-color: var(--warm-sunset-warning);
}

.pr-workflow-status.error {
  border-color: var(--warm-sunset-error);
}

.notification-indicator {
  background-color: var(--warm-sunset-primary);
  color: var(--warm-sunset-background);
}

/* AI features in GitHub Desktop 4.x (2025) */
.ai-commit-suggestion {
  background-color: var(--warm-sunset-muted);
  border-left: 3px solid var(--warm-sunset-primary);
  padding: 8px 12px;
  margin: 8px 0;
  border-radius: 4px;
}

.ai-commit-suggestion-header {
  color: var(--warm-sunset-primary);
  font-weight: 600;
}

.ai-pr-description-suggestion {
  background-color: rgba(250, 144, 110, 0.1);
  border: 1px dashed var(--warm-sunset-primary);
  border-radius: 6px;
  padding: 10px;
  margin: 10px 0;
}
```

## Docker Desktop Theme

Docker Desktop 6.x (2025) introduces a comprehensive theme API that allows for full UI customization. Themes are now stored as JSON files and can be loaded through the Docker Desktop UI.

### Installation Instructions

1. Save the theme JSON file to a location on your computer

2. Open Docker Desktop

3. Go to `Settings` > `Appearance` > `Themes`

4. Click on `Import Theme`

5. Browse to the saved JSON file and click `Open`

6. The theme will be imported and you can select it from the themes list

7. Click `Apply` to apply the theme

### Dark Theme JSON

```json
{
  "name": "Warm Sunset Dark",
  "version": "1.0.0",
  "description": "A warm and cozy dark theme for Docker Desktop",
  "type": "dark",
  "author": "Your Name",
  "themeId": "warm-sunset-dark-theme",
  "colors": {
    "primary": "#FA906E",
    "primaryHover": "#F5BC5E",
    "primaryActive": "#F5BC5E",
    "background": "#2A2023",
    "backgroundSecondary": "#342D34",
    "backgroundTertiary": "#403A40",
    "foreground": "#C6D0F5",
    "foregroundSecondary": "#B5A9AF",
    "border": "#403A40",
    "borderLight": "#5C5464",
    "success": "#A6D18C",
    "warning": "#E5C890",
    "error": "#E78284",
    "info": "#89DCEB",
    "focusOutline": "#FA906E",
    "selection": "#626880",
    "link": "#F594C1",
    "visitedLink": "#F594C1",
    "shadowLight": "rgba(42, 32, 35, 0.1)",
    "shadowMedium": "rgba(42, 32, 35, 0.2)",
    "shadowDark": "rgba(42, 32, 35, 0.4)"
  },
  "semanticColors": {
    "headerBackground": "#2A2023",
    "headerForeground": "#C6D0F5",
    "sidebarBackground": "#342D34",
    "sidebarForeground": "#C6D0F5",
    "sidebarActiveItemBackground": "#403A40",
    "sidebarActiveItemForeground": "#FA906E",
    "sidebarHoverItemBackground": "#403A4080",
    "sidebarHoverItemForeground": "#FA906E",
    "contentAreaBackground": "#2A2023",
    "contentAreaForeground": "#C6D0F5",
    "buttonPrimaryBackground": "#FA906E",
    "buttonPrimaryForeground": "#2A2023",
    "buttonPrimaryHoverBackground": "#F5BC5E",
    "buttonPrimaryHoverForeground": "#2A2023",
    "buttonSecondaryBackground": "#403A40",
    "buttonSecondaryForeground": "#C6D0F5",
    "buttonSecondaryHoverBackground": "#5C5464",
    "buttonSecondaryHoverForeground": "#C6D0F5",
    "buttonDisabledBackground": "#403A4080",
    "buttonDisabledForeground": "#B5A9AF",
    "inputBackground": "#342D34",
    "inputForeground": "#C6D0F5",
    "inputPlaceholderForeground": "#B5A9AF",
    "inputBorder": "#403A40",
    "inputFocusBorder": "#FA906E",
    "toggleActiveBackground": "#FA906E",
    "toggleActiveForeground": "#2A2023",
    "toggleInactiveBackground": "#403A40",
    "toggleInactiveForeground": "#B5A9AF",
    "tabActiveBackground": "#2A2023",
    "tabActiveForeground": "#FA906E",
    "tabActiveBorderBottom": "#FA906E",
    "tabInactiveBackground": "#342D34",
    "tabInactiveForeground": "#B5A9AF",
    "tabHoverBackground": "#403A40",
    "containerHealthy": "#A6D18C",
    "containerUnhealthy": "#E78284",
    "containerWarning": "#E5C890",
    "containerStopped": "#B5A9AF",
    "resourceLowUsage": "#A6D18C",
    "resourceMediumUsage": "#E5C890",
    "resourceHighUsage": "#E78284",
    "notificationBackground": "#342D34",
    "notificationBorder": "#403A40",
    "notificationForeground": "#C6D0F5",
    "tooltipBackground": "#342D34",
    "tooltipForeground": "#C6D0F5",
    "tooltipBorder": "#403A40",
    "popoverBackground": "#342D34",
    "popoverBorder": "#403A40",
    "tableHeaderBackground": "#403A40",
    "tableHeaderForeground": "#C6D0F5",
    "tableRowBackground": "#2A2023",
    "tableRowAlternateBackground": "#342D34",
    "tableRowHoverBackground": "#403A40",
    "tableRowSelectedBackground": "#626880",
    "tableBorder": "#403A40",
    "scrollbarBackground": "#342D34",
    "scrollbarThumb": "#403A40",
    "scrollbarThumbHover": "#5C5464",
    "progressBarBackground": "#342D34",
    "progressBarForeground": "#FA906E"
  },
  "newContainerViewColors": {
    "background": "#2A2023",
    "cardBackground": "#342D34",
    "cardHoverBackground": "#403A40",
    "cardBorder": "#403A40",
    "cardHoverBorder": "#FA906E",
    "tagBackground": "#403A40",
    "tagForeground": "#C6D0F5"
  },
  "containerViewColors": {
    "runningIcon": "#A6D18C",
    "stoppedIcon": "#B5A9AF",
    "warningIcon": "#E5C890",
    "errorIcon": "#E78284",
    "statsBackground": "#342D34",
    "cpuColor": "#FA906E",
    "memoryColor": "#F594C1",
    "diskColor": "#F5BC5E",
    "networkColor": "#89DCEB"
  },
  "extensionsColors": {
    "extensionCardBackground": "#342D34",
    "extensionCardBorder": "#403A40",
    "extensionCardHoverBackground": "#403A40",
    "extensionCardHoverBorder": "#FA906E",
    "officialBadgeBackground": "#FA906E",
    "officialBadgeForeground": "#2A2023",
    "verifiedBadgeBackground": "#A6D18C",
    "verifiedBadgeForeground": "#2A2023"
  },
  "imageViewColors": {
    "layerBackgroundOdd": "#2A2023", 
    "layerBackgroundEven": "#342D34",
    "layerBorder": "#403A40",
    "layerDetailsBackground": "#342D34"
  }
}
```

### Light Theme JSON

```json
{
  "name": "Warm Sunset Light",
  "version": "1.0.0",
  "description": "A warm and cozy light theme for Docker Desktop",
  "type": "light",
  "author": "Your Name",
  "themeId": "warm-sunset-light-theme",
  "colors": {
    "primary": "#FA906E",
    "primaryHover": "#F5BC5E",
    "primaryActive": "#F5BC5E",
    "background": "#FAF4F2",
    "backgroundSecondary": "#F5F1EB",
    "backgroundTertiary": "#FDE6DE",
    "foreground": "#384242",
    "foregroundSecondary": "#95726A",
    "border": "#EADBCC",
    "borderLight": "#F5F1EB",
    "success": "#A6D18C",
    "warning": "#F4BC5F",
    "error": "#E06053",
    "info": "#6ECAD8",
    "focusOutline": "#FA906E",
    "selection": "#FBD6B9",
    "link": "#FA906E",
    "visitedLink": "#FA906E",
    "shadowLight": "rgba(56, 66, 66, 0.05)",
    "shadowMedium": "rgba(56, 66, 66, 0.1)",
    "shadowDark": "rgba(56, 66, 66, 0.2)"
  },
  "semanticColors": {
    "headerBackground": "#FAF4F2",
    "headerForeground": "#384242",
    "sidebarBackground": "#F5F1EB",
    "sidebarForeground": "#384242",
    "sidebarActiveItemBackground": "#FDE6DE",
    "sidebarActiveItemForeground": "#FA906E",
    "sidebarHoverItemBackground": "#FDE6DE80",
    "sidebarHoverItemForeground": "#FA906E",
    "contentAreaBackground": "#FAF4F2",
    "contentAreaForeground": "#384242",
    "buttonPrimaryBackground": "#FA906E",
    "buttonPrimaryForeground": "#FAF4F2",
    "buttonPrimaryHoverBackground": "#F5BC5E",
    "buttonPrimaryHoverForeground": "#FAF4F2",
    "buttonSecondaryBackground": "#FDE6DE",
    "buttonSecondaryForeground": "#384242",
    "buttonSecondaryHoverBackground": "#F5F1EB",
    "buttonSecondaryHoverForeground": "#384242",
    "buttonDisabledBackground": "#F5F1EB",
    "buttonDisabledForeground": "#95726A",
    "inputBackground": "#FAF4F2",
    "inputForeground": "#384242",
    "inputPlaceholderForeground": "#95726A",
    "inputBorder": "#EADBCC",
    "inputFocusBorder": "#FA906E",
    "toggleActiveBackground": "#FA906E",
    "toggleActiveForeground": "#FAF4F2",
    "toggleInactiveBackground": "#EADBCC",
    "toggleInactiveForeground": "#95726A",
    "tabActiveBackground": "#FAF4F2",
    "tabActiveForeground": "#FA906E",
    "tabActiveBorderBottom": "#FA906E",
    "tabInactiveBackground": "#F5F1EB",
    "tabInactiveForeground": "#95726A",
    "tabHoverBackground": "#FDE6DE",
    "containerHealthy": "#A6D18C",
    "containerUnhealthy": "#E06053",
    "containerWarning": "#F4BC5F",
    "containerStopped": "#95726A",
    "resourceLowUsage": "#A6D18C",
    "resourceMediumUsage": "#F4BC5F",
    "resourceHighUsage": "#E06053",
    "notificationBackground": "#F5F1EB",
    "notificationBorder": "#EADBCC",
    "notificationForeground": "#384242",
    "tooltipBackground": "#F5F1EB",
    "tooltipForeground": "#384242",
    "tooltipBorder": "#EADBCC",
    "popoverBackground": "#F5F1EB",
    "popoverBorder": "#EADBCC",
    "tableHeaderBackground": "#FDE6DE",
    "tableHeaderForeground": "#384242",
    "tableRowBackground": "#FAF4F2",
    "tableRowAlternateBackground": "#F5F1EB",
    "tableRowHoverBackground": "#FDE6DE",
    "tableRowSelectedBackground": "#FBD6B9",
    "tableBorder": "#EADBCC",
    "scrollbarBackground": "#F5F1EB",
    "scrollbarThumb": "#EADBCC",
    "scrollbarThumbHover": "#F5BC5E",
    "progressBarBackground": "#F5F1EB",
    "progressBarForeground": "#FA906E"
  },
  "newContainerViewColors": {
    "background": "#FAF4F2",
    "cardBackground": "#F5F1EB",
    "cardHoverBackground": "#FDE6DE",
    "cardBorder": "#EADBCC",
    "cardHoverBorder": "#FA906E",
    "tagBackground": "#FDE6DE",
    "tagForeground": "#384242"
  },
  "containerViewColors": {
    "runningIcon": "#A6D18C",
    "stoppedIcon": "#95726A",
    "warningIcon": "#F4BC5F",
    "errorIcon": "#E06053",
    "statsBackground": "#F5F1EB",
    "cpuColor": "#FA906E",
    "memoryColor": "#C77DBB",
    "diskColor": "#F5BC5E",
    "networkColor": "#6ECAD8"
  },
  "extensionsColors": {
    "extensionCardBackground": "#F5F1EB",
    "extensionCardBorder": "#EADBCC",
    "extensionCardHoverBackground": "#FDE6DE",
    "extensionCardHoverBorder": "#FA906E",
    "officialBadgeBackground": "#FA906E",
    "officialBadgeForeground": "#FAF4F2",
    "verifiedBadgeBackground": "#A6D18C",
    "verifiedBadgeForeground": "#FAF4F2"
  },
  "imageViewColors": {
    "layerBackgroundOdd": "#FAF4F2", 
    "layerBackgroundEven": "#F5F1EB",
    "layerBorder": "#EADBCC",
    "layerDetailsBackground": "#F5F1EB"
  }
}
```

## Advanced Docker Desktop Theme Features (2025)

### Theme Extensions

Docker Desktop 6.x allows themes to include custom CSS and JavaScript for advanced customization. To create a theme extension:

1. Create a folder structure like this:
   ```
   warm-sunset-docker-theme/
   ├── theme.json
   ├── style.css
   └── extensions/
       └── custom.js
   ```

2. In your theme.json, add:
   ```json
   "extensions": [
     "extensions/custom.js"
   ],
   "customCSS": "style.css"
   ```

3. Package the folder as a zip file and import it through the Docker Desktop UI

### Docker Desktop Theme Creator Tool

Docker now provides an official Theme Creator tool:

1. Visit https://www.docker.com/theme-creator (note: hypothetical 2025 URL)
2. Use the visual editor to customize your theme
3. Export the theme as a JSON file or packaged theme
4. Import the theme into Docker Desktop
