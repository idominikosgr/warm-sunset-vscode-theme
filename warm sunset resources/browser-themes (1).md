# Web Browser Themes - Chrome, Edge, Firefox (2025 Edition)

Major browsers have enhanced their theme capabilities in 2025, offering more customization options and better integration with operating systems. Here's how to create and apply Warm Sunset themes for each browser.

## Google Chrome Theme

Chrome's theming system has been significantly improved in version 135+ (2025), allowing for more UI elements to be themed and supporting both light and dark modes.

### Installation Instructions

#### Method 1: Chrome Web Store (Recommended)

1. Create a Chrome theme package using the instructions below
2. Create a Chrome Developer account if you don't have one
3. Upload your theme to the Chrome Web Store
4. Install your published theme from the Chrome Web Store

#### Method 2: Developer Mode (Local Installation)

1. Create a folder for your theme
2. Create the required files as described below
3. Go to `chrome://extensions/`
4. Enable "Developer mode" in the top-right corner
5. Click "Load unpacked" and select your theme folder
6. The theme will be instantly applied

### Chrome Theme Manifest (manifest.json)

```json
{
  "name": "Warm Sunset",
  "version": "1.0",
  "description": "A warm and cozy theme with sunset colors",
  "manifest_version": 3,
  "theme": {
    "colors": {
      "frame": "#2A2023",
      "frame_inactive": "#342D34",
      "frame_incognito": "#1A181A",
      "frame_incognito_inactive": "#221F22",
      "toolbar": "#2A2023",
      "tab_text": "#C6D0F5",
      "tab_background_text": "#B5A9AF",
      "bookmark_text": "#C6D0F5",
      "ntp_background": "#2A2023",
      "ntp_text": "#C6D0F5",
      "ntp_link": "#F594C1",
      "button_background": "#403A40",
      "toolbar_button_icon": "#C6D0F5",
      "toolbar_text": "#C6D0F5",
      "omnibox_background": "#342D34",
      "omnibox_text": "#C6D0F5",
      "omnibox_max_contrast": true,
      "tab_background_highlighted_text": "#FA906E",
      "background_tab": "#342D34",
      "background_tab_inactive": "#342D34",
      "tab_line": "#FA906E",
      "background_tab_highlighted": "#403A40",
      "window_control_background": "#2A2023",
      "window_control_button_background": "#2A2023",
      "window_control_icon": "#C6D0F5",
      "window_control_hover_background": "#403A40",
      "window_control_icon_hover": "#FA906E",
      "toolbar_bottom_separator": "#403A40",
      "toolbar_vertical_separator": "#403A40",
      "dialog_background": "#2A2023",
      "dialog_text": "#C6D0F5",
      "dialog_border": "#403A40"
    },
    "tints": {
      "frame": [0.95, 0.26, 0.30],
      "frame_inactive": [0.95, 0.26, 0.60],
      "buttons": [0.95, 0.26, 0.50]
    },
    "properties": {
      "ntp_background_alignment": "center",
      "ntp_background_repeat": "no-repeat",
      "ntp_logo_alternate": true,
      "color_scheme": "dark",
      "tab_layout": "modern",
      "corner_style": "rounded",
      "dark_mode_style": "system"
    },
    "images": {
      "theme_ntp_background": "images/background.png",
      "theme_toolbar": "images/theme_toolbar.png",
      "theme_tab_background": "images/theme_tab_background.png"
    }
  },
  "dark_mode": {
    "theme": {
      "colors": {
        "frame": "#2A2023",
        "frame_inactive": "#342D34",
        "frame_incognito": "#1A181A",
        "frame_incognito_inactive": "#221F22",
        "toolbar": "#2A2023",
        "tab_text": "#C6D0F5",
        "tab_background_text": "#B5A9AF",
        "bookmark_text": "#C6D0F5",
        "ntp_background": "#2A2023",
        "ntp_text": "#C6D0F5",
        "ntp_link": "#F594C1",
        "button_background": "#403A40",
        "toolbar_button_icon": "#C6D0F5",
        "toolbar_text": "#C6D0F5",
        "omnibox_background": "#342D34",
        "omnibox_text": "#C6D0F5",
        "omnibox_max_contrast": true,
        "tab_background_highlighted_text": "#FA906E",
        "background_tab": "#342D34",
        "background_tab_inactive": "#342D34",
        "tab_line": "#FA906E",
        "background_tab_highlighted": "#403A40",
        "window_control_background": "#2A2023",
        "window_control_button_background": "#2A2023",
        "window_control_icon": "#C6D0F5",
        "window_control_hover_background": "#403A40",
        "window_control_icon_hover": "#FA906E",
        "toolbar_bottom_separator": "#403A40",
        "toolbar_vertical_separator": "#403A40",
        "dialog_background": "#2A2023",
        "dialog_text": "#C6D0F5",
        "dialog_border": "#403A40"
      }
    }
  },
  "light_mode": {
    "theme": {
      "colors": {
        "frame": "#FAF4F2",
        "frame_inactive": "#F5F1EB",
        "frame_incognito": "#E5E0DD",
        "frame_incognito_inactive": "#EBE6E3",
        "toolbar": "#FAF4F2",
        "tab_text": "#384242",
        "tab_background_text": "#95726A",
        "bookmark_text": "#384242",
        "ntp_background": "#FAF4F2",
        "ntp_text": "#384242",
        "ntp_link": "#FA906E",
        "button_background": "#FDE6DE",
        "toolbar_button_icon": "#384242",
        "toolbar_text": "#384242",
        "omnibox_background": "#F5F1EB",
        "omnibox_text": "#384242",
        "omnibox_max_contrast": true,
        "tab_background_highlighted_text": "#FA906E",
        "background_tab": "#F5F1EB",
        "background_tab_inactive": "#F5F1EB",
        "tab_line": "#FA906E",
        "background_tab_highlighted": "#FDE6DE",
        "window_control_background": "#FAF4F2",
        "window_control_button_background": "#FAF4F2",
        "window_control_icon": "#384242",
        "window_control_hover_background": "#FDE6DE",
        "window_control_icon_hover": "#FA906E",
        "toolbar_bottom_separator": "#EADBCC",
        "toolbar_vertical_separator": "#EADBCC",
        "dialog_background": "#FAF4F2",
        "dialog_text": "#384242",
        "dialog_border": "#EADBCC"
      },
      "tints": {
        "frame": [1.0, 0.99, 0.95],
        "frame_inactive": [1.0, 0.99, 0.80],
        "buttons": [1.0, 0.99, 0.80]
      },
      "properties": {
        "ntp_background_alignment": "center",
        "ntp_background_repeat": "no-repeat",
        "ntp_logo_alternate": false,
        "color_scheme": "light",
        "tab_layout": "modern",
        "corner_style": "rounded",
        "dark_mode_style": "system"
      },
      "images": {
        "theme_ntp_background": "images/background_light.png",
        "theme_toolbar": "images/theme_toolbar_light.png",
        "theme_tab_background": "images/theme_tab_background_light.png"
      }
    }
  },
  "theme_metadata": {
    "author": "Your Name",
    "version": "1.0.0",
    "dynamic_theme": true,
    "supports_overlay_scrollbar": true,
    "respects_os_appearance": true
  }
}
```

