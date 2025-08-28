## Cursor Rules

```bash
## General Rules
- Communicate in Turkish, but write all code in English.
- Add comments only when absolutely necessary.
- Remove unnecessary imports before each commit.
- Remove all console.log statements after debugging is complete.
- Commit messages must be written in English and must follow the conventional commits format (feat:, fix:, refactor:, etc.).
- Always add clear JSDoc comments for helper and utility functions, including a short description, @param tags for all parameters, and @returns if applicable, without redundant type annotations or extra sections.

## TypeScript Rules
- Avoid using the any type in TypeScript.
- Place all type definitions in the src/types directory, or create a new file if needed.
- Types must not be defined inside component files.
- Prefer using interface for object shapes, and type for unions or advanced type compositions.
- All type names must end with the word Type (e.g., MenuType, UserType).
- Type file names must end with the word `.type.ts` (e.g., menu.type.ts, user-list.type.ts).

## Functions & Hooks
- Hook names must start with use.
- Functions should follow the Single Responsibility Principle, keeping them short and focused.
- Inside components, always declare hooks and contexts first, then variables, and finally state definitions.

## Naming Conventions
- File and folder names must use kebab-case, and all naming should be in English.
- Component names must use PascalCase, except for certain UI components where different conventions may apply.
- Variable declarations and file names must use kebab-case.

## Components & Structure
- Every subfolder and file inside the components directory must contain an index.ts file (e.g., components/ui/index.ts, components/widgets/index.ts).
- Components inside the components/widgets directory must be named using PascalCase (e.g., components/widgets/User/User.tsx).
- Each component folder must contain an index.ts file exporting the component (e.g., export * from "./User";).
- UI components must be reusable and modular.
- Prop and variable naming must be intent-driven (e.g., onSubmit, isLoading, variant).

## Utilities
- If a function is generic and reusable across the project, place it under src/utils; if it performs a computation or is domain-specific, place it under src/helpers, and in both cases name the file in kebab-case (e.g., format-currency.ts, calculate-tax.ts).
- Constants must be placed under src/constants and must not be kept inside components.

## Styling & Design
- Do not use inline styles; use Tailwind CSS exclusively for styling.
- Prefer pastel and soft color tones in the design.

## Error Handling
- Always handle errors in API calls using try/catch, toast, or similar patterns.

## Accessibility (a11y)
- Follow accessibility (a11y) standards.
- Include appropriate aria attributes where necessary.
- Wrap all images within semantic <figure> elements for proper context and captions.
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
