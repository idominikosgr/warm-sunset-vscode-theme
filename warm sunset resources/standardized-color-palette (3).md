# Standardized Color Palette System

## Starship Configuration

Here's your Starship prompt configuration adapted to use both light and dark themes from our color palette:

```toml
"$schema" = 'https://starship.rs/config-schema.json'

# Improved format with more logical grouping and enhanced visual hierarchy
format = """
[](color_primary)\
$os\
$username\
[](bg:color_secondary fg:color_primary)\
$directory\
[](fg:color_secondary bg:color_accent)\
$git_branch\
$git_status\
[](fg:color_accent bg:color_info)\
$nodejs\
$java\
$kotlin\
$python\
$swift\
[](fg:color_info bg:color_muted)\
$docker_context\
$xcode\
$memory_usage\
$disk_usage\
[](fg:color_muted bg:color_subtle)\
$time\
[ ](fg:color_subtle)\
$line_break$character"""

# Universal palette that works in both light and dark environments
# No need to switch between light/dark palettes
palette = 'universal'

[palettes.universal]
# Core UI
color_fg = '#384242'          # Light mode foreground
color_fg_dark = '#C6D0F5'     # Dark mode foreground
color_bg = '#FAF4F2'          # Light mode background
color_bg_dark = '#2A2023'     # Dark mode background

# Semantic colors with good contrast in both modes
color_primary = '#FA906E'     # Primary action/branding (orange)
color_secondary = '#F5BC5E'   # Secondary action (yellow/gold)
color_accent = '#5BC1BF'      # Accent (teal/cyan)
color_info = '#8CAAEF'        # Information (blue)
color_success = '#A6D18C'     # Success/completion (green)
color_warning = '#F4BC5F'     # Warning (amber)
color_error = '#E06053'       # Error (red)
color_muted = '#95726A'       # Muted elements (brown-grey)
color_subtle = '#EADBCC'      # Subtle backgrounds (beige)
color_selection = '#FBD6B9'   # Selection (peach)
color_highlight = '#F594C1'   # Highlight (pink)

# Define whether to use light or dark foreground text
# Uncomment one of these options based on your terminal background:

# For light mode terminals:
color_on_primary = '#FFFFFF'      # White text on primary color
color_on_accent = '#FFFFFF'       # White text on accent color
color_on_info = '#FFFFFF'         # White text on info color
color_on_muted = '#FFFFFF'        # White text on muted color
color_on_subtle = '#384242'       # Dark text on subtle color

# For dark mode terminals (alternative):
# color_on_primary = '#2A2023'    # Dark text on primary color
# color_on_accent = '#2A2023'     # Dark text on accent color
# color_on_info = '#2A2023'       # Dark text on info color
# color_on_muted = '#FFFFFF'      # White text on muted color
# color_on_subtle = '#FFFFFF'     # White text on subtle color

[os]
disabled = false
style = "bg:color_orange fg:color_fg0"

[os.symbols]
Windows = "󰍲"
Ubuntu = "󰕈"
Macos = "󰀵"
Linux = "󰌽"
Android = ""
Arch = "󰣇"
Debian = "󰣚"

[username]
show_always = true
style_user = "bg:color_orange fg:color_fg0"
style_root = "bg:color_orange fg:color_red"
format = '[ $user ]($style)'

[directory]
style = "fg:color_fg0 bg:color_yellow"
format = "[ $path ]($style)"
truncation_length = 3
truncation_symbol = "…/"
read_only = "󰌾"
read_only_style = "fg:color_red bg:color_yellow"

[directory.substitutions]
"Documents" = "󰈙 "
"Downloads" = " "
"Music" = "󰝚 "
"Pictures" = " "
"Movies" = "󰎁 "
"Applications" = "󰀶 "
"Desktop" = "󰲋 "
"Library" = "󱂵 "
"Developer" = "󰅨 "
"Projects" = "󱒒 "
"Dropbox" = "󰇣 "
".config" = "󰖟 "
"~" = "󰋜 "

[git_branch]
symbol = " "
style = "bg:color_aqua"
format = '[[ $symbol $branch ](fg:color_fg0 bg:color_aqua)]($style)'

[git_status]
style = "bg:color_aqua"
format = '[[($all_status$ahead_behind )](fg:color_fg0 bg:color_aqua)]($style)'
conflicted = "󰞇 "
ahead = "󰄿 ${count}"
behind = "󰄼 ${count}"
diverged = "󰡏 󰄿${ahead_count}󰄼${behind_count}"
up_to_date = "󰄬"
untracked = "󰋗 ${count}"
stashed = "󰒷 "
modified = "󰝤 ${count}"
staged = "󰈖 ${count}"
renamed = "󰑕 ${count}"
deleted = "󰮈 ${count}"

[nodejs]
symbol = " "
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[php]
symbol = " "
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[java]
symbol = " "
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[kotlin]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[python]
symbol = " "
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'
python_binary = ["python3", "python"]
detect_extensions = ["py", "ipynb"]
detect_files = ["requirements.txt", "pyproject.toml", "setup.py"]

[swift]
symbol = "󰛥 "
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'
detect_extensions = ["swift"]
detect_files = ["Package.swift"]

[docker_context]
symbol = "  "
style = "bg:color_bg3"
format = '[[ $symbol( $context) ](fg:#83a598 bg:color_bg3)]($style)'

[memory_usage]
symbol = "󰍛 "
format = '[[${symbol} $ram](fg:color_fg0 bg:color_bg3)]($style)'
style = "bg:color_bg3"
threshold = 50
disabled = false

[time]
disabled = false
time_format = "%R"
style = "bg:color_bg1"
format = '[[  $time ](fg:color_fg0 bg:color_bg1)]($style)'

[line_break]
disabled = false

[character]
disabled = false
success_symbol = '[](bold fg:color_green)'
error_symbol = '[](bold fg:color_red)'
vimcmd_symbol = '[](bold fg:color_green)'
vimcmd_replace_one_symbol = '[](bold fg:color_purple)'
vimcmd_replace_symbol = '[](bold fg:color_purple)'
vimcmd_visual_symbol = '[](bold fg:color_yellow)'

[battery]
full_symbol = "󰁹"
charging_symbol = "󰂄"
discharging_symbol = "󰂃"
disabled = false

[[battery.display]]
threshold = 30
style = "fg:color_red"
discharging_symbol = "󱃍"

# Enhanced macOS custom modules

# Xcode detection
[custom.xcode]
command = "xcode-select --print-path | xargs -I{} basename {}"
format = '[[󰛥 $output](fg:color_fg0 bg:color_bg3)]($style)'
style = "bg:color_bg3"
when = "command -v xcode-select > /dev/null 2>&1"

# Disk usage on root
[custom.disk_usage]
command = "df -h / | tail -1 | awk '{print $3 \"/\" $2 \" (\" $5 \")\"}'"
format = '[[󰨣 $output](fg:color_fg0 bg:color_bg3)]($style)'
style = "bg:color_bg3"
when = "df -h > /dev/null 2>&1"

# Apple Silicon or Intel detection
[custom.processor]
command = "sysctl -n machdep.cpu.brand_string | grep -q 'Apple' && echo '󰘚 Apple Silicon' || echo '󰌢 Intel'"
when = "sysctl -n machdep.cpu.brand_string"
style = "bg:color_bg3"
format = '[[$output](fg:color_fg0 bg:color_bg3)]($style)'
disabled = false

# Rosetta detection for Apple Silicon Macs
[custom.rosetta]
command = "ps -p $ -o comm= | xargs file | grep -q 'x86_64' && echo '󰻠 Rosetta' || echo '󰨖 Native'"
when = "sysctl -n machdep.cpu.brand_string | grep -q 'Apple'"
style = "bg:color_bg3"
format = '[[$output](fg:color_fg0 bg:color_bg3)]($style)'
disabled = true

# Shows pending software updates
[custom.macos_updates]
command = "softwareupdate -l 2>/dev/null | grep -c 'recommended'"
when = "[ $(uname) = 'Darwin' ]"
style = "bg:color_bg3"
format = '[[󰚰 $output updates](fg:color_fg0 bg:color_bg3)]($style)'
disabled = true

[custom.brew]
command = "brew --version | head -n 1 | awk '{print $2}'"
format = '[🍺 $output](fg bg)'
style = "bg"
when = "command -v brew > /dev/null 2>&1"
```

