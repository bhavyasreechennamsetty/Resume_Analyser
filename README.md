Next.js + TailwindCSS + ShadCN UI Starter

This project is a Next.js 13 application built with the App Router, styled using TailwindCSS, and enhanced with ShadCN UI components.
It includes a fully configured development environment with TypeScript, PostCSS, modern UI libraries, and optional Firebase support.

Project Structure

The project uses:

Next.js App Router (app/ directory)

TailwindCSS configured through postcss.config.js 

postcss.config

 and tailwind.config.ts (referenced in components.json settings) 

components

ShadCN UI components configured through .shadcn/components.json 

components

TypeScript setup via tsconfig.json 

tsconfig

Static export support with next.config.js (using output: export) 

next.config

⚙️ Features
✔ Next.js 13 App Router

Supports server components, static exports, and modern routing.

✔ TailwindCSS + PostCSS

Configured out-of-the-box for fast and responsive UI development.

✔ ShadCN UI

Preconfigured aliases for components, utilities, hooks, and UI elements.

Aliases from .shadcn/components.json include:

@/components

@/components/ui

@/lib

@/hooks


components

 TypeScript Strict Mode

Configured with modern TS options for optimal DX.


tsconfig

 Firebase Support

package.json includes full Firebase SDK dependencies.


package

Rich UI Libraries Included

Radix UI components

Recharts (charts)

Embla Carousel

Sonner (notifications)

React Hook Form

Zod validation

All visible in package.json.


package

 Getting Started
1️.Install Dependencies
npm install

2️. Run Development Server
npm run dev


Visit:

http://localhost:3000

3️.Production Build
npm run build
npm start


Because next.config.js uses:

output: "export",
images: { unoptimized: true }


this project supports static export for deployment on Netlify, GitHub Pages, Vercel static export, etc.


next.config

 Styling

This project uses:

tailwind.config.ts (referenced by ShadCN)

app/globals.css for global styles

PostCSS plugins (tailwindcss + autoprefixer)


postcss.config

Scripts

From package.json:

npm run dev → Start local development

npm run build → Build project

npm run start → Start production server

npm run lint → Run ESLint


package

Technologies Used
Technology	Purpose
Next.js 13	Framework
React 18	UI library
TailwindCSS	Styling
TypeScript	Static typing
ShadCN UI / Radix	UI components
Firebase SDK	Authentication, DB, Storage
Recharts	Data visualization
React Hook Form	Form handling
Zod	Schema validation
🛠 Development Tools

ESLint (ignored during builds via next.config.js)

next.config

Autoprefixer

PostCSS

TypeScript incremental builds

 Deployment

Because the project uses:

output: "export"

next.config

You can deploy easily on platforms like:

GitHub Pages

Netlify

Vercel (Static Export)

Cloudflare Pages

Run:

npm run build

Your static export will be generated in the out/ directory.
