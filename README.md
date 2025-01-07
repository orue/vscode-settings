# VS Code Settings

### Themes
- [Halcyon](https://marketplace.visualstudio.com/items?itemName=brittanychiang.halcyon-vscode) - my favorite
- [Nord](https://marketplace.visualstudio.com/items?itemName=arcticicestudio.nord-visual-studio-code)
- [Monokai Pro](https://marketplace.visualstudio.com/items?itemName=monokai.theme-monokai-pro-vscode) (Paid)

### Icons
- File Icons
  - [Symbols](https://marketplace.visualstudio.com/items?itemName=miguelsolorio.symbols)
- Product Icons
  - [Fluent Icons](https://marketplace.visualstudio.com/items?itemName=miguelsolorio.fluent-icons)
### Fonts
- [MonoLisa](https://www.monolisa.dev/) (Paid) - my favorite
- [Cascadia Code](https://github.com/microsoft/cascadia-code)
- [JetBrains Mono](https://www.jetbrains.com/lp/mono/)
- [Dank Mono](https://philpl.gumroad.com/l/dank-mono) (Paid)

---
### Profiles
I'm using [VS Code Profiles](https://code.visualstudio.com/docs/editor/profiles) for different development environment:
- Default Profile (Base profile with all the common extensions and setting).
- Python Profile.
- JavaScript Profile.

### Extensions

#### Default Profile Extensions.

```
aaron-bond.better-comments
amazonwebservices.codewhisperer-for-command-line-companion
bierner.markdown-preview-github-styles
christian-kohler.path-intellisense
codezombiech.gitignore
foxundermoon.shell-format
github.copilot
github.copilot-chat
github.vscode-pull-request-github
mechatroner.rainbow-csv
mikestead.dotenv
redhat.vscode-xml
redhat.vscode-yaml
streetsidesoftware.code-spell-checker
sumneko.lua
tamasfe.even-better-toml
yzhang.markdown-all-in-one

```
You can export all the extensions to a .list file with the following comman:
```sh
code --list-extensions --profile profileName > vscode-extensions-profileName.list
```
And can install all the extension with the following command:
```sh
cat vscode-extensions-profileName.list | xargs -L 1 code --profile profileName --install-extension

```
Also check and setup [Settings Sync](https://code.visualstudio.com/docs/editor/settings-sync)
### Settings
#### Default Profile Settings
```json
{
  // * Workbench ==============================================================
  "workbench.startupEditor": "none",
  "workbench.editor.enablePreview": false,
  "workbench.editor.highlightModifiedTabs": true,
  "workbench.tree.renderIndentGuides": "always",
  "workbench.tree.indent": 16,
  "workbench.layoutControl.enabled": false,
  "workbench.settings.editor": "json",
  "workbench.editor.showTabs": "none",
  "workbench.sideBar.location": "right",
  "workbench.editor.labelFormat": "medium",
  "workbench.editorAssociations": {
    "*.md": "vscode.markdown.preview.editor"
  },
  "window.zoomLevel": 0.35,
  "window.commandCenter": false,
  "window.newWindowProfile": "Default",
  "breadcrumbs.enabled": false,
  "extensions.ignoreRecommendations": true,
  "security.workspace.trust.enabled": false,
  // * Editor =================================================================
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontLigatures": true,
  "editor.fontSize": 14,
  "editor.tabSize": 2,
  "editor.wordWrap": "on",
  "editor.wordWrapColumn": 120,
  "editor.cursorBlinking": "phase",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.multiCursorModifier": "ctrlCmd",
  "editor.autoIndent": "full",
  "editor.snippetSuggestions": "top",
  "editor.tabCompletion": "on",
  "editor.accessibilitySupport": "off",
  "editor.minimap.enabled": false,
  "editor.linkedEditing": true,
  "editor.stickyScroll.enabled": true,
  "editor.renderLineHighlight": "none",
  "editor.renderWhitespace": "none",
  "editor.formatOnSave": true,
  "editor.formatOnPaste": true,
  "editor.codeActionsOnSave": {
    "source.fixAll": "explicit",
    "source.organizeImports": "explicit"
  },
  "editor.rulers": [
    120
  ],
  "files.trimFinalNewlines": true,
  "files.insertFinalNewline": true,
  "files.trimTrailingWhitespace": true,
  "files.defaultLanguage": "markdown",
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  "explorer.compactFolders": false,
  "markdown.validate.enabled": true,
  // * Formatter ==============================================================
  "[javascript]": {
    "editor.defaultFormatter": "vscode.typescript-language-features"
  },
  "[typescript]": {
    "editor.defaultFormatter": "vscode.typescript-language-features"
  },
  "[html]": {
    "editor.defaultFormatter": "vscode.html-language-features"
  },
  "[css]": {
    "editor.defaultFormatter": "vscode.css-language-features"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "vscode.json-language-features"
  },
  // * Terminal Settings ======================================================
  "terminal.integrated.defaultProfile.osx": "zsh",
  "terminal.integrated.sendKeybindingsToShell": true,
  "terminal.integrated.fontFamily": "'JetBrains Mono','FiraMono Nerd Font Propo'",
  "terminal.integrated.fontSize": 14,
  "terminal.integrated.fontWeightBold": "normal",
  "terminal.integrated.lineHeight": 1.2,
  "terminal.integrated.cursorStyle": "line",
  "terminal.integrated.env.osx": {
    "Q_NEW_SESSION": "1"
  },
  // * Git ====================================================================
  "git.autofetch": true,
  "git.confirmSync": false,
  "git.enableSmartCommit": true,
  "git.showActionButton": {
    "commit": false,
    "publish": false,
    "sync": false
  },
  // * Copilot ================================================================
  "github.copilot.enable": {
    "*": true,
    "plaintext": false,
    "markdown": false,
    "scminput": false,
    "gitignore": false,
    "properties": false
  },
  "telemetry.telemetryLevel": "off",
  "workbench.settings.applyToAllProfiles": [
    "terminal.integrated.defaultProfile.osx",
    "terminal.integrated.sendKeybindingsToShell",
    "terminal.integrated.fontFamily",
    "terminal.integrated.fontSize",
    "terminal.integrated.fontWeightBold",
    "terminal.integrated.lineHeight",
    "terminal.integrated.cursorStyle",
    "terminal.integrated.env.osx",
    "workbench.startupEditor",
    "workbench.editor.enablePreview",
    "workbench.editor.highlightModifiedTabs",
    "workbench.tree.renderIndentGuides",
    "workbench.tree.indent",
    "workbench.layoutControl.enabled",
    "workbench.settings.editor",
    "extensions.ignoreRecommendations",
    "workbench.sideBar.location",
    "window.zoomLevel",
    "window.commandCenter",
    "breadcrumbs.enabled",
    "editor.wordWrap",
    "editor.wordWrapColumn",
    "editor.cursorBlinking",
    "editor.cursorSmoothCaretAnimation",
    "editor.multiCursorModifier",
    "editor.autoIndent",
    "editor.snippetSuggestions",
    "editor.tabCompletion",
    "editor.accessibilitySupport",
    "editor.minimap.enabled",
    "editor.linkedEditing",
    "editor.renderLineHighlight",
    "editor.renderWhitespace",
    "editor.bracketPairColorization.enabled",
    "editor.rulers",
    "files.trimFinalNewlines",
    "files.insertFinalNewline",
    "files.trimTrailingWhitespace",
    "files.defaultLanguage",
    "explorer.confirmDragAndDrop",
    "explorer.confirmDelete",
    "explorer.compactFolders",
    "git.autofetch",
    "git.confirmSync",
    "git.showActionButton",
    "git.enableSmartCommit",
    "workbench.editor.labelFormat"
  ]
}

```

Special thanks to CJ on [Syntax](https://youtu.be/GK7zLYAXdDs?si=Nx83M424yKx67fs9), I follow some of his ideas for setting up my default VS Code Profile.
