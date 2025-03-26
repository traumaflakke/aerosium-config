# @aerosium/config

Shared ESLint and Prettier configurations for Aerosium projects.

## Installation

```bash
# Using yarn
yarn add -D @aerosium/config

# Install peer dependencies
yarn add -D @next/eslint-plugin-next @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react eslint-plugin-react-hooks eslint-plugin-unicorn prettier typescript
```

## Usage

### ESLint Configuration

Create `eslint.config.mjs` in your project root:

```javascript
import aerosiumConfig from '@aerosium/config/eslint'

export default aerosiumConfig
```

### Prettier Configuration

Create `.prettierrc` in your project root:

```json
"@aerosium/config/prettier"
```

### VS Code Settings

Add these settings to your VS Code workspace settings:

```json
{
  "editor.formatOnSave": true,
  "editor.formatOnPaste": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.codeActionsOnSave": {
    "source.fixAll": "always",
    "source.organizeImports": "explicit",
    "source.fixAll.eslint": "always"
  },
  "prettier.arrowParens": "avoid"
}
```

## Features

- Next.js and React optimized configuration
- TypeScript support
- Modern ESLint rules
- Consistent code style with Prettier
- Accessibility rules (jsx-a11y)
- Import sorting and organization
- Strict TypeScript checks
- File naming conventions

## License

MIT
