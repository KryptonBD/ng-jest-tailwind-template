# Angular + Jest + Tailwind CSS Template

After setting up the same Angular + Jest + Tailwind stack repeatedly across projects, I created this template to save time on configuration. Skip the setup and start coding immediately.

This template also maintains opinionated default (like naming suffixes) that the Angular team removed, but many developers still prefer for better code organization.

**From idea to development in seconds, not hours.**

## Architecture

This template combines three powerful technologies:

- **Angular 20**: Modern TypeScript framework with standalone components and zoneless change detection
- **Jest**: Fast JavaScript testing framework with jest-preset-angular
- **Tailwind CSS v4**: Latest utility-first CSS framework with PostCSS integration

### Key Features

- Standalone components architecture (no NgModules)
- Zoneless change detection for better performance
- Enforced naming suffixes (.component, .service, etc.) - maintained for better code organization despite Angular team removing them
- OnPush change detection strategy by default for better performance
- Jest testing with jest-preset-angular
- Tailwind CSS v4 with PostCSS configuration
- TypeScript 5.8 with strict mode
- Prettier formatting with Angular template support

### Project Structure

```
src/
├── app/
│   ├── core/
│   │   ├── interceptors/   # HTTP interceptors
│   │   └── services/       # Core application services
│   ├── features/           # Feature modules/components
│   ├── shared/
│   │   └── models/         # Shared TypeScript interfaces
│   ├── app.config.ts       # Application configuration
│   ├── app.routes.ts       # Route definitions
│   └── app.ts              # Root component
├── environments/           # Environment configurations
└── styles.scss             # Global styles with Tailwind imports
```

## Development server

To start a local development server, run:

```bash
ng serve
```

Once the server is running, open your browser and navigate to `http://localhost:4200/`. The application will automatically reload whenever you modify any of the source files.

## Code scaffolding

Angular CLI includes powerful code scaffolding tools. To generate a new component, run:

```bash
ng generate component component-name
```

For a complete list of available schematics (such as `components`, `directives`, or `pipes`), run:

```bash
ng generate --help
```

## Building

To build the project run:

```bash
ng build
```

This will compile your project and store the build artifacts in the `dist/` directory. By default, the production build optimizes your application for performance and speed.

## Running unit tests

This template uses Jest with jest-preset-angular for faster testing:

```bash
npm test
```

For watch mode:

```bash
npm run test:watch
```

For coverage:

```bash
npm run test:coverage
```

## Running end-to-end tests

For end-to-end (e2e) testing, run:

```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.
