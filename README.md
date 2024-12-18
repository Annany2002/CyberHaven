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

```
cyberhaven/
├── packages/
│   ├── api/               # Backend API
│   │   ├── src/
│   │   │   ├── controllers/  # API route handlers
│   │   │   ├── models/      # Database models
│   │   │   ├── services/     # Business logic
│   │   │   ├── routes/       # API routes
│   │   │   ├── middleware/   # Authentication, authorization
│   │   │   ├── config/       # API configurations
│   │   │   └── index.js      # API entry point
│   ├── cli/               # Command-line interface
│   │   ├── src/
│   │   │   ├── commands/    # CLI command implementations
│   │   │   ├── utils/       # Helper functions
│   │   │   └── index.js      # CLI entry point
│   ├── dashboard/        # Web dashboard (React)
│   │   ├── src/
│   │   │   ├── components/  # UI components
│   │   │   ├── pages/       # Dashboard pages
│   │   │   ├── styles/      # CSS or styling files
│   │   │   └── App.js        # Main application component
│   └── core/              # Shared code (utils, types)
│       ├── src/
│       │   ├── utils/       # Shared utility functions
│       │   ├── types/       # TypeScript types
│       │   └── index.js      # Core module entry point
├── services/
│   ├── deployment/       # Deployment service
│   │   ├── src/
│   │   │   ├── deployer.js   # Handles deployment logic
│   │   │   ├── builder.js    # Handles build processes
│   │   │   └── index.js      # Deployment service entry point
│   ├── functions/        # Serverless function service
│   │   ├── src/
│   │   │   ├── runtime.js    # Function runtime environment
│   │   │   ├── manager.js   # Manages function deployments
│   │   │   └── index.js      # Function service entry point
│   ├── caching/          # Caching service
│   │   ├── src/
│   │   │   ├── cdn.js       # CDN interaction
│   │   │   ├── cache.js     # Caching logic
│   │   │   └── index.js      # Caching service entry point
├── infrastructure/      # Infrastructure as code
│   ├── aws/              # AWS infrastructure (Terraform)
│   │   ├── main.tf        # Main Terraform configuration
│   │   ├── variables.tf   # Terraform variables
│   │   └── outputs.tf     # Terraform outputs
├── scripts/              # Utility scripts
│   ├── deploy.sh         # Deployment script
│   ├── build.sh          # Build script
│   └── test.sh           # Test script
├── .eslintrc.js          # ESLint configuration
├── .prettierrc.js       # Prettier configuration
├── tsconfig.json         # TypeScript configuration
└── package.json          # Project metadata and dependencies
```

## Getting Started

**1. Clone the repository:**

```bash
git clone https://github.com/Annany2002/CyberHaven.git
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
