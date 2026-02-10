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

## Local Development

Simply open any HTML file in your browser:

```bash
# On Windows
start index.html

# On Mac
open index.html

# On Linux
xdg-open index.html
```

Or use a simple HTTP server:

```bash
# Python 3
python -m http.server 8000

# Node.js (if you have http-server installed)
npx http-server
```

Then visit `http://localhost:8000`

## Deployment to Vercel

### Method 1: Vercel CLI (Recommended)

1. Install Vercel CLI:
```bash
npm install -g vercel
```

2. Deploy:
```bash
vercel
```

3. Follow the prompts and your site will be live!

### Method 2: Vercel Dashboard

1. Visit [vercel.com](https://vercel.com)
2. Sign up or log in
3. Click "Add New Project"
4. Import your Git repository or drag & drop the folder
5. Deploy!

### Method 3: GitHub Integration

1. Push your code to GitHub
2. Connect your GitHub account to Vercel
3. Import the repository
4. Vercel will automatically deploy

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
