# Deployment Guide — Ship Prestiiiged Tonight

**Time estimate: 45 minutes total**

---

## Step 1: Export PDF (5 min)

### Option A: VS Code + Markdown PDF Extension
1. Open `exports/prestiiiged_high_achiever_os_v1.md` in VS Code
2. Install extension: "Markdown PDF" by yzane
3. Press `Ctrl+Shift+P` → "Markdown PDF: Export (pdf)"
4. Save as `High_Achiever_OS_V1.pdf`

### Option B: Use a Web Converter
1. Go to [markdown2pdf.com](https://www.markdown2pdf.com/)
2. Paste contents of `prestiiiged_high_achiever_os_v1.md`
3. Download PDF

### Option C: Google Docs
1. Create new Google Doc
2. Paste markdown content
3. Format headings manually
4. File → Download → PDF

**Output:** `High_Achiever_OS_V1.pdf`

---

## Step 2: Set Up Gumroad (10 min)

### Create Account
1. Go to [gumroad.com](https://gumroad.com)
2. Sign up (use Google for speed)
3. Skip onboarding questions

### Create Product
1. Click "New Product"
2. Select "Digital Product"

### Fill In Details
Copy from `exports/gumroad_product_copy.md`:

| Field | What to Paste |
|-------|---------------|
| Name | `The High Achiever Operating System` |
| Price | `$19` |
| Description | Copy the full description section |

### Upload Files
1. Click "Add files"
2. Upload:
   - `High_Achiever_OS_V1.pdf`
   - `exports/templates/weekly_review_template.md`
   - `exports/templates/daily_operating_template.md`
   - `exports/templates/positioning_tracker.md`
   - `exports/templates/high_stakes_prep.md`

### Set Thank You Message
1. Go to "Checkout" settings
2. Paste the thank you message from `gumroad_product_copy.md`

### Publish
1. Click "Publish"
2. Copy your Gumroad link (e.g., `gumroad.com/l/abc123`)

**Output:** Your Gumroad link

---

## Step 3: Set Up Chatbot (10 min)

### Create Account
1. Go to [chatbase.co](https://www.chatbase.co/) (or [customgpt.ai](https://customgpt.ai))
2. Sign up

### Create Chatbot
1. Click "New Chatbot"
2. Upload `exports/prestiiiged_high_achiever_os_v1.md` as knowledge base
3. Optionally upload `canon/prestiiiged_principles.md`

### Configure
1. Go to "Settings" or "Instructions"
2. Paste the system prompt from `exports/chatbot_config.md`

### Test
Ask: "I have an interview next week. How should I prepare?"

Verify it:
- Asks about your proof/leverage first
- Mentions temperature control
- Ends with a concrete action

### Get Link
1. Go to "Share" or "Embed"
2. Copy the shareable link or embed code

**Output:** Chatbot link or embed code

---

## Step 4: Deploy Landing Page (10 min)

### Option A: Open Locally (Fastest)
1. Open `exports/site/index.html` in your browser
2. It works immediately — but only on your computer

### Option B: GitHub Pages (Free, Public URL)

1. **Create GitHub repo** (if not already):
   ```
   # Already done — your repo is at github.com/diiimodiiimo/triii
   ```

2. **Enable GitHub Pages**:
   - Go to repo → Settings → Pages
   - Source: "Deploy from a branch"
   - Branch: `main`
   - Folder: `/exports/site` (or root if you move index.html)
   - Save

3. **Your site will be live at**:
   ```
   https://diiimodiiimo.github.io/triii/exports/site/
   ```

### Option C: Netlify (Free, Custom Domain)

1. Go to [netlify.com](https://www.netlify.com/)
2. Sign up with GitHub
3. Click "Add new site" → "Import an existing project"
4. Select your `triii` repo
5. Set publish directory: `exports/site`
6. Deploy

**Your site will be live at:** `https://random-name.netlify.app`

### Option D: Vercel (Free, Fast)

1. Go to [vercel.com](https://vercel.com)
2. Sign up with GitHub
3. Import `triii` repo
4. Set root directory: `exports/site`
5. Deploy

---

## Step 5: Connect Everything (5 min)

### Update Landing Page with Gumroad Link

1. Open `exports/site/index.html`
2. Find all instances of `YOUR_GUMROAD_LINK_HERE`
3. Replace with your actual Gumroad link (e.g., `https://gumroad.com/l/abc123`)
4. Save and redeploy (or refresh if local)

### Add Chatbot Link to Gumroad

In your Gumroad thank you message, add:
```
→ Access your AI advisor here: [YOUR_CHATBOT_LINK]
```

### Commit Changes

```bash
git add .
git commit -m "chore: add gumroad and chatbot links"
git push
```

---

## Step 6: Test End-to-End (5 min)

### Test Flow
1. Visit your landing page
2. Click "Get the playbook"
3. Complete Gumroad checkout (use test mode or buy your own product)
4. Verify:
   - PDF downloads
   - Templates download
   - Thank you message appears
   - Chatbot link works

### Checklist

- [ ] Landing page loads
- [ ] CTA buttons link to Gumroad
- [ ] Gumroad checkout works
- [ ] Files download after purchase
- [ ] Chatbot responds correctly
- [ ] Thank you message includes chatbot link

---

## You're Live

**Total time:** ~45 minutes

**What you now have:**
- A live landing page
- A working checkout (Gumroad)
- A trained AI advisor (Chatbot)
- A shipped product

**Next steps:**
1. Share the link somewhere (Twitter, friends, community)
2. Get 1 sale to validate
3. Collect feedback
4. Iterate

---

## Quick Reference

| Asset | Location |
|-------|----------|
| PDF content | `exports/prestiiiged_high_achiever_os_v1.md` |
| Templates | `exports/templates/` |
| Gumroad copy | `exports/gumroad_product_copy.md` |
| Chatbot config | `exports/chatbot_config.md` |
| Landing page | `exports/site/index.html` |
| This guide | `exports/DEPLOYMENT_GUIDE.md` |

---

*Ship it. Then improve it. Momentum beats perfection.*

