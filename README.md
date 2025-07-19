# AngularEslintPrettyHusky

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 19.2.9.

## Getting Started

### Development Server

Start the local development server:

```bash
ng serve
```

Open your browser at [http://localhost:4200/](http://localhost:4200/). The app reloads automatically when you modify source files.

### Code Generation

Generate a new component:

```bash
ng generate component component-name
```

For more schematics (components, directives, pipes, etc.):

```bash
ng generate --help
```

### Building the Project

Build the project:

```bash
ng build
```

Build artifacts are stored in the `dist/` directory. Production builds are optimized for performance.

### Running Unit Tests

Run unit tests with [Karma](https://karma-runner.github.io):

```bash
ng test
```

### Running End-to-End Tests

Run end-to-end (e2e) tests:

```bash
ng e2e
```

> Note: Angular CLI does not include an e2e testing framework by default. Choose one that fits your requirements.

## Linting Setup

Install ESLint:

```bash
npm i eslint --save-dev
```

Run linting:

```bash
ng lint
```

> When prompted, confirm to add Angular lint support by typing `y` and pressing Enter.

## Prettier Integration

Install Prettier and its ESLint plugins:

```bash
npm i --save-dev prettier eslint-config-prettier eslint-plugin-prettier
```

Add Prettier configuration (optional):

```json
// .prettierrc
{
  "singleQuote": true,
  "semi": true
}
```

Update your ESLint config to include Prettier (see `eslint.config.js`):

```javascript
// ...existing code...
extends: [
  // other configs,
  eslintConfigPrettier,
],
plugins: {
  prettier: prettier,
},
rules: {
  // other rules,
  "prettier/prettier": "error"
}
// ...existing code...
```

## Checking and Formatting Code

Check formatting for all files (including untracked):

```bash
npx prettier --check .
```

Format all files:

```bash
npx prettier --write .
```

## TypeScript Configuration

The `lib` property is added in `tsconfig.json`:

```jsonc
"lib": ["ES2022", "DOM"]
```

This enables modern JavaScript features and browser APIs in your Angular project.

## Resources

- [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli)
- [Prettier Documentation](https://prettier.io/docs/en/index.html)
- [ESLint Documentation](https://eslint.org/docs/latest/)