## Color System

### Light Theme

| Element | Hex | RGB | HSL |
|---------|-----|-----|-----|
| Background | #FAF4F2 | rgb(250, 244, 242) | hsl(24, 100%, 98%) |
| Foreground | #384242 | rgb(56, 66, 66) | hsl(347, 8%, 22%) |
| Primary | #FA906E | rgb(250, 144, 110) | hsl(12, 100%, 69%) |
| Secondary | #FDE6DE | rgb(253, 230, 222) | hsl(9, 100%, 96%) |
| Accent | #F5BC5E | rgb(245, 188, 94) | hsl(26, 99%, 74%) |
| Muted | #F5F1EB | rgb(245, 241, 235) | hsl(15, 100%, 96%) |
| Muted Text | #95726A | rgb(149, 114, 106) | hsl(6, 19%, 40%) |
| Success | #A6D18C | rgb(166, 209, 140) | hsl(98, 43%, 68%) |
| Warning | #F4BC5F | rgb(244, 188, 95) | hsl(38, 88%, 67%) |
| Error | #E06053 | rgb(224, 96, 83) | hsl(5, 70%, 60%) |
| Border | #EADBCC | rgb(234, 219, 204) | hsl(15, 48%, 86%) |
| Selection | #FBD6B9 | rgb(251, 214, 185) | hsl(29, 89%, 85%) |
| Link | #FA906E | rgb(250, 144, 110) | hsl(12, 100%, 69%) |

