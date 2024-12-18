# CyberHaven : My Vercel Alternative

This project aims to build an open-source alternative to Vercel, a platform for deploying and hosting front-end applications.

## Features

* **(Planned) Support for multiple frameworks:** Next.js (initial focus), React, Vue, Angular, and static site generators.
* **Git integration:** Connect to GitHub for automated deployments.
* **Serverless functions:** Deploy and manage serverless functions.
* **Edge caching:**  CDN integration for fast content delivery.
* **Custom domains and SSL certificates:** Securely host your applications.
* **CLI tool:**  Manage deployments from the command line.
* **Web dashboard:**  Monitor deployments and manage projects.

## Project Structure

cyberhaven/
├── packages/
│   ├── api/               \# Backend API
│   │   └── src/           \# API source code
│   ├── cli/               \# Command-line interface
│   │   └── src/           \# CLI source code
│   ├── dashboard/        \# Web dashboard (React)
│   │   └── src/           \# Dashboard source code
│   └── core/              \# Shared code (utils, types)
│       └── src/           \# Core source code
├── services/
│   ├── deployment/       \# Deployment service
│   │   └── src/           \# Deployment service source code
│   ├── functions/        \# Serverless function service
│   │   └── src/           \# Function service source code
│   └── caching/          \# Caching service
│       └── src/           \# Caching service source code
├── infrastructure/      \# Infrastructure as code
│   └── aws/              \# AWS infrastructure (Terraform)
├── scripts/              \# Utility scripts
├── .eslintrc.js          \# ESLint configuration
├── .prettierrc.js       \# Prettier configuration
├── tsconfig.json         \# TypeScript configuration
└── package.json          \# Project metadata and dependencies

## Getting Started

**1. Clone the repository:**

```bash
git clone url
````

**2. Install dependencies:**

```bash
cd cyberhaven
npm install
```

**3. Set up environment variables:**

  * Create a `.env` file in the root directory.
  * Add your cloud provider credentials, database connection string, and other necessary configurations.

**4. Start the development server:**

```bash
npm run dev
```

This will start the API, CLI, and dashboard in development mode.

## Contributing

Contributions are welcome\! Please feel free to open issues and submit pull requests.

## Roadmap

  * **Phase 1 (MVP):**
      * Basic Next.js deployment
      * Simple serverless functions
      * Basic CLI and dashboard
  * **Phase 2:**
      * Support for more frameworks (React, Vue, Angular)
      * Enhanced serverless function features
      * Improved CLI and dashboard
  * **Phase 3:**
      * Edge caching and CDN integration
      * Advanced deployment options
      * Open-source contributions

## License

This project is licensed under the MIT License - see the [LICENSE](https://www.google.com/url?sa=E&source=gmail&q=LICENSE) file for details.