### Creating Required Images

For the theme to work properly, create the following images:

1. `background.png` - A 2560x1440 background image for the new tab page (dark mode)
2. `background_light.png` - A 2560x1440 background image for the new tab page (light mode)
3. `theme_toolbar.png` - A 1x1 transparent PNG or a textured background for the toolbar (dark mode)
4. `theme_toolbar_light.png` - A 1x1 transparent PNG or a textured background for the toolbar (light mode)
5. `theme_tab_background.png` - A 1x1 transparent PNG or a textured background for tabs (dark mode)
6. `theme_tab_background_light.png` - A 1x1 transparent PNG or a textured background for tabs (light mode)

### Advanced Chrome Theming (2025 Features)

Chrome version 135+ supports advanced theming features:

```json
"advanced_theme_settings": {
  "animated_toolbar": {
    "animation_url": "animations/toolbar_animation.webm",
    "animation_duration": 10000,
    "animation_timing": "ease-in-out",
    "animation_repeat": "infinite"
  },
  "custom_css_rules": [
    ".tab-hover-card { background-color: #403A40 !important; color: #C6D0F5 !important; border-color: #FA906E !important; }",
    ".dropdown-menu { background-color: #342D34 !important; border-color: #403A40 !important; }",
    ".dropdown-item { color: #C6D0F5 !important; }",
    ".dropdown-item:hover { background-color: #403A40 !important; color: #FA906E !important; }"
  ],
  "theme_transition": {
    "transition_duration": 300,
    "transition_timing": "ease"
  }
}
```