### Dark Theme

| Element | Hex | RGB | HSL |
|---------|-----|-----|-----|
| Background | #2A2023 | rgb(42, 32, 35) | hsl(340, 14%, 15%) |
| Foreground | #C6D0F5 | rgb(198, 208, 245) | hsl(221, 35%, 92%) |
| Primary | #FA906E | rgb(250, 144, 110) | hsl(12, 100%, 69%) |
| Secondary | #403A40 | rgb(64, 58, 64) | hsl(325, 9%, 25%) |
| Accent | #F5BC5E | rgb(245, 188, 94) | hsl(26, 99%, 74%) |
| Muted | #342D34 | rgb(52, 45, 52) | hsl(324, 10%, 20%) |
| Muted Text | #B5A9AF | rgb(181, 169, 175) | hsl(22, 25%, 79%) |
| Success | #A6D18C | rgb(166, 209, 140) | hsl(98, 43%, 68%) |
| Warning | #E5C890 | rgb(229, 200, 144) | hsl(38, 97%, 73%) |
| Error | #E78284 | rgb(231, 130, 132) | hsl(359, 66%, 71%) |
| Border | #403A40 | rgb(64, 58, 64) | hsl(325, 9%, 25%) |
| Selection | #626880 | rgb(98, 104, 128) | hsl(225, 17%, 44%) |
| Link | #F594C1 | rgb(245, 148, 193) | hsl(336, 86%, 77%) |

## Platform-Specific Applications

### Terminal Applications (iTerm, Terminal, etc.)

```json
// Light Theme
{
  "background": "#FAF4F2",
  "foreground": "#384242",
  "cursor": "#FA906E",
  "selection": "#FBD6B9",
  "black": "#F1EFEF",
  "red": "#E06053",
  "green": "#A6D18C",
  "yellow": "#F4BC5F",
  "blue": "#8CAAEF",
  "magenta": "#F28ABF",
  "cyan": "#5BC1BF",
  "white": "#686868",
  "brightBlack": "#A0A0A0",
  "brightRed": "#D9534F",
  "brightGreen": "#8EC78D",
  "brightYellow": "#F5BC5E",
  "brightBlue": "#7B9EF0",
  "brightMagenta": "#F2A5F2",
  "brightCyan": "#5BBFB5",
  "brightWhite": "#384242"
}

// Dark Theme
{
  "background": "#2A2023",
  "foreground": "#C6D0F5",
  "cursor": "#F2D5CF",
  "selection": "#626880",
  "black": "#2A2023",
  "red": "#E78284",
  "green": "#A6D18C",
  "yellow": "#E5C890",
  "blue": "#8CAAEF",
  "magenta": "#F4B8F4",
  "cyan": "#81C8BE",
  "white": "#B5BFE2",
  "brightBlack": "#626880",
  "brightRed": "#E67279",
  "brightGreen": "#8EC78D",
  "brightYellow": "#E5C890",
  "brightBlue": "#8CAAEF",
  "brightMagenta": "#F2A5F2",
  "brightCyan": "#81C8BE",
  "brightWhite": "#C6D0F5"
}
```

### Code Editors (VS Code, Sublime, etc.)

```jsonc
// VS Code settings.json (Light Theme)
{
  "workbench.colorCustomizations": {
    "editor.background": "#FAF4F2",
    "editor.foreground": "#384242",
    "editor.selectionBackground": "#FBD6B9",
    "editorCursor.foreground": "#FA906E",
    "activityBar.background": "#F5F1EB",
    "activityBar.foreground": "#384242",
    "sideBar.background": "#FDF7F5",
    "sideBar.foreground": "#384242",
    "statusBar.background": "#FA906E",
    "statusBar.foreground": "#FFFFFF",
    "titleBar.activeBackground": "#FDE6DE",
    "titleBar.activeForeground": "#384242"
  },
  "editor.tokenColorCustomizations": {
    "strings": "#A6D18C",
    "numbers": "#F5BC5E",
    "comments": "#95726A",
    "functions": "#8CAAEF",
    "keywords": "#F28ABF"
  }
}

// VS Code settings.json (Dark Theme)
{
  "workbench.colorCustomizations": {
    "editor.background": "#2A2023",
    "editor.foreground": "#C6D0F5",
    "editor.selectionBackground": "#626880",
    "editorCursor.foreground": "#F2D5CF",
    "activityBar.background": "#342D34",
    "activityBar.foreground": "#C6D0F5",
    "sideBar.background": "#342D34",
    "sideBar.foreground": "#C6D0F5",
    "statusBar.background": "#FA906E",
    "statusBar.foreground": "#FFFFFF",
    "titleBar.activeBackground": "#403A40",
    "titleBar.activeForeground": "#C6D0F5"
  },
  "editor.tokenColorCustomizations": {
    "strings": "#A6D18C",
    "numbers": "#F5BC5E",
    "comments": "#B5A9AF",
    "functions": "#8CAAEF",
    "keywords": "#F4B8F4"
  }
}
```

