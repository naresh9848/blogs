---
title: "Deploying to Vercel for Free"
date: "2026-05-22"
excerpt: "Vercel's free tier is incredibly generous. Learn how to deploy your Next.js blog in 5 minutes with zero configuration."
author: "Your Name"
tags: ["vercel", "deployment", "devops"]
---

## Why Vercel?

Vercel was built by the creators of Next.js — so the two are a natural fit. The free **Hobby** plan gives you:

- ✅ Unlimited personal projects
- ✅ Automatic HTTPS
- ✅ Global CDN (Edge Network)
- ✅ Automatic deployments on every `git push`
- ✅ Preview deployments for every pull request
- ✅ Custom domains

## Step-by-Step Deployment

### 1. Push to GitHub

Make sure your project is on GitHub:

```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/you/my-blog.git
git push -u origin main
```

### 2. Import on Vercel

1. Go to [vercel.com](https://vercel.com) and sign in with GitHub
2. Click **Add New → Project**
3. Find your repo and click **Import**
4. Leave all settings as default — Vercel detects Next.js automatically
5. Click **Deploy** 🚀

Your site will be live in about 60 seconds.

### 3. Every Push = New Deploy

From now on, every `git push` to your `main` branch triggers a new production deployment automatically.

```bash
# Write a new post, then:
git add posts/my-new-post.md
git commit -m "Add new post"
git push
# → Vercel picks it up and deploys in ~30s
```

## Adding a Custom Domain

On the free plan you can use any domain you own:

1. Go to your project in the Vercel dashboard
2. Click **Settings → Domains**
3. Add your domain and follow the DNS instructions

Your blog will be available at `https://yourdomain.com` with a free SSL certificate — automatically renewed.

---

That's all there is to it. Happy shipping!
