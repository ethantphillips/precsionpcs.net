# Precision PCs Blog

Welcome to the source code for the **Precision PCs Blog** — a fast, modern, and AdSense-ready static blog built with Astro, Netlify CMS, and Markdown.

## 🚀 Features

- ⚡ Lightning-fast Astro static site
- ✍️ Write posts in Markdown or use Netlify CMS
- 📸 Image uploads supported (`/public/uploads`)
- 💸 Google AdSense-ready layout (pub ID: `ca-pub-5717141519109804`)
- 🔐 Protected `/admin` dashboard using Netlify Identity
- 🔁 Redirect from `/blog` to `blog.precisionpcs.net`
- 🧭 Clean navigation across pages
- 🚫 Custom 401 Unauthorized page
- 🕳 Custom 404 Not Found page

---

## 📦 How to Deploy (GitHub + Netlify)

### ✅ Step 1: Extract this ZIP

> 🔥 **DO NOT upload the ZIP to GitHub directly.**  
> Instead, **extract it first**, and upload the contents (folders/files) to your new GitHub repo.

### ✅ Step 2: Push to GitHub

Create a new GitHub repository (e.g. `precisionpcs-blog`) and upload all the extracted files and folders.

You can use GitHub Desktop, drag-and-drop in the browser, or `git` on the command line.

---

### ✅ Step 3: Deploy to Netlify

1. Log in to [Netlify](https://netlify.com)
2. Click **"Add new site" > "Import from GitHub"**
3. Select your repo and follow the prompts
4. Set build settings:
   - Build Command: `npm run build` or `astro build`
   - Publish Directory: `dist`

---

### ✅ Step 4: Protect `/admin` (Netlify CMS)

1. Go to your new blog site's dashboard on Netlify
2. Navigate to **Identity** tab → Click "Enable Identity"
3. Click **"Enable Git Gateway"**
4. Invite yourself as a user (your GitHub email)
5. Accept the email invite and log in once

You can now access:
```
https://blog.precisionpcs.net/admin/
```

Only invited users can use the CMS.

---

### ✅ Step 5: Setup Custom Domain

For the main blog:
- Go to Netlify → Site Settings → Domain
- Add custom domain: `blog.precisionpcs.net`
- Update your DNS (CNAME to Netlify)

---

### ✅ Step 6: Submit to Google & Bing

#### Google:
- Go to [Google Search Console](https://search.google.com/search-console/)
- Add property: `precisionpcs.net`
- Verify via DNS
- Submit: `https://precisionpcs.net` and `https://blog.precisionpcs.net`

#### Bing:
- Go to [Bing Webmaster Tools](https://www.bing.com/webmasters/)
- Add site and submit both URLs

---

### ✍️ Writing Blog Posts

#### Option 1: Use Netlify CMS
- Go to `/admin/`
- Click "New Post"
- Fill the form → Save & publish

#### Option 2: Markdown (GitHub)
- Go to `src/content/blog`
- Add a new `.md` file using the frontmatter format:

```markdown
---
title: "Sample Title"
pubDate: "2025-04-24"
description: "Short post description."
author: "Ethan Phillips"
---
Write your blog post here using **Markdown**!
```

---

### 📬 Questions or Support?

Created by Ethan Phillips • [precisionpcs.net](https://precisionpcs.net)


---

⚠️ **Reminder**: Run `npm install` after cloning or extracting to install Astro and all dependencies.