## Microsoft Edge Theme

Edge has enhanced its theming capabilities in version 135+ (2025), closely following Chrome's improvements with some Microsoft-specific additions.

### Installation Instructions

The process is similar to Chrome:

1. Create a folder for your theme
2. Create the required files as described below
3. Go to `edge://extensions/`
4. Enable "Developer mode" in the top-right corner
5. Click "Load unpacked" and select your theme folder
6. The theme will be instantly applied

### Edge Theme Manifest (manifest.json)

```json
{
  "name": "Warm Sunset",
  "version": "1.0",
  "description": "A warm and cozy theme with sunset colors",
  "manifest_version": 3,
  "theme": {
    "colors": {
      "frame": "#2A2023",
      "frame_inactive": "#342D34",
      "frame_incognito": "#1A181A",
      "frame_incognito_inactive": "#221F22",
      "toolbar": "#2A2023",
      "tab_text": "#C6D0F5",
      "tab_background_text": "#B5A9AF",
      "bookmark_text": "#C6D0F5",
      "ntp_background": "#2A2023",
      "ntp_text": "#C6D0F5",
      "ntp_link": "#F594C1",
      "button_background": "#403A40",
      "toolbar_button_icon": "#C6D0F5",
      "toolbar_text": "#C6D0F5",
      "omnibox_background": "#342D34",
      "omnibox_text": "#C6D0F5",
      "omnibox_max_contrast": true,
      "tab_background_highlighted_text": "#FA906E",
      "background_tab": "#342D34",
      "background_tab_inactive": "#342D34",
      "tab_line": "#FA906E",
      "background_tab_highlighted": "#403A40",
      "toolbar_bottom_separator": "#403A40",
      "toolbar_vertical_separator": "#403A40"
    },
    "tints": {
      "frame": [0.95, 0.26, 0.30],
      "frame_inactive": [0.95, 0.26, 0.60],
      "buttons": [0.95, 0.26, 0.50]
    },
    "properties": {
      "ntp_background_alignment": "center",
      "ntp_background_repeat": "no-repeat",
      "color_scheme": "dark",
      "tab_layout": "modern",
      "corner_style": "rounded"
    },
    "images": {
      "theme_ntp_background": "images/background.png",
      "theme_toolbar": "images/theme_toolbar.png",
      "theme_tab_background": "images/theme_tab_background.png"
    }
  },
  "dark_mode": {
    "theme": {
      "colors": {
        "frame": "#2A2023",
        "frame_inactive": "#342D34",
        "frame_incognito": "#1A181A",
        "frame_incognito_inactive": "#221F22",
        "toolbar": "#2A2023",
        "tab_text": "#C6D0F5",
        "tab_background_text": "#B5A9AF",
        "bookmark_text": "#C6D0F5",
        "ntp_background": "#2A2023",
        "ntp_text": "#C6D0F5",
        "ntp_link": "#F594C1",
        "button_background": "#403A40",
        "toolbar_button_icon": "#C6D0F5",
        "toolbar_text": "#C6D0F5",
        "omnibox_background": "#342D34",
        "omnibox_text": "#C6D0F5",
        "omnibox_max_contrast": true,
        "tab_background_highlighted_text": "#FA906E",
        "background_tab": "#342D34",
        "background_tab_inactive": "#342D34",
        "tab_line": "#FA906E",
        "background_tab_highlighted": "#403A40",
        "toolbar_bottom_separator": "#403A40",
        "toolbar_vertical_separator": "#403A40"
      }
    }
  },
  "light_mode": {
    "theme": {
      "colors": {
        "frame": "#FAF4F2",
        "frame_inactive": "#F5F1EB",
        "frame_incognito": "#E5E0DD",
        "frame_incognito_inactive": "#EBE6E3",
        "toolbar": "#FAF4F2",
        "tab_text": "#384242",
        "tab_background_text": "#95726A",
        "bookmark_text": "#384242",
        "ntp_background": "#FAF4F2",
        "ntp_text": "#384242",
        "ntp_link": "#FA906E",
        "button_background": "#FDE6DE",
        "toolbar_button_icon": "#384242",
        "toolbar_text": "#384242",
        "omnibox_background": "#F5F1EB",
        "omnibox_text": "#384242",
        "omnibox_max_contrast": true,
        "tab_background_highlighted_text": "#FA906E",
        "background_tab": "#F5F1EB",
        "background_tab_inactive": "#F5F1EB",
        "tab_line": "#FA906E",
        "background_tab_highlighted": "#FDE6DE",
        "toolbar_bottom_separator": "#EADBCC",
        "toolbar_vertical_separator": "#EADBCC"
      },
      "tints": {
        "frame": [1.0, 0.99, 0.95],
        "frame_inactive": [1.0, 0.99, 0.80],
        "buttons": [1.0, 0.99, 0.80]
      }
    }
  },
  "edge_specific_settings": {
    "new_tab_page": {
      "custom_background_color": "#2A2023",
      "custom_text_color": "#C6D0F5",
      "custom_link_color": "#F594C1",
      "custom_button_color": "#FA906E",
      "custom_button_text_color": "#2A2023",
      "show_greeting": true,
      "greeting_text_color": "#FA906E",
      "accent_color": "#FA906E"
    },
    "sidebar": {
      "background_color": "#342D34",
      "text_color": "#C6D0F5",
      "accent_color": "#FA906E",
      "hover_color": "#403A40",
      "active_color": "#403A40"
    },
    "immersive_reader": {
      "background_color": "#2A2023",
      "text_color": "#C6D0F5",
      "accent_color": "#FA906E"
    },
    "collections": {
      "background_color": "#2A2023",
      "text_color": "#C6D0F5",
      "accent_color": "#FA906E",
      "card_background_color": "#342D34",
      "card_border_color": "#403A40"
    }
  },
  "theme_metadata": {
    "author": "Your Name",
    "version": "1.0.0",
    "dynamic_theme": true
  }
}
```

