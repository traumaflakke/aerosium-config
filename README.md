# @aerosium/config

Modern ESLint and Prettier configuration for Next.js and React projects with TypeScript support. This package provides a ready-to-use set of rules for maintaining high code quality and consistent style across all projects.

## Features

### ✨ Key Benefits

- **Ready-made Next.js Configuration** - optimized rules for working with Next.js 14+
- **Modern Standards Support** - uses the new ESLint flat config structure
- **TypeScript Out of the Box** - full TypeScript support with strict rules
- **Performance Optimization** - rules for Core Web Vitals and optimization
- **Accessibility (A11Y)** - built-in rules for ensuring accessibility
- **Consistent Code Style** - Prettier integration for unified formatting
- **Automatic Import Sorting** - maintaining order in imports
- **File Naming** - rules for consistent file naming

### 🎯 What's Included

- Next.js and React rules
- TypeScript configuration
- Accessibility rules (jsx-a11y)
- Import sorting
- Prettier integration
- Unicorn rules for modern JavaScript
- Strict TypeScript rules

## Installation

```bash
# Using yarn
yarn add -D @aerosium/config

# Install peer dependencies
yarn add -D @eslint/eslintrc @eslint/js @next/eslint-plugin-next @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react eslint-plugin-react-hooks eslint-plugin-unicorn prettier typescript eslint-config-next eslint-import-resolver-typescriptы
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

Add these settings to your VS Code workspace:

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

## Benefits

1. **Unified Code Style**
   - Automatic formatting with Prettier
   - Consistent rules across all projects
   - Import and props sorting

2. **Code Quality Improvement**
   - Prevention of common mistakes
   - Following React and Next.js best practices
   - Strict typing with TypeScript

3. **Performance**
   - Core Web Vitals optimization rules
   - Prevention of unnecessary re-renders
   - Image and font optimization

4. **Accessibility**
   - Built-in a11y rules
   - ARIA attributes validation
   - Semantic validation

5. **Modern Standards**
   - Support for new ESLint flat config structure
   - Compatibility with latest Next.js versions
   - Rules for modern JavaScript

## Limitations and Considerations

1. **Strict Rules**
   - Some rules might seem too strict
   - Team adaptation time might be needed
   - May need to disable some rules for legacy code

2. **Dependencies**
   - Large number of peer dependencies
   - Need to maintain up-to-date versions
   - Possible version conflicts in large projects

3. **Performance**
   - ESLint with many rules might work slower
   - Might need to configure ignored files/folders
   - ESLint cache recommended for large projects

## Usage Recommendations

1. **Gradual Implementation**
   - Implement rules gradually in existing projects
   - Use `eslint --fix` for automatic fixes
   - Start with formatting, then add stricter rules

2. **Project-specific Setup**
   - Disable rules that don't fit your project
   - Configure ignored files and folders
   - Adapt configuration to project specifics

3. **Process Optimization**
   - Set up pre-commit hooks
   - Use ESLint and Prettier in CI/CD
   - Regularly update dependencies

## License

MIT
