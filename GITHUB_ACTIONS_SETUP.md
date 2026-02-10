# GitHub Actions Setup Guide

This guide will help you set up automatic deployments to Vercel when you push to GitHub.

## Step 1: Get Your Vercel Token

1. Go to [Vercel Tokens Page](https://vercel.com/account/tokens)
2. Click **"Create Token"**
3. Name it: `GitHub Actions - Society of Legal Professionals`
4. Set expiration: Choose your preference (recommended: No Expiration or 1 year)
5. Click **"Create"**
6. **IMPORTANT:** Copy the token immediately (you won't be able to see it again)

## Step 2: Add Secrets to GitHub

1. Go to your GitHub repository: https://github.com/mohitmail85/society-of-legal-professionals
2. Click **"Settings"** (top menu)
3. Click **"Secrets and variables"** → **"Actions"** (left sidebar)
4. Click **"New repository secret"**

Add these **3 secrets** one by one:

### Secret 1: VERCEL_TOKEN
- **Name:** `VERCEL_TOKEN`
- **Value:** (paste the token you created in Step 1)
- Click **"Add secret"**

### Secret 2: VERCEL_ORG_ID
- Click **"New repository secret"** again
- **Name:** `VERCEL_ORG_ID`
- **Value:** `team_eFzZWROtHQwTQzjN6dWp4Tkm`
- Click **"Add secret"**

### Secret 3: VERCEL_PROJECT_ID
- Click **"New repository secret"** again
- **Name:** `VERCEL_PROJECT_ID`
- **Value:** `prj_id4AmNSU2QC0EYVPj6oATjhfbJzI`
- Click **"Add secret"**

## Step 3: Verify Setup

After adding all secrets, you should see:
- ✅ VERCEL_TOKEN
- ✅ VERCEL_ORG_ID
- ✅ VERCEL_PROJECT_ID

## Step 4: Test the Workflow

The GitHub Action will automatically run when you push to the `master` or `main` branch.

To test it:

```bash
# Make a small change
echo "<!-- GitHub Actions test -->" >> index.html

# Commit and push
git add .
git commit -m "test: GitHub Actions deployment"
git push
```

## Step 5: Monitor Deployment

1. Go to your repository on GitHub
2. Click the **"Actions"** tab
3. You'll see your workflow running
4. Click on it to see detailed logs

## How It Works

```
You push to GitHub
       ↓
GitHub Actions triggers
       ↓
Workflow installs Vercel CLI
       ↓
Builds your project
       ↓
Deploys to Vercel
       ↓
Your site is live! 🎉
```

## Workflow Triggers

The workflow runs automatically on:
- ✅ Push to `master` branch
- ✅ Push to `main` branch
- ✅ Pull requests to these branches

## Troubleshooting

### Error: "VERCEL_TOKEN not found"
- Make sure you added the secret correctly (no extra spaces)
- Secret names are case-sensitive

### Error: "Project not found"
- Verify VERCEL_PROJECT_ID matches your project
- Check VERCEL_ORG_ID is correct

### Workflow not running
- Check if the workflow file is in `.github/workflows/deploy.yml`
- Verify you pushed to `master` or `main` branch
- Check GitHub Actions is enabled in repository settings

## Workflow File Location

The workflow file is located at:
```
.github/workflows/deploy.yml
```

## Viewing Deployment URL

After successful deployment, check the workflow logs for the deployment URL, or visit your Vercel dashboard.

---

**Need Help?**
- [Vercel Documentation](https://vercel.com/docs)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)