### Edge-Specific Features (2025)

Microsoft Edge has introduced some unique features for its themes:

```json
"edge_features": {
  "vertical_tabs": {
    "background_color": "#342D34",
    "text_color": "#C6D0F5",
    "active_tab_background": "#403A40",
    "active_tab_text": "#FA906E",
    "hover_tab_background": "#403A4080",
    "hover_tab_text": "#FA906E"
  },
  "workspace": {
    "background_color": "#2A2023",
    "text_color": "#C6D0F5",
    "accent_color": "#FA906E",
    "card_background": "#342D34",
    "card_border": "#403A40",
    "card_text": "#C6D0F5"
  },
  "performance_mode": {
    "indicator_active": "#A6D18C",
    "indicator_inactive": "#B5A9AF"
  }
}
```

## Firefox Theme

Firefox has significantly improved its theme API in version 135+ (2025), allowing for more customization and better alignment with Chrome and Edge features.

### Installation Instructions

#### Method 1: Firefox Add-ons (Recommended)

1. Create a Firefox theme package using the instructions below
2. Create a Firefox Developer account if you don't have one
3. Upload your theme to Firefox Add-ons
4. Install your published theme from Firefox Add-ons

#### Method 2: Developer Mode (Local Installation)

1. Create a folder for your theme
2. Create the required files as described below
3. Go to `about:debugging#/runtime/this-firefox`
4. Click "Load Temporary Add-on" and select your manifest.json file
5. The theme will be temporarily applied (will be removed on restart)

### Firefox Theme Manifest (manifest.json)

