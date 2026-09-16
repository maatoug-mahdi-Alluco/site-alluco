# ALLUCO 3D Website

Premium public website for ALLUCO — aluminium, import, export, logistics and distribution.

## Stack

- Next.js 16
- React 19
- TypeScript
- Three.js
- React Three Fiber
- GSAP / ScrollTrigger

No external 3D file is required for the first deployment. The industrial environment is generated with Three.js geometry.

## Local development

```bash
npm install
npm run dev
```

Open http://localhost:3000

## Production validation

```bash
npm run typecheck
npm run build
npm run start
```

## Contact information

Copy `.env.example` to `.env.local` and fill only verified ALLUCO values:

```bash
cp .env.example .env.local
```

Variables:

```text
NEXT_PUBLIC_ALLUCO_EMAIL=
NEXT_PUBLIC_ALLUCO_PHONE=
NEXT_PUBLIC_ALLUCO_ADDRESS=
NEXT_PUBLIC_ALLUCO_WHATSAPP=
```

If values remain empty, the website clearly displays placeholders instead of inventing contact information.

## GitHub

The following files must be at the repository root:

```text
app/
components/
lib/
public/
package.json
tsconfig.json
next.config.mjs
```

Example commands:

```bash
git init
git add .
git commit -m "ALLUCO 3D website"
git branch -M main
git remote add origin https://github.com/YOUR_ACCOUNT/YOUR_REPOSITORY.git
git push -u origin main
```

## Vercel deployment

1. Sign in to Vercel with GitHub.
2. Import the ALLUCO repository.
3. Framework preset: Next.js.
4. Root Directory: `./` if `package.json` is at repository root.
5. Deploy.

Vercel does not require a `Main file path` for a Next.js application.

## Replacing procedural 3D assets later

Put production GLB/GLTF assets under `public/models/` and introduce `GLTFLoader` or `useGLTF` only after the files are available and optimised. Keep model sizes low, use Draco/Meshopt when appropriate, and provide simplified mobile assets.
