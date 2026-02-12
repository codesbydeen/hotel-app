# HotelApp

A responsive Angular frontend for a hotel application. This project was generated with the Angular CLI and uses Bootstrap for styling. [Project is currently still being updated]

Current stack (from package.json)
- Angular ^16.1.0
- Bootstrap 5.3
- TypeScript ~5.1
- Test tools: Karma + Jasmine

## Table of Contents

- [Features](#features)
- [API Integration](#api-integration)
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
- Integrated with a backend API to fetch, create, update and delete hotel data (CRUD)

## API Integration

This application is designed to work with a backend API (RESTful or similar). The frontend performs the following operations against the API:

- Fetch data (GET) — retrieve lists and individual resources (e.g., hotels, rooms, bookings)
- Create data (POST) — add new resources
- Update data (PUT/PATCH) — modify existing resources
- Delete data (DELETE) — remove resources

Notes:
- The API base URL is configurable via the Angular environment files (see [Environment configuration](#environment-configuration)).
- The UI uses Angular's HttpClient within services to communicate with the API.
- Authentication, headers, and exact endpoint paths are provided by the backend; the frontend expects endpoints for the resource types used by the app (examples below).

Example environment entry (placeholder):
```ts
// src/environments/environment.ts
export const environment = {
  production: false,
  apiBaseUrl: 'https://api.example.com' // change to your API URL
};
