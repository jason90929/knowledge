```
Windows:路徑位置：C:\Users\志豪\.IntelliJIdea14\config\colors
```

```
Mac步驟：
- 從Idea建立一個Color & font名稱，並隨便修改個東西(為了讓他產生資料)後關閉Idea
- 到~/Library/Preferences/IntelliJIdea15/colors/${檔案名稱}.icls
- vi進去複製以下全貼上，存檔離開。重新開啟Idea
```

```xml
<scheme name=“jason_custom" version="142" parent_scheme="Default">
  <option name="LINE_SPACING" value="1.0" />
  <option name="EDITOR_FONT_SIZE" value="12" />
  <option name="CONSOLE_FONT_NAME" value="Monospaced" />
  <option name="EDITOR_FONT_NAME" value="Source Code Pro Semibold" />
  <attributes>
    <option name="BREAKPOINT_ATTRIBUTES">
      <value>
        <option name="BACKGROUND" value="ffc8c8" />
        <option name="ERROR_STRIPE_COLOR" value="ffc8c8" />
      </value>
    </option>
    <option name="COFFEESCRIPT.EXPRESSIONS_SUBSTITUTION_MARK">
      <value>
        <option name="FOREGROUND" value="a9b7c6" />
        <option name="EFFECT_TYPE" value="5" />
      </value>
    </option>
    <option name="DEFAULT_COMMA">
      <value>
        <option name="FOREGROUND" value="cc7832" />
      </value>
    </option>
    <option name="DEFAULT_KEYWORD">
      <value>
        <option name="FOREGROUND" value="80" />
        <option name="BACKGROUND" value="f5f2e9" />
        <option name="FONT_TYPE" value="1" />
      </value>
    </option>
    <option name="DEFAULT_PARAMETER">
      <value>
        <option name="FOREGROUND" value="7f0019" />
        <option name="BACKGROUND" value="f5f2e9" />
        <option name="EFFECT_COLOR" value="630000" />
        <option name="EFFECT_TYPE" value="1" />
      </value>
    </option>
    <option name="DEFAULT_SEMICOLON">
      <value>
        <option name="FOREGROUND" value="cc7832" />
      </value>
    </option>
    <option name="DIFF_DELETED">
      <value>
        <option name="BACKGROUND" value="d6d6d6" />
        <option name="ERROR_STRIPE_COLOR" value="cbcbcb" />
      </value>
    </option>
    <option name="DIFF_INSERTED">
      <value>
        <option name="BACKGROUND" value="c8f2c8" />
        <option name="ERROR_STRIPE_COLOR" value="baeeba" />
      </value>
    </option>
    <option name="DIFF_MODIFIED">
      <value>
        <option name="BACKGROUND" value="cad9fa" />
        <option name="ERROR_STRIPE_COLOR" value="bccff9" />
      </value>
    </option>
    <option name="EXECUTIONPOINT_ATTRIBUTES">
      <value>
        <option name="FOREGROUND" value="ffffff" />
        <option name="BACKGROUND" value="ff" />
        <option name="ERROR_STRIPE_COLOR" value="3763b0" />
      </value>
    </option>
    <option name="GENERIC_SERVER_ERROR_OR_WARNING">
      <value>
        <option name="EFFECT_COLOR" value="f49810" />
        <option name="ERROR_STRIPE_COLOR" value="f49810" />
        <option name="EFFECT_TYPE" value="2" />
      </value>
    </option>
    <option name="IDENTIFIER_UNDER_CARET_ATTRIBUTES">
      <value>
        <option name="BACKGROUND" value="e4e4ff" />
        <option name="ERROR_STRIPE_COLOR" value="ccccff" />
      </value>
    </option>
    <option name="INFO_ATTRIBUTES">
      <value>
        <option name="EFFECT_COLOR" value="cccccc" />
        <option name="ERROR_STRIPE_COLOR" value="ffffcc" />
        <option name="EFFECT_TYPE" value="2" />
      </value>
    </option>
    <option name="Instance property reference ID">
      <value>
        <option name="FOREGROUND" value="9876aa" />
      </value>
    </option>
    <option name="JAVA_COMMA">
      <value>
        <option name="FOREGROUND" value="cc7832" />
      </value>
    </option>
    <option name="JAVA_SEMICOLON">
      <value>
        <option name="FOREGROUND" value="cc7832" />
      </value>
    </option>
    <option name="List/map to object conversion">
      <value>
        <option name="FOREGROUND" value="ff" />
        <option name="BACKGROUND" value="cccccc" />
        <option name="FONT_TYPE" value="1" />
        <option name="EFFECT_TYPE" value="5" />
      </value>
    </option>
    <option name="Map key">
      <value>
        <option name="FOREGROUND" value="3300" />
        <option name="BACKGROUND" value="cccccc" />
        <option name="EFFECT_TYPE" value="5" />
      </value>
    </option>
    <option name="PROPERTIES.KEY_VALUE_SEPARATOR">
      <value>
        <option name="FOREGROUND" value="808080" />
      </value>
    </option>
    <option name="REGEXP.BRACES">
      <value>
        <option name="FOREGROUND" value="e8bf6a" />
      </value>
    </option>
    <option name="REGEXP.BRACKETS">
      <value>
        <option name="FOREGROUND" value="e8bf6a" />
      </value>
    </option>
    <option name="REGEXP.PARENTHS">
      <value>
        <option name="FOREGROUND" value="e8bf6a" />
      </value>
    </option>
    <option name="Static property reference ID">
      <value>
        <option name="FOREGROUND" value="d0d0ff" />
        <option name="FONT_TYPE" value="2" />
        <option name="EFFECT_COLOR" value="ffffff" />
        <option name="EFFECT_TYPE" value="1" />
      </value>
    </option>
    <option name="TEXT">
      <value>
        <option name="FOREGROUND" value="7f0019" />
        <option name="BACKGROUND" value="f5f2e9" />
        <option name="EFFECT_TYPE" value="1" />
      </value>
    </option>
    <option name="TEXT_SEARCH_RESULT_ATTRIBUTES">
      <value>
        <option name="BACKGROUND" value="ffff00" />
        <option name="ERROR_STRIPE_COLOR" value="ff00" />
      </value>
    </option>
    <option name="TODO_ATTRIBUTES">
      <value>
        <option name="FOREGROUND" value="ff" />
        <option name="FONT_TYPE" value="3" />
      </value>
    </option>
    <option name="TODO_DEFAULT_ATTRIBUTES">
      <value>
        <option name="FOREGROUND" value="ff" />
        <option name="FONT_TYPE" value="3" />
        <option name="ERROR_STRIPE_COLOR" value="ff" />
      </value>
    </option>
    <option name="TYPO">
      <value>
        <option name="EFFECT_COLOR" value="8000" />
        <option name="EFFECT_TYPE" value="2" />
      </value>
    </option>
    <option name="Unresolved reference access">
      <value>
        <option name="FOREGROUND" value="0" />
        <option name="BACKGROUND" value="cccccc" />
        <option name="EFFECT_COLOR" value="808080" />
        <option name="EFFECT_TYPE" value="1" />
      </value>
    </option>
    <option name="WRITE_IDENTIFIER_UNDER_CARET_ATTRIBUTES">
      <value>
        <option name="BACKGROUND" value="ffe4ff" />
        <option name="ERROR_STRIPE_COLOR" value="ffcdff" />
      </value>
    </option>
    <option name="YAML_SIGN">
      <value>
        <option name="FOREGROUND" value="a5c261" />
        <option name="EFFECT_TYPE" value="2" />
      </value>
    </option>
  </attributes>
</scheme>
```
