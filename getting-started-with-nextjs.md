---
title: "Getting Started with Next.js"
date: "2026-05-20"
excerpt: "Next.js is the most popular React framework today. Here's why you should use it and how to get started in under 10 minutes."
author: "Your Name"
tags: ["nextjs", "react", "tutorial"]
---

## Why Next.js?

Next.js is a React framework that gives you everything you need to build production-ready web apps. It handles **routing**, **rendering**, **data fetching**, and **deployment** with minimal configuration.

## Key Features

- **App Router** — file-system based routing with layouts and nested routes
- **Server Components** — render on the server by default for better performance
- **Static & Dynamic rendering** — choose per page
- **Built-in Image optimization** — the `<Image>` component handles everything
- **Zero-config TypeScript** — just rename files to `.tsx`

## Your First Page

Create a file at `app/page.tsx`:

```tsx
export default function Home() {
  return <h1>Hello, world!</h1>;
}
```

That's it. Next.js auto-discovers this as your homepage.

## Data Fetching

With the App Router, any component can be `async`:

```tsx
async function getData() {
  const res = await fetch("https://api.example.com/posts");
  return res.json();
}

export default async function Page() {
  const data = await getData();
  return <pre>{JSON.stringify(data, null, 2)}</pre>;
}
```

## Deploying to Vercel

Push your code to GitHub, connect the repo on [vercel.com](https://vercel.com), and you're live — no config needed.

> "Next.js makes the right thing the easy thing."

Happy coding!
