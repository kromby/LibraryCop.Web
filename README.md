# LibraryCop Web

A SvelteKit landing page and admin surface for Bókasapp, a library management system for small libraries in Iceland. Deployed to Azure Static Web Apps, it serves as both a marketing surface and a foundation for future admin features.

> **Status:** Portfolio piece. Maintained as a CV and EMBA showcase, not as production software.

## Tech Stack

- SvelteKit 1.x with Svelte 3.x
- Vite 4.x build system
- Azure Static Web Apps deployment (`svelte-adapter-azure-swa`)
- Playwright for E2E testing
- Vitest for unit testing
- TypeScript for type safety

## Architecture

This is the web layer of the Bókasapp system. It provides a public landing page and admin interface, backed by the [Backend API](https://github.com/kromby/LibraryCop.Backend). For the full system architecture, see the backend repository.

## Related Repositories

- [Backend](https://github.com/kromby/LibraryCop.Backend) - C# .NET 6 REST API on Azure Functions
- [Frontend](https://github.com/kromby/LibraryCop.Frontend) - Flutter cross-platform mobile app

## Local Development

### Prerequisites

- [Node.js](https://nodejs.org/) 16+ with npm
- [Playwright](https://playwright.dev/) (for E2E tests)

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/kromby/LibraryCop.Web
   cd LibraryCop.Web
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```
   The app will be available at `http://localhost:5173`.

4. Run unit tests:
   ```bash
   npm run test:unit
   ```

5. Run E2E tests (requires the dev server running):
   ```bash
   npm run test
   ```

6. Build for production:
   ```bash
   npm run build
   ```

7. Preview the production build:
   ```bash
   npm run preview
   ```

## Key Features

- **Modern SvelteKit framework**: Performant, lightweight UI with Vite-powered fast builds
- **Azure Static Web Apps integration**: Serverless deployment with CDN, branch previews, and auto-scaling
- **TypeScript support**: Type-safe development out of the box
- **Comprehensive testing**: E2E tests with Playwright and unit tests with Vitest
- **Landing page**: SEO-friendly public surface for the Bókasapp project

## Known Limitations and Tradeoffs

- **Minimal features**: The web app is primarily a landing page and portfolio surface. Conversion features and user dashboards are out of scope.
- **Hardcoded Icelandic UI**: All content is in Icelandic. Production would adopt `sveltekit-i18n` or similar for multi-language support.
- **No admin workflows**: Admin features for kindergarten management are not yet implemented. Production would include role-based access control and full CRUD interfaces.
- **No backend integration yet**: The landing page is static. Production would integrate with the backend API for dynamic content and real-time data.
- **Limited test coverage**: Tests focus on critical workflows. Full coverage would be required for production code.

## Privacy and Data

This is a portfolio project. No real user data is collected or stored. Firebase analytics (if enabled) is used for development and debugging purposes only.

## License

MIT License. Copyright (c) 2023 Guðjón Karl.

## Contact

Questions or feedback? Reach out at gudjon@noona.app.