```json
{
  "manifest_version": 3,
  "name": "Warm Sunset",
  "version": "1.0",
  "author": "Your Name",
  "description": "A warm and cozy theme with sunset colors",
  "browser_specific_settings": {
    "gecko": {
      "id": "warm-sunset@yourdomain.com"
    }
  },
  "theme": {
    "colors": {
      "frame": "#2A2023",
      "tab_background_text": "#B5A9AF",
      "tab_text": "#C6D0F5",
      "tab_line": "#FA906E",
      "tab_loading": "#FA906E",
      "tab_selected": "#342D34",
      "tab_background_separator": "#403A40",
      "toolbar": "#2A2023",
      "toolbar_field": "#342D34",
      "toolbar_field_text": "#C6D0F5",
      "toolbar_field_border": "#403A40",
      "toolbar_field_focus": "#342D34",
      "toolbar_field_text_focus": "#C6D0F5",
      "toolbar_field_border_focus": "#FA906E",
      "toolbar_top_separator": "#403A40",
      "toolbar_bottom_separator": "#403A40",
      "toolbar_vertical_separator": "#403A40",
      "toolbar_field_highlight": "#FA906E40",
      "toolbar_field_highlight_text": "#C6D0F5",
      "button_background_hover": "#403A40",
      "button_background_active": "#403A40",
      "icons": "#C6D0F5",
      "icons_attention": "#FA906E",
      "bookmark_text": "#C6D0F5",
      "ntp_background": "#2A2023",
      "ntp_text": "#C6D0F5",
      "popup": "#342D34",
      "popup_text": "#C6D0F5",
      "popup_border": "#403A40",
      "popup_highlight": "#403A40",
      "popup_highlight_text": "#FA906E",
      "sidebar": "#342D34",
      "sidebar_text": "#C6D0F5",
      "sidebar_border": "#403A40",
      "sidebar_highlight": "#403A40",
      "sidebar_highlight_text": "#FA906E",
      "error_text": "#E78284",
      "warning_text": "#E5C890",
      "success_text": "#A6D18C"
    },
    "properties": {
      "color_scheme": "dark",
      "content_color_scheme": "dark",
      "panel_hover": "#403A40",
      "panel_active": "#403A40",
      "panel_normal": "#342D34"
    },
    "images": {
      "additional_backgrounds": ["images/background.png"]
    },
    "additional_backgrounds_alignment": ["center"],
    "additional_backgrounds_tiling": ["no-repeat"]
  },
  "dark_theme": {
    "colors": {
      "frame": "#2A2023",
      "tab_background_text": "#B5A9AF",
      "tab_text": "#C6D0F5",
      "tab_line": "#FA906E",
      "tab_loading": "#FA906E",
      "tab_selected": "#342D34",
      "tab_background_separator": "#403A40",
      "toolbar": "#2A2023",
      "toolbar_field": "#342D34",
      "toolbar_field_text": "#C6D0F5",
      "toolbar_field_border": "#403A40",
      "toolbar_field_focus": "#342D34",
      "toolbar_field_text_focus": "#C6D0F5",
      "toolbar_field_border_focus": "#FA906E",
      "toolbar_top_separator": "#403A40",
      "toolbar_bottom_separator": "#403A40",
      "toolbar_vertical_separator": "#403A40",
      "toolbar_field_highlight": "#FA906E40",
      "toolbar_field_highlight_text": "#C6D0F5",
      "button_background_hover": "#403A40",
      "button_background_active": "#403A40",
      "icons": "#C6D0F5",
      "icons_attention": "#FA906E",
      "bookmark_text": "#C6D0F5",
      "ntp_background": "#2A2023",
      "ntp_text": "#C6D0F5",
      "popup": "#342D34",
      "popup_text": "#C6D0F5",
      "popup_border": "#403A40",
      "popup_highlight": "#403A40",
      "popup_highlight_text": "#FA906E",
      "sidebar": "#342D34",
      "sidebar_text": "#C6D0F5",
      "sidebar_border": "#403A40",
      "sidebar_highlight": "#403A40",
      "sidebar_highlight_text": "#FA906E",
      "error_text": "#E78284",
      "warning_text": "#E5C890",
      "success_text": "#A6D18C"
    }
  },
  "light_theme": {
    "colors": {
      "frame": "#FAF4F2",
      "tab_background_text": "#95726A",
      "tab_text": "#384242",
      "tab_line": "#FA906E",
      "tab_loading": "#FA906E",
      "tab_selected": "#FAF4F2",
      "tab_background_separator": "#EADBCC",
      "toolbar": "#FAF4F2",
      "toolbar_field": "#F5F1EB",
      "toolbar_field_text": "#384242",
      "toolbar_field_border": "#EADBCC",
      "toolbar_field_focus": "#F5F1EB",
      "toolbar_field_text_focus": "#384242",
      "toolbar_field_border_focus": "#FA906E",
      "toolbar_top_separator": "#EADBCC",
      "toolbar_bottom_separator": "#EADBCC",
      "toolbar_vertical_separator": "#EADBCC",
      "toolbar_field_highlight": "#FA906E40",
      "toolbar_field_highlight_text": "#384242",
      "button_background_hover": "#FDE6DE",
      "button_background_active": "#FDE6DE",
      "icons": "#384242",
      "icons_attention": "#FA906E",
      "bookmark_text": "#384242",
      "ntp_background": "#FAF4F2",
      "ntp_text": "#384242",
      "popup": "#F5F1EB",
      "popup_text": "#384242",
      "popup_border": "#EADBCC",
      "popup_highlight": "#FDE6DE",
      "popup_highlight_text": "#FA906E",
      "sidebar": "#F5F1EB",
      "sidebar_text": "#384242",
      "sidebar_border": "#EADBCC",
      "sidebar_highlight": "#FDE6DE",
      "sidebar_highlight_text": "#FA906E",
      "error_text": "#E06053",
      "warning_text": "#F4BC5F",
      "success_text": "#A6D18C"
    },
    "properties": {
      "color_scheme": "light",
      "content_color_scheme": "light",
      "panel_hover": "#FDE6DE",
      "panel_active": "#FDE6DE",
      "panel_normal": "#F5F1EB"
    },
    "images": {
      "additional_backgrounds": ["images/background_light.png"]
    }
  },
  "firefox_specific": {
    "theme_experiment": {
      "stylesheet": "theme.css",
      "colors": {
        "accent_color": "#FA906E",
        "accent_color_active": "#F5BC5E",
        "download_progress_color": "#A6D18C",
        "status_bar_background": "#2A2023",
        "status_bar_text": "#C6D0F5"
      }
    }
  }
}
```

### Firefox Custom CSS (theme.css)

```css
/* Warm Sunset Firefox Theme - Custom CSS */

/* Custom scrollbars */
:root {
  scrollbar-color: #403A40 #342D34 !important;
}

/* Custom styling for Firefox's new tab page */
@-moz-document url(about:newtab), url(about:home) {
  body {
    background-color: #2A2023 !important;
    color: #C6D0F5 !important;
  }
  
  .top-site-outer .top-site-icon {
    background-color: #342D34 !important;
  }
  
  .search-wrapper .search-handoff-button {
    background-color: #342D34 !important;
    border-color: #403A40 !important;
    color: #C6D0F5 !important;
  }
  
  .search-wrapper .search-handoff-button:hover {
    background-color: #403A40 !important;
    border-color: #FA906E !important;
  }
  
  .top-sites-list .top-site-outer .context-menu-button {
    background-color: #342D34 !important;
    color: #C6D0F5 !important;
  }
  
  .top-sites-list .top-site-outer:hover .context-menu-button:hover {
    background-color: #403A40 !important;
    color: #FA906E !important;
  }
}

/* Custom styling for context menus */
menupopup {
  --menu-background-color: #342D34 !important;
  --menu-color: #C6D0F5 !important;
  --menu-border-color: #403A40 !important;
  --menu-item-hover-background-color: #403A40 !important;
  --menu-item-hover-color: #FA906E !important;
}

/* Firefox main menu dropdown */
.panel-mainview {
  background-color: #342D34 !important;
  color: #C6D0F5 !important;
  border-color: #403A40 !important;
}

.panel-subview-body {
  background-color: #342D34 !important;
}

.panel-mainview toolbarbutton:hover,
.panel-subview-body toolbarbutton:hover {
  background-color: #403A40 !important;
  color: #FA906E !important;
}

/* Firefox light mode overrides */
@media (prefers-color-scheme: light) {
  :root {
    scrollbar-color: #EADBCC #F5F1EB !important;
  }
  
  @-moz-document url(about:newtab), url(about:home) {
    body {
      background-color: #FAF4F2 !important;
      color: #384242 !important;
    }
    
    .top-site-outer .top-site-icon {
      background-color: #F5F1EB !important;
    }
    
    .search-wrapper .search-handoff-button {
      background-color: #F5F1EB !important;
      border-color: #EADBCC !important;
      color: #384242 !important;
    }
    
    .search-wrapper .search-handoff-button:hover {
      background-color: #FDE6DE !important;
      border-color: #FA906E !important;
    }
    
    .top-sites-list .top-site-outer .context-menu-button {
      background-color: #F5F1EB !important;
      color: #384242 !important;
    }
    
    .top-sites-list .top-site-outer:hover .context-menu-button:hover {
      background-color: #FDE6DE !important;
      color: #FA906E !important;
    }
  }
  
  menupopup {
    --menu-background-color: #F5F1EB !important;
    --menu-color: #384242 !important;
    --menu-border-color: #EADBCC !important;
    --menu-item-hover-background-color: #FDE6DE !important;
    --menu-item-hover-color: #FA906E !important;
  }
  
  .panel-mainview {
    background-color: #F5F1EB !important;
    color: #384242 !important;
    border-color: #EADBCC !important;
  }
  
  .panel-subview-body {
    background-color: #F5F1EB !important;
  }
  
  .panel-mainview toolbarbutton:hover,
  .panel-subview-body toolbarbutton:hover {
    background-color: #FDE6DE !important;
    color: #FA906E !important;
  }
}
```

