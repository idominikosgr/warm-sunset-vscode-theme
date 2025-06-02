# Windows Terminal Theme (2025 Edition)

Windows Terminal has become even more customizable in 2025, supporting more granular theme options including transparency effects and rounded corners. Here are the configurations for both light and dark themes.

## Installation Instructions

1. Open Windows Terminal
2. Press `Ctrl+,` to open the Settings UI
3. Click on "Add a new theme" in the Themes section
4. Paste the JSON configuration for your preferred theme
5. Click "Save"
6. To apply the theme, go to your profile settings and select "Warm Sunset Light" or "Warm Sunset Dark" from the theme dropdown

## Dark Theme Configuration

```json
{
    "name": "Warm Sunset Dark",
    "cursorColor": "#FA906E",
    "cursorShape": "bar",
    "selectionBackground": "#626880",
    "background": "#2A2023",
    "foreground": "#C6D0F5",
    "black": "#2A2023",
    "brightBlack": "#B5A9AF",
    "red": "#E78284",
    "brightRed": "#E78284",
    "green": "#A6D18C",
    "brightGreen": "#A6D18C",
    "yellow": "#E5C890",
    "brightYellow": "#F5BC5E",
    "blue": "#8CAAEE",
    "brightBlue": "#8CAAEE",
    "purple": "#F594C1",
    "brightPurple": "#F594C1",
    "cyan": "#89DCEB",
    "brightCyan": "#89DCEB",
    "white": "#C6D0F5",
    "brightWhite": "#C6D0F5",
    
    // New 2025 features
    "tabBackground": "#342D34",
    "tabActiveBackground": "#403A40",
    "tabActiveForeground": "#FA906E",
    "tabInactiveForeground": "#B5A9AF",
    "tabBarBackground": "#2A2023",
    "glassEffect": "acrylic", // Available in Windows 11 2025+
    "opacity": 95,
    "cornerRadius": 8,
    "accentColor": "#FA906E",
    "accentColorHover": "#F5BC5E",
    "enableCommandPaletteTheme": true,
    "commandPaletteBackground": "#342D34",
    "commandPaletteForeground": "#C6D0F5",
    "commandPaletteSelectionBackground": "#403A40",
    "commandPaletteSelectionForeground": "#FA906E"
}
```

## Light Theme Configuration

```json
{
    "name": "Warm Sunset Light",
    "cursorColor": "#FA906E",
    "cursorShape": "bar",
    "selectionBackground": "#FBD6B9",
    "background": "#FAF4F2",
    "foreground": "#384242",
    "black": "#384242",
    "brightBlack": "#95726A",
    "red": "#E06053",
    "brightRed": "#E06053",
    "green": "#A6D18C",
    "brightGreen": "#A6D18C",
    "yellow": "#F4BC5F",
    "brightYellow": "#F5BC5E",
    "blue": "#7B90D4",
    "brightBlue": "#7B90D4",
    "purple": "#C77DBB",
    "brightPurple": "#C77DBB",
    "cyan": "#6ECAD8",
    "brightCyan": "#6ECAD8",
    "white": "#F5F1EB",
    "brightWhite": "#FAF4F2",
    
    // New 2025 features
    "tabBackground": "#F5F1EB",
    "tabActiveBackground": "#FAF4F2",
    "tabActiveForeground": "#FA906E",
    "tabInactiveForeground": "#95726A",
    "tabBarBackground": "#F5F1EB",
    "glassEffect": "acrylic", // Available in Windows 11 2025+
    "opacity": 95,
    "cornerRadius": 8,
    "accentColor": "#FA906E",
    "accentColorHover": "#F5BC5E",
    "enableCommandPaletteTheme": true,
    "commandPaletteBackground": "#F5F1EB",
    "commandPaletteForeground": "#384242",
    "commandPaletteSelectionBackground": "#FDE6DE",
    "commandPaletteSelectionForeground": "#FA906E"
}
```

## Advanced Usage (2025 Features)

### Dynamic Time-Based Theme Switching

Windows Terminal now supports automatic theme switching based on time of day:

```json
"themeSettings": {
    "enableTimeBasedThemes": true,
    "morningTheme": "Warm Sunset Light",
    "eveningTheme": "Warm Sunset Dark",
    "morningHour": 6,
    "eveningHour": 18
}
```

### Per-Tab Theming

You can now set different themes for different tabs:

```json
"profiles": {
    "defaults": {
        "theme": "Warm Sunset Dark"
    },
    "list": [
        {
            "name": "PowerShell",
            "theme": "Warm Sunset Dark"
        },
        {
            "name": "Command Prompt",
            "theme": "Warm Sunset Light"
        }
    ]
}
```
