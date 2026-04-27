# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [v0.1.0] - 2026-04-27

### Added

- Initial project structure with Nuxt 3 framework
- Core directory organization:
  - `app/` - Application root with Vue entry point
  - `components/` - Component directories (account, base, casino, common, sportsbook)
  - `composables/` - Vue composables (account, casino, core, sportsbook)
  - `layouts/` - Page layouts (auth, default, sportsbook)
  - `middleware/` - Route middleware (auth, guest, kyc, responsible-gaming)
  - `plugins/` - Nuxt plugins (analytics, api, i18n, socket)
  - `server/` - Server-side API routes and utilities
  - `services/` - Business logic services
  - `stores/` - Pinia state management stores
  - `types/` - TypeScript type definitions
  - `utils/` - Utility functions (constants, formatters, validators)
- Configuration files:
  - `nuxt.config.ts` - Nuxt configuration with @nuxt/ui and @pinia/nuxt modules
  - `tsconfig.json` - TypeScript configuration
  - `.gitignore` - Git ignore patterns
- Internationalization setup with i18n support (English, Spanish)
- Sportsbook module with event and sport pages
- Placeholder files for core composables (useApi, useAuth, useWebSocket)
- Placeholder service files (api.client, auth, wallet, casino, sportsbook, promotions)
- Placeholder type definitions (wallet, casino, sportsbook)
- Test directories structure (e2e, unit)
- Shared constants and schemas directories