# Society of Legal Professionals Website

A professional static website for a legal association built with HTML and Tailwind CSS.

## Features

- 📱 Fully responsive design
- 🎨 Modern UI with Tailwind CSS
- 📄 5 Pages: Home, About, Services, Membership, Contact
- 🚀 Static HTML (no build process required)
- ⚡ Fast loading times
- 📧 Contact form with validation

## Pages

1. **Home** (`index.html`) - Landing page with hero section and services overview
2. **About** (`about.html`) - Organization information, mission, and values
3. **Services** (`services.html`) - Detailed service descriptions
4. **Membership** (`membership.html`) - Membership tiers and benefits
5. **Contact** (`contact.html`) - Contact form and information

## Tech Stack

- HTML5
- Tailwind CSS (via CDN)
- Font Awesome Icons (via CDN)
- Vanilla JavaScript for interactions

## 🚀 Quick Start

### Prerequisites
- A web browser (Chrome, Firefox, Safari, or Edge)
- Git installed on your computer
- Node.js installed (for Vercel CLI deployment)

### Clone the Repository

```bash
git clone https://github.com/mohitmail85/society-of-legal-professionals.git
cd society-of-legal-professionals
```

## 💻 Running Locally

### Option 1: Direct Browser Opening (Simplest)

Just double-click `index.html` or open it with your browser:

```bash
# On Windows
start index.html

# On Mac
open index.html

# On Linux
xdg-open index.html
```

**Note:** Some features might not work properly due to CORS restrictions with this method.

### Option 2: Using Python HTTP Server (Recommended)

If you have Python installed:

```bash
# Python 3
python -m http.server 8000

# Python 2 (older systems)
python -m SimpleHTTPServer 8000
```

Then open your browser and visit: `http://localhost:8000`

### Option 3: Using Node.js HTTP Server

If you have Node.js installed:

```bash
# Install http-server globally (one time only)
npm install -g http-server

# Run the server
http-server -p 8000

# Or use npx (no installation needed)
npx http-server -p 8000
```

Then open your browser and visit: `http://localhost:8000`

### Option 4: Using Live Server (VS Code)

If you use Visual Studio Code:

1. Install the "Live Server" extension
2. Right-click on `index.html`
3. Select "Open with Live Server"

## 🌐 Deploying to Vercel

### Method 1: Vercel CLI (Recommended for Developers)

**Step 1: Install Vercel CLI**

```bash
# Using npm
npm install -g vercel

# Using yarn
yarn global add vercel
```

**Step 2: Login to Vercel**

```bash
vercel login
```

This will open your browser to authenticate. Follow the prompts.

**Step 3: Deploy**

```bash
# Navigate to your project directory
cd path/to/society-of-legal-professionals

# Deploy to Vercel
vercel

# For production deployment
vercel --prod
```

**Step 4: Follow the Prompts**

- Set up and deploy? **Yes**
- Which scope? Select your account
- Link to existing project? **No** (for first deployment)
- Project name? (default is folder name, press Enter)
- Directory? **./** (press Enter)

Your site will be live in seconds! 🎉

**Subsequent Deployments:**

```bash
# Deploy with automatic production settings
vercel --prod
```

### Method 2: Vercel Dashboard (Easiest for Beginners)

**Step 1: Sign Up/Login**

Visit [vercel.com](https://vercel.com) and create an account or log in.

**Step 2: Import Project**

1. Click "Add New Project" or "Import Project"
2. Select "Import Git Repository"
3. Connect your GitHub, GitLab, or Bitbucket account
4. Select the `society-of-legal-professionals` repository
5. Click "Import"

**Step 3: Configure (Usually Auto-detected)**

- **Framework Preset:** Other (auto-detected for static sites)
- **Build Command:** Leave empty (no build needed)
- **Output Directory:** Leave as `.` or `./`
- **Install Command:** Leave empty

**Step 4: Deploy**

Click "Deploy" and wait for the build to complete (usually 10-30 seconds).

**Your site is now live!** 🚀

### Method 3: GitHub Integration (Best for Continuous Deployment)

This method automatically deploys your site whenever you push changes to GitHub.

**Step 1: Push Code to GitHub**

```bash
# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit"

# Add remote (replace with your repository URL)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git

# Push to GitHub
git push -u origin master
```

**Step 2: Import on Vercel**

1. Go to [vercel.com](https://vercel.com)
2. Click "Add New Project"
3. Select your GitHub repository
4. Click "Import"
5. Click "Deploy"

**Step 3: Automatic Deployments**

Now, every time you push to GitHub, Vercel will automatically deploy:

```bash
# Make changes to your files
git add .
git commit -m "Update homepage content"
git push

# Vercel automatically deploys! ✨
```

### Method 4: Drag & Drop (Quickest for Testing)

1. Go to [vercel.com](https://vercel.com)
2. Drag your project folder onto the Vercel dashboard
3. Wait for deployment
4. Done! 🎊

## 🔧 Post-Deployment

### Custom Domain Setup

1. Go to your project dashboard on Vercel
2. Click "Settings" → "Domains"
3. Add your custom domain (e.g., `societyoflegal.org`)
4. Follow DNS configuration instructions
5. SSL certificate is automatically provided by Vercel

### Environment Variables (if needed in future)

1. Go to "Settings" → "Environment Variables"
2. Add your variables
3. Redeploy for changes to take effect

### Monitoring & Analytics

- **Vercel Analytics:** Available in project dashboard
- **Real-time logs:** View in "Deployments" → Select deployment → "View Logs"

## Project Structure

```
law/
├── index.html          # Homepage
├── about.html          # About page
├── services.html       # Services page
├── membership.html     # Membership page
├── contact.html        # Contact page
├── images/            # Images directory
│   ├── logo.png       # Organization logo
│   └── bg.jpg         # Hero background image
├── vercel.json        # Vercel configuration
└── README.md          # This file
```

## Customization

### Update Content
Simply edit the HTML files to update text, images, and content.

### Change Colors
The site uses Tailwind's default blue color scheme. To change colors, update the class names:
- `bg-blue-600` → `bg-green-600` (for green)
- `text-blue-600` → `text-red-600` (for red)
- etc.

### Add Images
Replace placeholder sections with actual images:
```html
<img src="your-image.jpg" alt="Description" class="w-full h-auto">
```

### Update Contact Information
Edit the contact details in `contact.html` and the footer sections.

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

This project is open source and available for modification.

## Support

For questions or issues, please contact the development team.
