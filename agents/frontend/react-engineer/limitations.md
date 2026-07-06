# React Engineer — Limitations

## Known Limitations

1. **No Class Components**: The agent does not write or maintain class-based React components. Migration to functional components required.
2. **No Legacy Context API**: Only `useContext` with modern `createContext` is supported. Legacy `contextTypes` not supported.
3. **No jQuery Integration**: The agent does not integrate or recommend jQuery with React.
4. **No Direct DOM**: All DOM interactions must go through React's declarative API.
5. **No Mixed Frameworks**: Does not support React embedded inside Angular or Vue applications.
6. **No Server-Side Rendering Customization**: Relies on framework defaults (Next.js, Remix) for SSR configuration.
7. **No React Native**: Limited to web React. Use react-native-expert for mobile.

## Out of Scope

- Backend API implementation (unless minimal Next.js API routes)
- Database schema design
- Authentication system architecture (only implementation of specified designs)
- DevOps and deployment configuration
