Live Demo: https://syncinterview.vercel.app

A lightweight interview management app that syncs user roles (interviewer/candidate) via Clerk authentication and Convex edge functions, built with Next.js and Tailwind CSS.

---

## 📝 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running Locally](#running-locally)
- [Environment Variables](#-environment-variables)
- [Project Structure](#-project-structure)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

## ✨ Features

- **Role Sync**: Automatically insert or upgrade users in Convex with `interviewer` role via the `syncUser` mutation.
- **Authentication**: Secure sign-up and sign-in flows powered by Clerk.
- **Real-time Data**: Fetch and display user lists with Convex queries.
- **Serverless Edge Functions**: Run your business logic close to users using Convex.
- **Responsive UI**: Modern, mobile-first design with Tailwind CSS.
- **Performance Optimizations**: SSR/ISR, code-splitting, and lazy loading for fast experience.

---

## 🛠 Tech Stack

- **Framework:** Next.js (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **Auth:** Clerk
- **Database & Functions:** Convex
- **Deployment:** Vercel

---

## 🚀 Getting Started

### Prerequisites

- Node.js ≥ 18
- npm or yarn
- A Convex project & deployment token
- Clerk account & API keys

### Installation

1. **Clone the repo**
   ```bash
   git clone https://github.com/FixRin/syncinterview.git
   cd syncinterview
   ```
2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn
   ```
3. **Copy environment example**
   ```bash
   cp .env.example .env.local
   ```

### Running Locally

- **Development mode**
  ```bash
  npm run dev
  ```
  Open at http://localhost:3000

- **Build & Preview**
  ```bash
  npm run build
  npm run start
  ```

---

## 🔒 Environment Variables

```dotenv
# Convex
NEXT_PUBLIC_CONVEX_URL=your_convex_url
CONVEX_SECRET=your_convex_secret

# Clerk
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_live_...
CLERK_SECRET_KEY=sk_live_...
```

---