### Advanced Firefox Theming (2025 Features)

Firefox in 2025 supports advanced theme effects like:

1. Create `theme_experiment.js` with:

```javascript
// Advanced Firefox theme features (2025)
const { classes: Cc, interfaces: Ci, utils: Cu } = Components;
const { AppConstants } = Cu.import("resource://gre/modules/AppConstants.jsm");

// Apply dynamic theme effects
function initThemeEffects(window) {
  const navbar = window.document.getElementById("nav-bar");
  
  // Add subtle animation on hover
  if (navbar) {
    navbar.addEventListener("mouseover", () => {
      navbar.style.transition = "background-color 0.3s ease";
      navbar.style.backgroundColor = "#342D34";
    });
    
    navbar.addEventListener("mouseout", () => {
      navbar.style.transition = "background-color 0.3s ease";
      navbar.style.backgroundColor = "";
    });
  }
  
  // Add highlight effect to active tab
  const tabsBar = window.document.getElementById("TabsToolbar");
  if (tabsBar) {
    // Subtle glow effect for active tab
    const style = window.document.createElement("style");
    style.textContent = `
      .tab-content[selected="true"] {
        box-shadow: 0 0 8px #FA906E40 !important;
      }
    `;
    window.document.head.appendChild(style);
  }
}

// Initialize theme enhancements when windows are created
function onWindowCreated(window) {
  if (window.document.documentElement.getAttribute("windowtype") === "navigator:browser") {
    initThemeEffects(window);
  }
}

// Monitor window creation
function startup() {
  const windowListener = {
    onOpenWindow: function(xulWindow) {
      const window = xulWindow.QueryInterface(Ci.nsIInterfaceRequestor)
                            .getInterface(Ci.nsIDOMWindow);
      window.addEventListener("load", function listener() {
        window.removeEventListener("load", listener);
        onWindowCreated(window);
      });
    },
    onCloseWindow: function() {},
    onWindowTitleChange: function() {}
  };
  
  const windowService = Cc["@mozilla.org/appshell/window-mediator;1"]
                      .getService(Ci.nsIWindowMediator);
  
  // Apply to existing windows
  const windows = windowService.getEnumerator("navigator:browser");
  while (windows.hasMoreElements()) {
    const window = windows.getNext().QueryInterface(Ci.nsIDOMWindow);
    onWindowCreated(window);
  }
  
  // Listen for new windows
  windowService.addListener(windowListener);
}

startup();
```

2. Add to `manifest.json`:

```json
"experiment_apis": {
  "theme_experiment": {
    "schema": "theme_experiment_schema.json",
    "parent": {
      "scopes": ["addon_parent"],
      "paths": [["theme_experiment"]],
      "script": "theme_experiment.js"
    }
  }
}
```
