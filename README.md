# HotelApp

A responsive Angular frontend for a hotel application. This project was generated with the Angular CLI and uses Bootstrap for styling.

Current stack (from package.json)
- Angular ^16.1.0
- Bootstrap 5.3
- TypeScript ~5.1
- Test tools: Karma + Jasmine

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Getting started](#getting-started)
- [Development server](#development-server)
- [Build](#build)
- [Testing](#testing)
- [Project structure](#project-structure)
- [Generating components/services](#generating-componentsservices)
- [Styling](#styling)
- [Environment configuration](#environment-configuration)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- Angular-based single-page application
- Responsive layout using Bootstrap
- Ready for component-based development and routing
- Unit testing scaffolded with Karma and Jasmine

## Prerequisites

- Node.js 18+ (or compatible version for Angular 16)
- npm (recommended) or yarn
- Angular CLI (optional, for local global usage)
  - Install with: `npm install -g @angular/cli@~16.1.6`

## Getting started

1. Clone the repository:
   ```bash
   git clone https://github.com/codesbydeen/hotel-app.git
   cd hotel-app
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   # yarn
   ```

## Development server

Run the development server (live reload):
```bash
npm start
# or
ng serve
```

Open your browser to http://localhost:4200/. The app will automatically reload when you change source files.

## Build

Build the project for production:
```bash
npm run build
# or
ng build --configuration production
```

Build outputs are placed in the `dist/` directory.

There's also a watch mode useful for local development:
```bash
npm run watch
# runs: ng build --watch --configuration development
```

## Testing

Run unit tests with Karma:
```bash
npm test
# runs: ng test
```

End-to-end tests are not included by default. To add e2e tests, install a test runner (e.g., Cypress) or configure Protractor/Playwright and add scripts to package.json.

## Project structure (typical)

- src/
  - app/              # Angular app modules, components, services
  - assets/           # Images, static assets
  - environments/     # Environment-specific configuration files
  - index.html
  - main.ts
- e2e/                # (if added) end-to-end test setup
- angular.json
- package.json

Note: This repository was scaffolded with Angular CLI. The structure follows standard Angular app conventions.

## Generating components/services

Use the Angular CLI to generate files:
```bash
ng generate component components/my-component
ng generate service services/my-service
```
Or the shorthand:
```bash
ng g c my-component
ng g s my-service
```

## Styling

Bootstrap is included as a dependency (Bootstrap 5.3). To customise Bootstrap or include additional CSS, edit `styles` in `angular.json` or import CSS in `src/styles.scss` / `src/styles.css`.

## Environment configuration

Use the `src/environments/` folder for environment-specific variables (e.g., API endpoints). By default, Angular CLI will swap `environment.ts` with `environment.prod.ts` when building for production.

Example usage:
```ts
import { environment } from '../environments/environment';
const apiUrl = environment.apiBaseUrl;
```

## Contributing

- Fork the repo and open a pull request with descriptive changes.
- Follow Angular style guidelines for structure and naming.
- Add or update unit tests for new logic where applicable.

If you'd like a CONTRIBUTING.md or issue templates, I can add those.

## License

Add your license here (e.g., MIT). Example:
```
MIT License
```

## Contact

Maintainer: codesbydeen (GitHub)

---

If you'd like, I can:
- Commit this README.md to `master` (or another branch) for you, or
- Create a more detailed README that documents specific app screens, API contracts, and example screenshots — tell me which you'd prefer.
