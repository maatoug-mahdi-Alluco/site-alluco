# Project status

## Included

- Next.js public website
- React Three Fiber / Three.js procedural 3D scene
- GSAP ScrollTrigger reveal animations
- Cinematic scroll-driven camera
- Industrial aluminium yard
- Global supply globe
- Maritime cargo scene
- Stylised Tunisia hub
- Warehouse scene
- Aluminium profile showcase
- Product catalogue presentation
- Responsive/mobile performance reductions
- Reduced-motion support
- WebGL error fallback
- Explicit contact placeholders
- GitHub Actions CI
- Vercel deployment instructions

## Validation performed in the generation environment

- package.json parsed successfully
- tsconfig.json parsed successfully
- local project structure validator passed
- every TypeScript/TSX source file passed TypeScript syntax transpilation
- exact dependency versions in package.json were selected from published npm versions

## Environment limitation

A full `npm install` / `next build` could not be executed here because the runtime timed out while reaching the npm registry. Run the following after uploading to GitHub or on a machine with normal npm access:

```bash
npm install
npm run typecheck
npm run build
```

The included GitHub Actions workflow runs those checks automatically on push to `main`.
