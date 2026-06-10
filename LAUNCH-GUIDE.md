# Launch Guide: paycrunch.co

**Your 10-tool finance calculator site is ready to deploy.**
**Total cost: ~$5-12/year for the domain. Hosting is free.**
**Time to complete: ~20 minutes.**

---

## Step 1: Buy the Domain on Porkbun (2 minutes)

1. Go to: **https://porkbun.com/checkout/search?q=paycrunch.co**
2. If paycrunch.co is available, click **Add to Cart**
3. Click the cart icon (top right) and proceed to checkout
4. Log in with your Porkbun account (or create one if needed)
5. Complete the purchase — WHOIS privacy is included free

---

## Step 2: Create a GitHub Repo (5 minutes)

1. Go to: **https://github.com/new**
2. Log in to your GitHub account
3. Repository name: **paycrunch-site**
4. Set it to **Public** (required for free GitHub Pages)
5. Click **Create repository**

Now upload the site files:

6. On the new repo page, click **"uploading an existing file"** (the link in the quick setup section)
7. Open your Dropbox folder on your computer: **Dropbox > Claude > Video Intelligence > calctools-site**
8. Select **ALL files and folders** inside calctools-site (Ctrl+A to select all)
9. Drag them onto the GitHub upload area
10. Scroll down and click **Commit changes**
11. Wait for the upload to finish — you have ~80 files so it may take a minute

**Important:** Upload the CONTENTS of calctools-site, not the folder itself. Your index.html should be at the root of the repo, not inside a subfolder.

---

## Step 3: Enable GitHub Pages (2 minutes)

1. In your paycrunch-site repo, click **Settings** (gear icon tab at the top)
2. In the left sidebar, click **Pages**
3. Under "Source" select **Deploy from a branch**
4. Branch: select **main**, folder: select **/ (root)**
5. Click **Save**
6. Wait 1-2 minutes, then refresh the page — you'll see a green banner with your live URL: **https://YOUR-USERNAME.github.io/paycrunch-site/**
7. Click that URL and verify your site works — test a few calculators

---

## Step 4: Connect Your Custom Domain (10 minutes)

### In GitHub:

