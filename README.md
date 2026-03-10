# Juneteenth Barcelona Website

Modern website for Juneteenth Barcelona with a built-in CMS for easy content management.

---

## 🚀 Deploy to Netlify (one-time setup, ~10 minutes)

### Step 1 — Put files on GitHub
1. Create a free account at [github.com](https://github.com)
2. Create a new **public** repository called `juneteenthbarcelona`
3. Upload all these files to the repository

### Step 2 — Deploy on Netlify
1. Go to [netlify.com](https://netlify.com) and sign up (free)
2. Click **"Add new site" → "Import an existing project"**
3. Connect your GitHub account and select the `juneteenthbarcelona` repo
4. Leave all build settings as default and click **"Deploy site"**
5. Your site will be live at a URL like `https://random-name.netlify.app`

### Step 3 — Connect your domain (juneteenthbarcelona.es)
1. In Netlify: go to **Site settings → Domain management → Add custom domain**
2. Enter `juneteenthbarcelona.es`
3. Update your domain's DNS records with your registrar to point to Netlify
   (Netlify will show you the exact records to add)

### Step 4 — Enable the CMS
1. In Netlify: go to **Site settings → Identity → Enable Identity**
2. Scroll to **Registration** and set it to **"Invite only"**
3. Go to **Site settings → Identity → Services → Enable Git Gateway**
4. Open `admin/config.yml` and replace `YOUR-GITHUB-USERNAME` with your actual GitHub username

### Step 5 — Invite volunteers
1. In Netlify: go to **Identity → Invite users**
2. Enter each volunteer's email address
3. They'll receive an invite link and can log in at `yoursite.com/admin`

---

## ✏️ Using the CMS (for volunteers)

1. Go to `https://juneteenthbarcelona.es/admin`
2. Log in with your email and password
3. You'll see the dashboard with four sections:

| Section | What you can edit |
|---|---|
| **Event Details** | Date, venue, registration link, schedule items |
| **Announcements** | Create/edit news posts shown on the homepage |
| **Photo Gallery** | Upload photos and add captions |
| **Site Settings** | Tagline, contact email, social media links |

4. Make your changes and click **Publish** — the site updates automatically within ~1 minute.

---

## 📁 File Structure

```
juneteenthbarcelona/
├── index.html          ← Main website
├── netlify.toml        ← Netlify configuration
├── admin/
│   ├── index.html      ← CMS login page (visit /admin)
│   └── config.yml      ← CMS field definitions
├── _data/
│   ├── event.json      ← Event details (managed by CMS)
│   ├── gallery.json    ← Gallery photos (managed by CMS)
│   ├── settings.json   ← Site settings (managed by CMS)
│   └── announcements/  ← News posts (managed by CMS)
└── images/             ← Uploaded images stored here
```

---

## 🆘 Need help?

Email: barcelona@juneteenth.es
