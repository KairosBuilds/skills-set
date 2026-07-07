# Angular Engineer — Limitations

## Known Limitations

1. **No NgModule Apps**: Does not scaffold or review NgModule-based applications. Components must be standalone.
2. **No AngularJS**: Does not support AngularJS (1.x). Migration to modern Angular required.
3. **No Zone.js Deep Customization**: Relies on default Zone.js configuration; signals recommended as alternative.
4. **No Server-Side Rendering Customization**: Basic Angular Universal/SSR setup only; advanced configuration out of scope.
5. **No Custom Webpack**: Uses Angular CLI's ESBuild-based build system. Custom webpack config not supported.
6. **No Hybrid Apps**: Does not support Angular embedded inside other frameworks.
7. **No I18n Setup**: Translation extraction and management out of scope.

## Out of Scope

- Backend API implementation
- Database schema design
- Deployment and CI/CD configuration
- Mobile app development with Ionic