1. Still on the **Settings > Pages** page
2. Under "Custom domain", type: **paycrunch.co**
3. Click **Save**
4. Check the box for **Enforce HTTPS** (if it's not already checked — it may take a few minutes to become available)

### In Porkbun:

5. Go to: **https://porkbun.com/account/domainsSpe498s** (or click "Domain Management" after logging in)
6. Find paycrunch.co and click **DNS**
7. **Delete any existing A records or CNAME records** that Porkbun may have added by default
8. Add these **4 A records** (one at a time):

   | Type | Host | Answer |
   |------|------|--------|
   | A | (leave blank) | 185.199.108.153 |
   | A | (leave blank) | 185.199.109.153 |
   | A | (leave blank) | 185.199.110.153 |
   | A | (leave blank) | 185.199.111.153 |

9. Add this **CNAME record**:

   | Type | Host | Answer |
   |------|------|--------|
   | CNAME | www | YOUR-USERNAME.github.io |

   (Replace YOUR-USERNAME with your actual GitHub username)

10. Click **Save** after each record

**DNS propagation takes 15 minutes to a few hours.** Usually under 30 minutes with Porkbun.

Once propagated, GitHub automatically gives you a free SSL certificate (the padlock icon).

---

## Step 5: Verify It's Working (15-30 minutes after Step 4)

1. Open a new browser tab and go to: **https://paycrunch.co**
2. You should see your homepage with all 10 calculator links
3. Click through 2-3 calculators to make sure they work
4. Try it on your phone too

If it's not working yet, just wait — DNS can take up to a few hours.

---

## Step 6: Submit to Google (5 minutes)

1. Go to: **https://search.google.com/search-console**
2. Click **Add property** > enter **https://paycrunch.co**
3. Google will ask you to verify ownership — choose the **DNS record** method
4. Go back to Porkbun DNS settings and add the TXT record Google gives you
5. Once verified, click **Sitemaps** in Search Console
6. Submit: **https://paycrunch.co/sitemap.xml**
7. Google will start crawling your pages

---

## Step 7: Apply for Google AdSense (after 2-4 weeks)

Wait until Google has indexed your pages (you'll see them in Search Console), then:

1. Go to: **https://adsense.google.com**
2. Sign up with your Google account
3. Enter paycrunch.co as your site
4. Google will give you an AdSense code snippet
5. Send me the code and I'll update all 10 tool pages with your real ad slots
6. Push the updated files to GitHub (see "Updating Your Site" below)
7. Go back to AdSense and complete the verification

**Tip:** Google is more likely to approve if:
- Your site has been live for at least 2-4 weeks
- All 10 tools work properly
- You have privacy policy and terms pages (already included)
- The content is original and useful (it is)

---

## Updating Your Site Later

Whenever you want to make changes:

1. Go to your repo: **https://github.com/YOUR-USERNAME/paycrunch-site**
2. Navigate to the file you want to update
3. Click the **pencil icon** (Edit this file) — or drag updated files onto the repo page to re-upload
4. Commit the changes
5. GitHub Pages auto-deploys in about 1 minute

Or, if you have a batch of updates, just ask me — I'll update the files in your Dropbox folder and you can re-upload them all at once using the same drag-and-drop method from Step 2.

---

## What's Included in Your Site

| File | What It Is |
|------|-----------|
| index.html | Homepage with links to all 10 tools |
| hourly-to-salary-calculator.html | Convert hourly wage to annual salary |
| salary-to-hourly-calculator.html | Convert salary to hourly rate |
| tip-calculator.html | Tip calculator with bill splitting |
| percentage-calculator.html | 3-in-1 percentage calculator |
| overtime-calculator.html | Overtime pay calculator |
| compound-interest-calculator.html | Investment growth calculator |
| take-home-pay-calculator.html | Net pay after taxes estimator |
| loan-payment-calculator.html | Mortgage/loan payment calculator |
| roi-calculator.html | Return on investment calculator |
| discount-calculator.html | Sale price and savings calculator |
| salary/ folder | 50+ programmatic "$X/hour" pages |
| privacy.html | Privacy policy (required for AdSense) |
| terms.html | Terms of use |
| sitemap.xml | Tells Google about all your pages |
| robots.txt | Tells search engines to index everything |
| DEMO-20-per-hour.html | Design demo (can delete before launch) |

---

## Timeline Expectations

- **Day 1 (today):** Buy domain, deploy site, submit to Google
- **Week 1-2:** Google indexes your pages
- **Week 3-4:** Apply for AdSense
- **Month 2-3:** Start seeing organic search traffic trickle in
- **Month 6+:** Meaningful traffic and revenue begin
- **Month 12+:** Portfolio mature enough for $300-1,000+/month potential

---

## Quick Reference Links

| What | Link |
|------|------|
| Buy domain | https://porkbun.com/checkout/search?q=paycrunch.co |
| Porkbun DNS settings | https://porkbun.com/account/domainsSpeeds (then click DNS next to your domain) |
| Create GitHub repo | https://github.com/new |
| GitHub Pages docs | https://docs.github.com/en/pages |
| Google Search Console | https://search.google.com/search-console |
| Google AdSense | https://adsense.google.com |

---

## Next Steps After Launch

Tell Claude to:
1. "Build 5 more finance calculators for paycrunch.co" — expand the portfolio
2. "Create more programmatic SEO pages for hourly-to-salary" — generate pages like "$55/hour annual salary", "$60/hour annual salary", etc.
3. "Write blog posts for my calculator site" — add content depth for SEO
4. "Check my Google Search Console data and suggest improvements" — ongoing optimization