### CSS Variables (for websites)

```css
/* Light theme */
:root {
  --background: #FAF4F2;
  --foreground: #384242;
  --primary: #FA906E;
  --primary-foreground: #FFFFFF;
  --secondary: #FDE6DE;
  --secondary-foreground: #79514A;
  --muted: #F5F1EB;
  --muted-foreground: #95726A;
  --accent: #F5BC5E;
  --accent-foreground: #384242;
  --destructive: #E06053;
  --destructive-foreground: #FFFFFF;
  --border: #EADBCC;
  --input: #EADBCC;
  --ring: #FA906E;
  
  --success: #A6D18C;
  --warning: #F4BC5F;
  --error: #E06053;
  
  --selection: #FBD6B9;
  --selection-foreground: #384242;
  --link: #FA906E;
  
  --radius: 0.625rem;
  --font-sans: Montserrat, sans-serif;
  --font-serif: Merriweather, serif;
  --font-mono: Ubuntu Mono, monospace;
}

/* Dark theme */
.dark {
  --background: #2A2023;
  --foreground: #C6D0F5;
  --primary: #FA906E;
  --primary-foreground: #FFFFFF;
  --secondary: #403A40;
  --secondary-foreground: #C6D0F5;
  --muted: #342D34;
  --muted-foreground: #B5A9AF;
  --accent: #F5BC5E;
  --accent-foreground: #2A2023;
  --destructive: #E78284;
  --destructive-foreground: #FFFFFF;
  --border: #403A40;
  --input: #403A40;
  --ring: #FA906E;
  
  --success: #A6D18C;
  --warning: #E5C890;
  --error: #E78284;
  
  --selection: #626880;
  --selection-foreground: #C6D0F5;
  --link: #F594C1;
}
```

### SCSS Variables (for broader design systems)

```scss
// _colors.scss
// Light Theme
$light-theme: (
  "background": #FAF4F2,
  "foreground": #384242,
  "primary": #FA906E,
  "primary-foreground": #FFFFFF,
  "secondary": #FDE6DE,
  "secondary-foreground": #79514A,
  "muted": #F5F1EB,
  "muted-foreground": #95726A,
  "accent": #F5BC5E,
  "accent-foreground": #384242,
  "destructive": #E06053,
  "destructive-foreground": #FFFFFF,
  "border": #EADBCC,
  "input": #EADBCC,
  "ring": #FA906E,
  "success": #A6D18C,
  "warning": #F4BC5F,
  "error": #E06053,
  "selection": #FBD6B9,
  "selection-foreground": #384242,
  "link": #FA906E
);

// Dark Theme
$dark-theme: (
  "background": #2A2023,
  "foreground": #C6D0F5,
  "primary": #FA906E,
  "primary-foreground": #FFFFFF,
  "secondary": #403A40,
  "secondary-foreground": #C6D0F5,
  "muted": #342D34,
  "muted-foreground": #B5A9AF,
  "accent": #F5BC5E,
  "accent-foreground": #2A2023,
  "destructive": #E78284,
  "destructive-foreground": #FFFFFF,
  "border": #403A40,
  "input": #403A40,
  "ring": #FA906E,
  "success": #A6D18C,
  "warning": #E5C890,
  "error": #E78284,
  "selection": #626880,
  "selection-foreground": #C6D0F5,
  "link": #F594C1
);
```

## Implementation Tips

1. **For Terminals**: Most terminals accept import/export of color themes in JSON or XML format. Use the terminal-specific structure above.

2. **For IDEs/Code Editors**: Most editors have theme plugins or allow direct customization through settings files. Use the provided VS Code example as a starting point.

3. **For Websites**: 
   - Use the CSS variables for consistent theming
   - Implement dark mode toggle with a simple class change on your `<html>` or `<body>` element
   - Use `prefers-color-scheme` media query for automatic theme detection

4. **For Design Systems (Figma, Sketch, etc.)**:
   - Create color style libraries using the hex values provided
   - Use consistent naming conventions matching the element names

5. **For WordPress**:
   - Implement these colors through your theme's customizer
   - Use CSS variables in your theme's stylesheet

6. **For Canva and other design tools**:
   - Create a brand kit with these colors
   - Save hex codes for quick reference
