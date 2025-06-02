# JetBrains IDEs Theme (2025 Edition)

This theme is compatible with all JetBrains IDEs including IntelliJ IDEA, PyCharm, WebStorm, PhpStorm, Rider, and others. JetBrains IDEs in 2025 now support their enhanced Theme API 3.0 with more customizable elements and improved plugin support.

## Installation Instructions

### Method 1: Import from Settings

1. Download the `.icls` files for your preferred theme
2. Open your JetBrains IDE
3. Go to `Settings` > `Editor` > `Color Scheme`
4. Click the gear icon and select `Import Scheme`
5. Browse to the downloaded `.icls` file and click `OK`
6. Select the imported scheme and click `Apply`

### Method 2: Install as Plugin (New in 2025)

1. Download the `.jar` file (bundled plugin)
2. Open your JetBrains IDE
3. Go to `Settings` > `Plugins`
4. Click the gear icon and select `Install Plugin from Disk...`
5. Browse to the downloaded `.jar` file and click `OK`
6. Restart the IDE when prompted
7. The themes will appear in `Settings` > `Editor` > `Color Scheme`

## Dark Theme (XML Configuration)

Save this as `Warm-Sunset-Dark.icls`:

```xml
<scheme name="Warm Sunset Dark" version="142" parent_scheme="Darcula">
  <metaInfo>
    <property name="created">2025-05-16T12:00:00</property>
    <property name="ide">idea</property>
    <property name="ideVersion">2025.1.0.0</property>
    <property name="modified">2025-05-16T12:00:00</property>
    <property name="originalScheme">Warm Sunset Dark</property>
    <property name="vendorMail">your-email@example.com</property>
    <property name="vendorName">Your Name</property>
    <property name="vendorUrl">https://your-website.com</property>
  </metaInfo>
  <colors>
    <!-- Main IDE colors -->
    <option name="EDITOR_BACKGROUND" value="#2A2023" />
    <option name="CARET_ROW_COLOR" value="#342D34" />
    <option name="CONSOLE_BACKGROUND_KEY" value="#2A2023" />
    <option name="GUTTER_BACKGROUND" value="#2A2023" />
    <option name="LINE_NUMBERS_COLOR" value="#B5A9AF" />
    <option name="SELECTED_INDENT_GUIDE" value="#FA906E" />
    <option name="SELECTION_BACKGROUND" value="#626880" />
    <option name="SELECTION_FOREGROUND" value="#C6D0F5" />
    <option name="TEARLINE_COLOR" value="#403A40" />
    <option name="WHITESPACES" value="#403A4055" />
    
    <!-- UI colors -->
    <option name="BORDER_LINES_COLOR" value="#403A40" />
    <option name="NOTIFICATION_BACKGROUND" value="#342D34" />
    <option name="RECENT_LOCATIONS_SELECTION" value="#403A40" />
    <option name="RIGHT_MARGIN_COLOR" value="#403A40" />
    <option name="VISUAL_INDENT_GUIDE" value="#403A40" />
    
    <!-- New in 2025: AI assistant panel -->
    <option name="AI_PANEL_BACKGROUND" value="#342D34" />
    <option name="AI_PANEL_FOREGROUND" value="#C6D0F5" />
    <option name="AI_USER_MESSAGE_BACKGROUND" value="#FA906E30" />
    <option name="AI_ASSISTANT_MESSAGE_BACKGROUND" value="#403A40" />
    
    <!-- New in 2025: Collaborative editing highlights -->
    <option name="COLLABORATIVE_USER_1" value="#FA906E" />
    <option name="COLLABORATIVE_USER_2" value="#F594C1" />
    <option name="COLLABORATIVE_USER_3" value="#F5BC5E" />
    <option name="COLLABORATIVE_USER_4" value="#A6D18C" />
  </colors>
  <attributes>
    <!-- Basic attributes -->
    <option name="DEFAULT_BLOCK_COMMENT">
      <value>
        <option name="FOREGROUND" value="#B5A9AF" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_BRACES">
      <value>
        <option name="FOREGROUND" value="#C6D0F5" />
      </value>
    </option>
    <option name="DEFAULT_BRACKETS">
      <value>
        <option name="FOREGROUND" value="#C6D0F5" />
      </value>
    </option>
    <option name="DEFAULT_CLASS_NAME">
      <value>
        <option name="FOREGROUND" value="#E5C890" />
      </value>
    </option>
    <option name="DEFAULT_COMMA">
      <value>
        <option name="FOREGROUND" value="#C6D0F5" />
      </value>
    </option>
    <option name="DEFAULT_CONSTANT">
      <value>
        <option name="FOREGROUND" value="#F5BC5E" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_DOC_COMMENT">
      <value>
        <option name="FOREGROUND" value="#B5A9AF" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_DOC_COMMENT_TAG">
      <value>
        <option name="FOREGROUND" value="#F594C1" />
        <option name="FONT_TYPE" value="3" />
        <option name="EFFECT_TYPE" value="1" />
      </value>
    </option>
    <option name="DEFAULT_FUNCTION_CALL">
      <value>
        <option name="FOREGROUND" value="#8CAAEE" />
      </value>
    </option>
    <option name="DEFAULT_FUNCTION_DECLARATION">
      <value>
        <option name="FOREGROUND" value="#8CAAEE" />
      </value>
    </option>
    <option name="DEFAULT_IDENTIFIER">
      <value>
        <option name="FOREGROUND" value="#C6D0F5" />
      </value>
    </option>
    <option name="DEFAULT_INSTANCE_FIELD">
      <value>
        <option name="FOREGROUND" value="#FA906E" />
      </value>
    </option>
    <option name="DEFAULT_INTERFACE_NAME">
      <value>
        <option name="FOREGROUND" value="#E5C890" />
      </value>
    </option>
    <option name="DEFAULT_KEYWORD">
      <value>
        <option name="FOREGROUND" value="#F594C1" />
        <option name="FONT_TYPE" value="1" />
      </value>
    </option>
    <option name="DEFAULT_LINE_COMMENT">
      <value>
        <option name="FOREGROUND" value="#B5A9AF" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_NUMBER">
      <value>
        <option name="FOREGROUND" value="#F5BC5E" />
      </value>
    </option>
    <option name="DEFAULT_OPERATION_SIGN">
      <value>
        <option name="FOREGROUND" value="#FA906E" />
      </value>
    </option>
    <option name="DEFAULT_PARAMETER">
      <value>
        <option name="FOREGROUND" value="#C6D0F5" />
      </value>
    </option>
    <option name="DEFAULT_PARENTHS">
      <value>
        <option name="FOREGROUND" value="#C6D0F5" />
      </value>
    </option>
    <option name="DEFAULT_SEMICOLON">
      <value>
        <option name="FOREGROUND" value="#C6D0F5" />
      </value>
    </option>
    <option name="DEFAULT_STATIC_FIELD">
      <value>
        <option name="FOREGROUND" value="#FA906E" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_STATIC_METHOD">
      <value>
        <option name="FOREGROUND" value="#8CAAEE" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_STRING">
      <value>
        <option name="FOREGROUND" value="#A6D18C" />
      </value>
    </option>
    <option name="DEFAULT_TEMPLATE_LANGUAGE_COLOR">
      <value>
        <option name="BACKGROUND" value="#2A202355" />
      </value>
    </option>
    <option name="TEXT">
      <value>
        <option name="FOREGROUND" value="#C6D0F5" />
        <option name="BACKGROUND" value="#2A2023" />
      </value>
    </option>
    
    <!-- Error and warning highlighting -->
    <option name="ERROR_HINT">
      <value>
        <option name="EFFECT_COLOR" value="#E78284" />
        <option name="EFFECT_TYPE" value="2" />
      </value>
    </option>
    <option name="WARNING_ATTRIBUTES">
      <value>
        <option name="EFFECT_COLOR" value="#E5C890" />
        <option name="EFFECT_TYPE" value="2" />
      </value>
    </option>
    
    <!-- Specific language attributes -->
    <!-- Java -->
    <option name="JAVA_KEYWORD">
      <value>
        <option name="FOREGROUND" value="#F594C1" />
      </value>
    </option>
    
    <!-- JavaScript/TypeScript -->
    <option name="JS.GLOBAL_VARIABLE">
      <value>
        <option name="FOREGROUND" value="#F5BC5E" />
      </value>
    </option>
    <option name="JS.LOCAL_VARIABLE">
      <value>
        <option name="FOREGROUND" value="#C6D0F5" />
      </value>
    </option>
    
    <!-- Markdown -->
    <option name="MARKDOWN_HEADING">
      <value>
        <option name="FOREGROUND" value="#FA906E" />
        <option name="FONT_TYPE" value="1" />
      </value>
    </option>
    
    <!-- Python -->
    <option name="PY.SELF_PARAMETER">
      <value>
        <option name="FOREGROUND" value="#F594C1" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    
    <!-- New in 2025: AI Code Completion -->
    <option name="AI_COMPLETED_TEXT">
      <value>
        <option name="FOREGROUND" value="#B5A9AF" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
  </attributes>
</scheme>
```

