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
- [Default Profile](https://github.com/orue/my-vscode-settings/blob/master/vscode-extensions-default.list) (Base profile with all the common extensions and setting).
- Python Profile.
- JavaScript Profile.

### Extensions

#### Default Profile Extensions.

```
aaron-bond.better-comments
amazonwebservices.codewhisperer-for-command-line-companion
arcticicestudio.nord-visual-studio-code
bierner.markdown-preview-github-styles
brittanychiang.halcyon-vscode
christian-kohler.path-intellisense
codezombiech.gitignore
github.copilot
github.copilot-chat
github.vscode-pull-request-github
hackrio.hackr-theme
mechatroner.rainbow-csv
mhutchie.git-graph
miguelsolorio.fluent-icons
miguelsolorio.symbols
mikestead.dotenv
monokai.theme-monokai-pro-vscode
ms-azuretools.vscode-docker
redhat.vscode-xml
redhat.vscode-yaml
streetsidesoftware.code-spell-checker
tamasfe.even-better-toml
visualstudioexptteam.intellicode-api-usage-examples
yzhang.markdown-all-in-one
```
You can export all the extensions to a .list file with the following comman:
```sh
code --list-extensions --profile profileName > vscode-extensions-profileName.list
```
And can install all the extension with the following command:
```sh
cat vscode-extensions-profileName.list | xargs -L 1 code --install-extension --profile profileName
```
Also check and setup [Settings Sync](https://code.visualstudio.com/docs/editor/settings-sync)
### Settings
#### Default Profile Settings
```json
{
  "workbench.productIconTheme": "fluent-icons",
  "workbench.iconTheme": "symbols",
  "workbench.startupEditor": "none",
  "workbench.editor.enablePreview": false,
  "workbench.editor.highlightModifiedTabs": true,
  "workbench.tree.renderIndentGuides": "always",
  "workbench.tree.indent": 14,
  "workbench.layoutControl.enabled": false,
  "workbench.settings.editor": "json",
  "workbench.editor.showTabs": "none",
  "workbench.statusBar.visible": false,
  "workbench.sideBar.location": "right",
  "workbench.editor.labelFormat": "medium",
  "window.zoomLevel": 0.52,
  "window.commandCenter": false,
  "window.newWindowProfile": "Default",
  "breadcrumbs.enabled": false,
  "extensions.ignoreRecommendations": true,
  "security.workspace.trust.enabled": false,
  "editor.fontFamily": "MonoLisa",
  "editor.fontLigatures": true,
  "editor.fontSize": 14,
  "editor.tabSize": 2,
  "editor.wordWrap": "on",
  "editor.wordWrapColumn": 120,
  "editor.cursorBlinking": "phase",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.multiCursorModifier": "ctrlCmd",
  "editor.snippetSuggestions": "top",
  "editor.tabCompletion": "on",
  "editor.accessibilitySupport": "off",
  "editor.minimap.enabled": false,
  "editor.linkedEditing": true,
  "editor.renderLineHighlight": "none",
  "editor.renderWhitespace": "none",
  "diffEditor.ignoreTrimWhitespace": false,
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
  "terminal.integrated.defaultProfile.osx": "zsh",
  "terminal.integrated.sendKeybindingsToShell": true,
  "terminal.integrated.fontFamily": "'Cascadia Mono NF'",
  "terminal.integrated.fontSize": 14,
  "terminal.integrated.lineHeight": 1.2,
  "terminal.integrated.cursorStyle": "line",
  "terminal.integrated.env.osx": {
    "Q_NEW_SESSION": "1"
  },
  "github.copilot.enable": {
    "*": true,
    "plaintext": false,
    "markdown": false,
    "scminput": false,
    "gitignore": false,
    "properties": false
  },
}


```

Special thanks to CJ on [Syntax](https://youtu.be/GK7zLYAXdDs?si=Nx83M424yKx67fs9), I follow some of his ideas for setting up my default VS Code Profile.
