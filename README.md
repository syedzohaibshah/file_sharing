#  Supabase File & Text Sharer

A lightweight, real-time web app that lets you share **files** and **text** across devices using a simple shared **room code** — no login required.

##  Features

-  No authentication needed
-  Real-time shared text (via Supabase Database)
-  File uploads (up to 50MB) using Supabase Storage
- Live sync across devices using a room code
-  Easily deployable to Netlify, Vercel, or Firebase Hosting

---


##  Setup Instructions

### 1. Create a Supabase project
- Go to [https://supabase.com](https://supabase.com)
- Create a new project
- Copy your `supabaseUrl` and `anon` key from `Project Settings → API`

### 2. Create resources
####  Storage Bucket
- Name: `files`
- Make public
- Add `INSERT` and `SELECT` policies with:
  ```sql
  (true)