## Light Theme (XML Configuration)

Save this as `Warm-Sunset-Light.icls`:

```xml
<scheme name="Warm Sunset Light" version="142" parent_scheme="Default">
  <metaInfo>
    <property name="created">2025-05-16T12:00:00</property>
    <property name="ide">idea</property>
    <property name="ideVersion">2025.1.0.0</property>
    <property name="modified">2025-05-16T12:00:00</property>
    <property name="originalScheme">Warm Sunset Light</property>
    <property name="vendorMail">your-email@example.com</property>
    <property name="vendorName">Your Name</property>
    <property name="vendorUrl">https://your-website.com</property>
  </metaInfo>
  <colors>
    <!-- Main IDE colors -->
    <option name="EDITOR_BACKGROUND" value="#FAF4F2" />
    <option name="CARET_ROW_COLOR" value="#F5F1EB" />
    <option name="CONSOLE_BACKGROUND_KEY" value="#FAF4F2" />
    <option name="GUTTER_BACKGROUND" value="#FAF4F2" />
    <option name="LINE_NUMBERS_COLOR" value="#95726A" />
    <option name="SELECTED_INDENT_GUIDE" value="#FA906E" />
    <option name="SELECTION_BACKGROUND" value="#FBD6B9" />
    <option name="SELECTION_FOREGROUND" value="#384242" />
    <option name="TEARLINE_COLOR" value="#EADBCC" />
    <option name="WHITESPACES" value="#EADBCC55" />
    
    <!-- UI colors -->
    <option name="BORDER_LINES_COLOR" value="#EADBCC" />
    <option name="NOTIFICATION_BACKGROUND" value="#F5F1EB" />
    <option name="RECENT_LOCATIONS_SELECTION" value="#FDE6DE" />
    <option name="RIGHT_MARGIN_COLOR" value="#EADBCC" />
    <option name="VISUAL_INDENT_GUIDE" value="#EADBCC" />
    
    <!-- New in 2025: AI assistant panel -->
    <option name="AI_PANEL_BACKGROUND" value="#F5F1EB" />
    <option name="AI_PANEL_FOREGROUND" value="#384242" />
    <option name="AI_USER_MESSAGE_BACKGROUND" value="#FA906E30" />
    <option name="AI_ASSISTANT_MESSAGE_BACKGROUND" value="#FDE6DE" />
    
    <!-- New in 2025: Collaborative editing highlights -->
    <option name="COLLABORATIVE_USER_1" value="#FA906E" />
    <option name="COLLABORATIVE_USER_2" value="#C77DBB" />
    <option name="COLLABORATIVE_USER_3" value="#F5BC5E" />
    <option name="COLLABORATIVE_USER_4" value="#A6D18C" />
  </colors>
  <attributes>
    <!-- Basic attributes -->
    <option name="DEFAULT_BLOCK_COMMENT">
      <value>
        <option name="FOREGROUND" value="#95726A" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_BRACES">
      <value>
        <option name="FOREGROUND" value="#384242" />
      </value>
    </option>
    <option name="DEFAULT_BRACKETS">
      <value>
        <option name="FOREGROUND" value="#384242" />
      </value>
    </option>
    <option name="DEFAULT_CLASS_NAME">
      <value>
        <option name="FOREGROUND" value="#F4BC5F" />
      </value>
    </option>
    <option name="DEFAULT_COMMA">
      <value>
        <option name="FOREGROUND" value="#384242" />
      </value>
    </option>
    <option name="DEFAULT_CONSTANT">
      <value>
        <option name="FOREGROUND" value="#F5BC5E" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_DOC_COMMENT">
      <value>
        <option name="FOREGROUND" value="#95726A" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_DOC_COMMENT_TAG">
      <value>
        <option name="FOREGROUND" value="#C77DBB" />
        <option name="FONT_TYPE" value="3" />
        <option name="EFFECT_TYPE" value="1" />
      </value>
    </option>
    <option name="DEFAULT_FUNCTION_CALL">
      <value>
        <option name="FOREGROUND" value="#7B90D4" />
      </value>
    </option>
    <option name="DEFAULT_FUNCTION_DECLARATION">
      <value>
        <option name="FOREGROUND" value="#7B90D4" />
      </value>
    </option>
    <option name="DEFAULT_IDENTIFIER">
      <value>
        <option name="FOREGROUND" value="#384242" />
      </value>
    </option>
    <option name="DEFAULT_INSTANCE_FIELD">
      <value>
        <option name="FOREGROUND" value="#FA906E" />
      </value>
    </option>
    <option name="DEFAULT_INTERFACE_NAME">
      <value>
        <option name="FOREGROUND" value="#F4BC5F" />
      </value>
    </option>
    <option name="DEFAULT_KEYWORD">
      <value>
        <option name="FOREGROUND" value="#C77DBB" />
        <option name="FONT_TYPE" value="1" />
      </value>
    </option>
    <option name="DEFAULT_LINE_COMMENT">
      <value>
        <option name="FOREGROUND" value="#95726A" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_NUMBER">
      <value>
        <option name="FOREGROUND" value="#F5BC5E" />
      </value>
    </option>
    <option name="DEFAULT_OPERATION_SIGN">
      <value>
        <option name="FOREGROUND" value="#FA906E" />
      </value>
    </option>
    <option name="DEFAULT_PARAMETER">
      <value>
        <option name="FOREGROUND" value="#384242" />
      </value>
    </option>
    <option name="DEFAULT_PARENTHS">
      <value>
        <option name="FOREGROUND" value="#384242" />
      </value>
    </option>
    <option name="DEFAULT_SEMICOLON">
      <value>
        <option name="FOREGROUND" value="#384242" />
      </value>
    </option>
    <option name="DEFAULT_STATIC_FIELD">
      <value>
        <option name="FOREGROUND" value="#FA906E" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_STATIC_METHOD">
      <value>
        <option name="FOREGROUND" value="#7B90D4" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    <option name="DEFAULT_STRING">
      <value>
        <option name="FOREGROUND" value="#A6D18C" />
      </value>
    </option>
    <option name="DEFAULT_TEMPLATE_LANGUAGE_COLOR">
      <value>
        <option name="BACKGROUND" value="#FAF4F255" />
      </value>
    </option>
    <option name="TEXT">
      <value>
        <option name="FOREGROUND" value="#384242" />
        <option name="BACKGROUND" value="#FAF4F2" />
      </value>
    </option>
    
    <!-- Error and warning highlighting -->
    <option name="ERROR_HINT">
      <value>
        <option name="EFFECT_COLOR" value="#E06053" />
        <option name="EFFECT_TYPE" value="2" />
      </value>
    </option>
    <option name="WARNING_ATTRIBUTES">
      <value>
        <option name="EFFECT_COLOR" value="#F4BC5F" />
        <option name="EFFECT_TYPE" value="2" />
      </value>
    </option>
    
    <!-- Specific language attributes -->
    <!-- Java -->
    <option name="JAVA_KEYWORD">
      <value>
        <option name="FOREGROUND" value="#C77DBB" />
      </value>
    </option>
    
    <!-- JavaScript/TypeScript -->
    <option name="JS.GLOBAL_VARIABLE">
      <value>
        <option name="FOREGROUND" value="#F5BC5E" />
      </value>
    </option>
    <option name="JS.LOCAL_VARIABLE">
      <value>
        <option name="FOREGROUND" value="#384242" />
      </value>
    </option>
    
    <!-- Markdown -->
    <option name="MARKDOWN_HEADING">
      <value>
        <option name="FOREGROUND" value="#FA906E" />
        <option name="FONT_TYPE" value="1" />
      </value>
    </option>
    
    <!-- Python -->
    <option name="PY.SELF_PARAMETER">
      <value>
        <option name="FOREGROUND" value="#C77DBB" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
    
    <!-- New in 2025: AI Code Completion -->
    <option name="AI_COMPLETED_TEXT">
      <value>
        <option name="FOREGROUND" value="#95726A" />
        <option name="FONT_TYPE" value="2" />
      </value>
    </option>
  </attributes>
</scheme>
```

