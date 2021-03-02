# Configuration de VSCode

## Configuration sans Python

```json
{
    // config générale
      "editor.suggestSelection": "first",
      "editor.rulers": [
        88,
        120
      ],
      "workbench.colorTheme": "One Dark Pro",
      "workbench.colorCustomizations": {
        "editorRuler.foreground": "#750917"
      },
      "editor.fontLigatures": true,
      "editor.fontFamily": "JetBrains Mono Medium",
      "editor.fontSize": 16,
      "terminal.integrated.cursorStyle": "line",
      "terminal.integrated.cursorWidth": 2,
      "terminal.integrated.fontFamily": "MesloLGS NF",
      "git.autofetch": true,
      "trailing-spaces.trimOnSave": true,
}
```

## Configuration avec Python

```json
{
  // config générale
    "editor.suggestSelection": "first",
    "editor.rulers": [
      88,
      120
    ],
    "workbench.colorTheme": "One Dark Pro",
    "workbench.colorCustomizations": {
      "editorRuler.foreground": "#750917"
    },
    "editor.fontLigatures": true,
    "editor.fontFamily": "JetBrains Mono Medium",
    "editor.fontSize": 16,
    "terminal.integrated.cursorStyle": "line",
    "terminal.integrated.cursorWidth": 2,
    "terminal.integrated.fontFamily": "MesloLGS NF",
    "git.autofetch": true,
    "trailing-spaces.trimOnSave": true,
  // config python
  "python.languageServer": "Pylance",
  "python.sortImports.path": "isort",
  "python.linting.flake8Path": "flake8",
  "python.linting.flake8Enabled": true,
  "python.linting.pylintEnabled": false,
  "python.linting.ignorePatterns": [
      ".vscode/*.py",
      "**/site-packages/**/*.py",
      ".venv/**/*.py",
      "**.pytest_cache/**/*.py"
    ],
  "python.formatting.provider": "black",
  "python.formatting.blackArgs": [
    "--line-length=88"
  ],
  "python.linting.mypyPath": "mypy",
  "python.linting.mypyEnabled": true,
  "python.testing.pytestEnabled" : true,
  "editor.formatOnSave": true,
  "editor.formatOnPaste": false,
  "editor.formatOnType": false,
  }
```