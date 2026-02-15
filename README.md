# Smart-BookMark-Manager
Bookmarks

## Summary
**Goal:** Prepare the project for deployment by adding Vercel configuration for the Vite + React SPA and documenting deployment and verification steps.

**Planned changes:**
- Add Vercel deployment configuration to build and serve the frontend as a static SPA, including rewrites so deep links route to `index.html`.
- Update the repository README with step-by-step deployment instructions for both the frontend (static hosting such as Vercel) and the Internet Computer Motoko canister (via `dfx`), plus an English troubleshooting section.
- Document a local “deployment verification” workflow that starts a clean local `dfx` environment, deploys canister(s), builds the frontend, and validates local Internet Identity sign-in and bookmark CRUD.

**User-visible outcome:** The app can be deployed as a static SPA on Vercel with working client-side routing, and the README provides clear deployment, troubleshooting, and local verification steps for the frontend and canister.
To run app build and run docker image: `docker build -t app . docker run -it --network host app`
 Smart Bookmarks - Internet Computer Bookmark Manager

A private, secure bookmark manager built on the Internet Computer using Internet Identity authentication. Your bookmarks are stored on-chain and are completely private to you.

## Features

- 🔐 **Secure Authentication**: Sign in with Internet Identity (no passwords needed)
- 🔒 **Private by Default**: Your bookmarks are only visible to you
- ⚡ **Real-time Sync**: Changes appear instantly across all your open tabs
- 🎨 **Beautiful UI**: Clean, modern interface with warm amber/orange theme
- 📱 **Responsive Design**: Works seamlessly on desktop and mobile devices

## Tech Stack

- **Frontend**: React + TypeScript + Vite
- **Backend**: Motoko (Internet Computer)
- **Authentication**: Internet Identity
- **Styling**: Tailwind CSS + shadcn/ui components
- **State Management**: React Query (TanStack Query)

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- [DFX](https://internetcomputer.org/docs/current/developer-docs/setup/install/) (Internet Computer SDK)
- [pnpm](https://pnpm.io/) package manager

### Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   cd frontend
   pnpm install
   ```

### Local Development

For a complete local development workflow, see the [Deployment Verification Guide](./docs/deployment-verification.md) which includes step-by-step instructions for:
- Setting up a clean local environment
- Deploying canisters locally
- Running the frontend development server
- Verifying Internet Identity login and bookmark operations

Quick start:
