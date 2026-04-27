# casino-web-front

A modern web frontend for a casino platform built with Nuxt 4, featuring casino games, sportsbook, wallet management, and internationalization support.

## Prerequisites

- **Node.js**: `>=18.0.0`
- **npm**: `>=9.0.0`

## Installation

```bash
# Clone the repository
git clone <repository-url>
cd casino-web-front

# Install dependencies
npm install
```

## Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run generate` | Generate static site |
| `npm run postinstall` | Run Nuxt prepare (auto-installed with `npm install`) |

## Project Structure

```
casino-web-front/
├── app/                    # Application source (Nuxt 4 structure)
│   ├── app.vue            # Root component
│   ├── assets/            # Static assets
│   │   └── css/          # Stylesheets
│   ├── components/        # Vue components
│   │   ├── account/      # Account-related components
│   │   ├── base/         # Base components
│   │   ├── casino/       # Casino game components
│   │   ├── common/       # Shared/common components
│   │   └── sportsbook/   # Sportsbook components
│   ├── composables/      # Vue composables
│   │   ├── account/      # Account logic
│   │   ├── casino/       # Casino logic
│   │   ├── core/         # Core utilities (API, Auth, WebSocket)
│   │   └── sportsbook/   # Sportsbook logic
│   ├── layouts/          # Page layouts
│   │   ├── auth.vue     # Authentication layout
│   │   ├── default.vue  # Default layout
│   │   └── sportsbook.vue # Sportsbook layout
│   ├── middleware/       # Nuxt middleware
│   │   ├── auth.global.ts # Global auth middleware
│   │   ├── guest.ts     # Guest-only routes middleware
│   │   ├── kyc.ts       # KYC verification middleware
│   │   └── responsible-gaming.ts # Responsible gaming middleware
│   ├── pages/           # Application pages
│   │   ├── account/     # Account pages
│   │   ├── auth/        # Authentication pages
│   │   ├── casino/      # Casino pages
│   │   ├── live/        # Live casino pages
│   │   ├── promotions/  # Promotions pages
│   │   └── sportsbook/  # Sportsbook pages
│   ├── plugins/         # Nuxt plugins
│   │   ├── analytics.client.ts # Client-side analytics
│   │   ├── api.ts       # API plugin
│   │   ├── i18n.ts      # i18n plugin
│   │   └── socket.client.ts # WebSocket client plugin
│   └── types/           # TypeScript type definitions
│       └── api/         # API types
├── i18n/                # Internationalization
│   ├── en.json          # English translations
│   └── es.json          # Spanish translations
├── server/              # Server-side code
│   ├── api/             # API routes
│   │   ├── proxy/       # Proxy routes
│   │   └── health.get.ts # Health check endpoint
│   └── utils/           # Server utilities
├── services/            # Business logic services
│   ├── api.client.ts    # HTTP client
│   ├── auth.service.ts # Authentication service
│   ├── casino.service.ts # Casino service
│   ├── promotions.service.ts # Promotions service
│   ├── sportsbook.service.ts # Sportsbook service
│   └── wallet.service.ts # Wallet service
├── shared/              # Shared resources
│   ├── constants/       # Application constants
│   └── schemas/         # Validation schemas
├── stores/              # Pinia stores
├── tests/               # Test files
│   ├── e2e/            # End-to-end tests
│   └── unit/           # Unit tests
├── public/              # Static public files
├── types/               # Global TypeScript types
├── utils/               # Utility functions
│   ├── constants/       # Constants
│   ├── formatters/     # Formatters
│   └── validators/     # Validators
├── nuxt.config.ts       # Nuxt configuration
├── tsconfig.json       # TypeScript configuration
└── package.json        # Dependencies
```

## Features

### Core Features

- **Casino**: Online casino games interface
- **Sportsbook**: Sports betting platform with live events
- **Wallet**: Integrated wallet management system
- **Authentication**: User authentication and session management
- **i18n**: Internationalization support (English, Spanish)
- **Responsive**: Mobile-first responsive design

### Technical Stack

- **Framework**: [Nuxt 4](https://nuxt.com/)
- **UI**: [@nuxt/ui](https://ui.nuxt.com/)
- **State Management**: [Pinia](https://pinia.vuejs.org/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **Language**: TypeScript

## Development

### Adding Dependencies

```bash
npm install <package-name>
```

## Contributing

This project follows the [Conventional Commits](https://www.conventionalcommits.org/) specification.

### Commit Message Format

```
<type>: <description>
```

### Types

| Type | Description |
|------|-------------|
| `feat` | A new feature |
| `fix` | A bug fix |
| `docs` | Documentation only changes |
| `refactor` | A code change that neither fixes a bug nor adds a feature |
| `test` | Adding missing tests |
| `build` | Changes that affect the build system |
| `ci` | Changes to CI configuration |
| `chore` | Other changes |

## License

Private project - All rights reserved