## Creating a Custom JetBrains Plugin (2025 Method)

In 2025, JetBrains introduced a simpler way to create and distribute theme plugins using the Theme Creator tool:

1. Go to JetBrains Theme Creator at https://plugins.jetbrains.com/theme-creator/
2. Upload your ICLS files
3. Fill in the plugin metadata
4. Generate the plugin JAR

This method automatically creates a plugin that can be installed directly through the JetBrains Marketplace or from disk.

## Theme Customization for Specific IDEs

JetBrains now allows specific customizations for different IDEs while maintaining the base theme. Here's how to extend the theme for specific IDEs:

### For PyCharm

Add these to the attributes section:

```xml
<option name="PY.KEYWORD">
  <value>
    <option name="FOREGROUND" value="#F594C1" />
    <option name="FONT_TYPE" value="1" />
  </value>
</option>
<option name="PY.BUILTIN_NAME">
  <value>
    <option name="FOREGROUND" value="#8CAAEE" />
  </value>
</option>
```

### For WebStorm

Add these to the attributes section:

```xml
<option name="JS.REGEXP">
  <value>
    <option name="FOREGROUND" value="#89DCEB" />
  </value>
</option>
<option name="JS.MODULE_NAME">
  <value>
    <option name="FOREGROUND" value="#E5C890" />
  </value>
</option>
```
