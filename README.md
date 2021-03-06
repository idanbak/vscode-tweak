# vscode-tweak
Collection of extension, settings, and tips for Visual Studio Code

## Extensions / Plugins
List of useful extension or plugins in Visual Studio Code:

**(1) Main**

| Extensions | Description|
|:--------|:-----------------|
| [GitLens: Git supercharged](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) | Visualize code authorship at a glance via Git blame annotations and code lens, seamlessly navigate and explore Git repositories, gain valuable insights via powerful comparison commands, and so much more |
| [Bookmarks](https://marketplace.visualstudio.com/items?itemName=alefragnani.Bookmarksc) | Mark lines and jump to them |
| [Project Manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager) | Easily switch between projects |
| [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) | Run code snippet or code file for multiple languages: C, C++, Java, JavaScript, PHP, Python, Perl, Perl 6, Ruby, Go, Lua, Groovy, PowerShell, BAT/CMD, BASH/SH, F# Script, F# (.NET Core), C# Script, C# (.NET Core), VBScript, TypeScript, CoffeeScript, Scala, Swift, Julia, Crystal, OCaml Script, R, AppleScript, Elixir, Visual Basic .NET, Clojure, Haxe, Objective-C, Rust, Racket, AutoHotkey, AutoIt, Kotlin, Dart, Free Pascal, Haskell, Nim, D, and custom command |
| [VS Live Share](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare) | Real-time collaborative development from the comfort of your favorite tools. |


**(2) Misc**


| Extensions | Description|
|:--------|:-----------------|
| [COBOL](https://marketplace.visualstudio.com/items?itemName=bitlang.cobol) | COBOL, JCL, PL/I & DIR syntax support |
| [Java Extension Pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack) | Language Support for Java™ by Red Hat, Debugger for Java, Java Test Runner, and Maven Project Explorer |
| [Bracket Pair Colorizer 2](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer-2c) | A customizable extension for colorizing matching brackets |
| [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme) | Material Design Icons for Visual Studio Code |
| [Rainbow CSV](https://marketplace.visualstudio.com/items?itemName=mechatroner.rainbow-csv) | Highlight columns in comma (.csv), tab (.tsv), semicolon and pipe - separated files in different colors. |
| [Instant Markdown](https://marketplace.visualstudio.com/items?itemName=dbankier.vscode-instant-markdown) | Instant previews of your markdown files as you type. |



---
## Useful Shortcut

| Shortcut | Usage|
|:--------|:-----------------|
| `Ctrl` + `P` | Open any file / component |
| `Ctrl` + `+` | Zoom in |
| `Ctrl` + `-` | Zoom out |
| `Ctrl` + `Alt` + `Up` | Multi cursor selection |
| `Ctrl` + `Alt` + `Down` | Multi cursor selection |
| `Ctrl` + `\` | Side by side editing |
| `Ctrl` + `K` then `Ctrl` + `X` | Trim trailing whitespace |
| `Ctrl` + `Shift` + `P` | Open Setting / Preference |
| `Alt` + `Left` | Go to last cursor (go back) |
| `Alt` + `Right` | Go to last cursor (forward) |
| `F12` | Go to definition |
| `Alt` + `F12` | Simply peek at the definition, which shows you the definition right in line where your cursor is rather than opening up the source file.|

See [Windows shortcut](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf) for complete list,
or [VS Tips and Tricks](https://code.visualstudio.com/docs/getstarted/tips-and-tricks) for more inspiration.

---
## User Settings

Go to *File* > *Preference*, or
Press `Ctrl` + `Shift` + `P` and type `User Setting`. On right side, choose *Open settings.json* on `...` buttons.
Type below example settings for COBOL developer:

```javascript
{
    "window.title": "${dirty}${activeEditorLong}${separator}${rootName}",
    "breadcrumbs.enabled": true,
    "editor.renderControlCharacters": true,
    "editor.renderWhitespace": "all",
    "window.zoomLevel": 1,
    "terminal.integrated.shell.windows": "C:\\Program Files\\Git\\bin\\bash.exe",
    "terminal.integrated.shellArgs.windows": [
        "-l"
      ],
    "[COBOL]": {
      "files.autoGuessEncoding": true,
      "editor.rulers": [
        6,
        7,
        11,
        42,
        72,
        80
      ],
      "editor.detectIndentation": false,
      "editor.wordSeparators": "`~!#$%^&*()=+[{]}\\|;:'\",.<>/?",
      "editor.copyWithSyntaxHighlighting": false
    },
}
```

---
## Terminal
Integrate **Git Bash** in Visual Studio Terminal by adding below setting (later this setting also useful when adding command/git alias):

```javascript
{
    "terminal.integrated.shell.windows": "C:\\Program Files\\Git\\bin\\bash.exe",
    "terminal.integrated.shellArgs.windows": [
        "-l"
      ]
}
```

Open your terminal using shortcut `Ctrl` + ` ` `

---

