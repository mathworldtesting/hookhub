# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

HookHub is a Next.js 15.5.3 application using the App Router architecture with TypeScript, Tailwind CSS v4, and Turbopack for optimized builds.

## Development Commands

```bash
# Start development server with hot reload (using Turbopack)
npm run dev

# Build production bundle (using Turbopack)
npm run build

# Start production server
npm run start

# Run ESLint for code quality checks
npm run lint
```

## Architecture

### Tech Stack
- **Framework**: Next.js 15.5.3 with App Router
- **Language**: TypeScript with strict mode enabled
- **Styling**: Tailwind CSS v4 with PostCSS
- **Build Tool**: Turbopack (enabled for both dev and build)
- **Font System**: Uses Geist font family via next/font

### Project Structure
- `/app` - App Router pages and layouts
  - `layout.tsx` - Root layout with font configuration
  - `page.tsx` - Home page component
  - `globals.css` - Global styles and Tailwind directives
- `/public` - Static assets (images, SVGs)

### Key Configuration
- **TypeScript**: Strict mode enabled, uses path alias `@/*` for imports from project root
- **ESLint**: Configured with Next.js core-web-vitals and TypeScript rules
- **Tailwind**: Version 4 with PostCSS configuration

## Important Notes

- The project uses Turbopack for both development and production builds (see --turbopack flag in package.json)
- Path imports use the `@/` alias which maps to the project root
- Default port for development server is 3000