# Issue Report for Calculator Deployment Problem

## 🐛 Bug Report: Deployment Fails Due to Special Character in Filename

**Issue URL:** https://github.com/vaishaknr2005-eng/calculator/issues

### **Title:** 
Deployment fails - special character in `p&l.html` filename breaks hosting platforms

### **Description:**
```markdown
## Problem
The calculator website fails to deploy properly on hosting platforms (Netlify, Vercel, GitHub Pages) due to a special character in the filename `p&l.html`.

## Root Cause
The ampersand (`&`) character in `p&l.html` causes URL encoding issues and breaks deployment on most hosting platforms.

## Impact
- Cannot deploy website to production
- All calculators work locally but fail online
- Profit & Loss calculator becomes inaccessible after deployment

## Expected Behavior
All calculator pages should be accessible when deployed to any hosting platform.

## Current Behavior
- Local testing: ✅ Works perfectly
- Deployment: ❌ Fails or Profit & Loss page returns 404

## Reproduction Steps
1. Try to deploy the repository to Netlify, Vercel, or GitHub Pages
2. Navigate to the Profit & Loss calculator
3. Observe 404 error or deployment failure

## Environment
- Browser: Any
- Platforms tested: GitHub Pages, Netlify, Vercel
- Local environment: Works fine

## Proposed Solution
Rename `p&l.html` to `profit-loss.html` and update all references in:
- `index.html` (navigation link)
- Internal meta tags and canonical URLs

## Additional Context
This is a common deployment issue. Most hosting platforms have restrictions on special characters in URLs for security and compatibility reasons.

Labels: bug, deployment, high-priority
```

### **Screenshots/Evidence:**
- Local: Works fine
- Deployed: 404 error on P&L calculator

---

**Copy this content and paste it when creating the issue at:**
https://github.com/vaishaknr2005-eng/calculator/issues/new
