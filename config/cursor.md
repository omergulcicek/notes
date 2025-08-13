## Cursor Rules

```bash
Communicate in Turkish, but write all code in English.

Avoid using the any type in TypeScript. Place all type definitions in the appropriate files under the src/types directory, or create a new file if needed. Types must not be defined inside component files. All type names should have the word Type at the end (e.g., MenuType, UserType).

Hook names should start with use.

File and folder names must use kebab-case, and all naming should be in English. Component names should use PascalCase, except for certain UI components where different conventions may apply.

Functions should follow the Single Responsibility Principle, keeping them short and focused.

Add comments only when absolutely necessary.

Remove unnecessary imports before each commit.

Remove all console.log statements after debugging is complete.

Commit messages should follow the conventional commits format (feat:, fix:, chore:, etc.).

Prefer pastel and soft color tones in the design.

Avoid code duplication by collecting shared logic in the utils directory.

Always handle errors in API calls using try/catch, toast, or similar patterns.

Follow accessibility (a11y) standards, include appropriate aria attributes where necessary, and wrap all images within semantic <figure> elements for proper context and captions.

UI components should be reusable and modular.

Do not use inline styles; use Tailwind CSS exclusively for styling.
```

## Cursor settings.json

```json
{
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode",
        "editor.formatOnSave": true
    },
    "[javascriptreact]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode",
        "editor.formatOnSave": true
    },
    "[typescript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode",
        "editor.formatOnSave": true
    },
    "[typescriptreact]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode",
        "editor.formatOnSave": true
    },
    "explorer.compactFolders": false,
    "bracketPairColorizer.depreciation-notice": true,
    "breadcrumbs.enabled": true,
    "debug.console.fontSize": 14,
    "editor.accessibilitySupport": "off",
    "editor.cursorBlinking": "solid",
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.fontFamily": "Fira Code",
    "editor.fontLigatures": true,
    "editor.fontSize": 14,
    "editor.formatOnSave": false,
    "editor.hover.enabled": true,
    "editor.inlineSuggest.enabled": true,
    "editor.tabSize": 2,
    "editor.useTabStops": false,
    "explorer.confirmDelete": false,
    "explorer.confirmDragAndDrop": false,
    "files.exclude": {
        "**/.cache": true,
        "**/.next": true,
        "**/.parcel-cache": true,
        "**/build": true,
        "**/dist": true,
        "**/node_modules": true
    },
    "git.autofetch": true,
    "github.copilot.enable": {
        "*": true,
        "markdown": true,
        "plaintext": true,
        "yaml": true
    },
    "javascript.updateImportsOnFileMove.enabled": "never",
    "screencastMode.verticalOffset": 0,
    "search.searchOnType": false,
    "svelte.enable-ts-plugin": true,
    "terminal.external.osxExec": "iTerm.app",
    "terminal.integrated.fontFamily": "'SpaceMono NF'",
    "terminal.integrated.fontSize": 14,
    "typescript.updateImportsOnFileMove.enabled": "always",
    "window.zoomLevel": 1,
    "workbench.colorTheme": "Bearded Theme Black & Gold",
    "workbench.editor.decorations.badges": true,
    "workbench.editor.decorations.colors": true,
    "workbench.iconTheme": "vscode-icons",
    "workbench.sideBar.location": "right",
    "terminal.integrated.env.osx": {
        "FIG_NEW_SESSION": "1"
    },
    "git.confirmSync": false,
    "explorer.confirmPasteNative": false,
    "workbench.startupEditor": "none",
    "git.suggestSmartCommit": false,
    "github.copilot.editor.enableAutoCompletions": true,
    "vsicons.dontShowNewVersionMessage": true,
    "diffEditor.ignoreTrimWhitespace": true,
    "git.ignoreRebaseWarning": true,
    "security.workspace.trust.untrustedFiles": "open"
}
```
