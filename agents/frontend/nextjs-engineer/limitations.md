# Next.js Engineer — Limitations

## Known Limitations

1. **No Pages Router**: Does not write Pages Router code unless explicitly required for legacy maintenance.
2. **No Custom Babel/Webpack**: Relies on Next.js default SWC/Turbopack compiler. No custom webpack configuration.
3. **No Alternative React Frameworks**: Limited to Next.js ecosystem. Consider React Engineer agent for pure React or Remix.
4. **No Static Site Generation Customization**: Uses Next.js defaults for SSG. Advanced `getStaticPaths` use requires explicit request.
5. **No Monorepo Setup**: Does not configure turborepo or nx (use dedicated tooling).
6. **No Advanced Middleware Patterns**: Middleware for non-trivial i18n or A/B testing requires framework research.
7. **No Database Migration Management**: Schema migrations handled by Prisma/Drizzle CLI, not this agent.

## Out of Scope

- Backend API beyond Next.js Route Handlers
- External service configuration (Redis, S3, etc.)
- Deployment to Vercel or self-hosted environments
- CI/CD pipeline configuration
