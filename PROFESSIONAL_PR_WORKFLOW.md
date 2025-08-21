# Professional Pull Request Workflow

## After Forking the Repository:

### Step 1: Add Your Fork as Remote
```bash
cd /Users/kiran/Desktop/code/calculator

# Replace YOUR_USERNAME with your actual GitHub username
git remote add fork https://github.com/YOUR_USERNAME/calculator.git

# Verify remotes
git remote -v
# Should show:
# origin    https://github.com/vaishaknr2005-eng/calculator.git (fetch)
# origin    https://github.com/vaishaknr2005-eng/calculator.git (push)
# fork      https://github.com/YOUR_USERNAME/calculator.git (fetch)
# fork      https://github.com/YOUR_USERNAME/calculator.git (push)
```

### Step 2: Create Feature Branch (Professional Practice)
```bash
# Create and switch to a feature branch
git checkout -b fix/deployment-special-character

# Verify you're on the new branch
git branch
```

### Step 3: Push Your Changes to Your Fork
```bash
# Push your branch to your fork
git push fork fix/deployment-special-character
```

### Step 4: Create Pull Request
Go to your forked repository and create a Pull Request with this template:

---

## Pull Request Template

**Title:** Fix deployment issue - rename p&l.html to profit-loss.html

**Description:**
```markdown
## 🔗 Related Issue
Fixes #[ISSUE_NUMBER] - Deployment fails due to special character in filename

## 📋 Changes Made
- [x] Renamed `p&l.html` to `profit-loss.html` to resolve URL encoding issues
- [x] Updated navigation link in `index.html`
- [x] Fixed canonical URL in profit-loss.html
- [x] Updated Open Graph meta tags
- [x] Added comprehensive deployment guide (`DEPLOYMENT_FIX.md`)

## 🧪 Testing
- [x] Local testing - all calculators load correctly
- [x] Verified all internal links work
- [x] Confirmed no 404 errors
- [x] Tested navigation between calculators

## 📸 Before/After
**Before:** `href="p&l.html"` - breaks deployment
**After:** `href="profit-loss.html"` - deployment ready

## 🎯 Impact
- ✅ Enables successful deployment on all major platforms
- ✅ Maintains all existing functionality
- ✅ Improves URL structure and SEO
- ✅ Adds deployment documentation for future reference

## 🚀 Deployment Ready
This fix makes the calculator ready for deployment on:
- GitHub Pages
- Netlify
- Vercel
- Any static hosting platform

## 📝 Additional Notes
- No functionality changes - only filename and references
- Backward compatibility maintained through proper redirects if needed
- Added comprehensive documentation for deployment process

Ready for review! 🎉
```

**Reviewers:** @vaishaknr2005-eng
**Labels:** bugfix, deployment, ready-for-review

---

## Commands Summary:

1. **Create Issue** (copy from ISSUE_TEMPLATE.md)
2. **Fork repository** on GitHub
3. **Set up remotes:**
   ```bash
   git remote add fork https://github.com/YOUR_USERNAME/calculator.git
   ```
4. **Create feature branch:**
   ```bash
   git checkout -b fix/deployment-special-character
   ```
5. **Push to your fork:**
   ```bash
   git push fork fix/deployment-special-character
   ```
6. **Create Pull Request** with the template above

This follows industry best practices! 🏆
