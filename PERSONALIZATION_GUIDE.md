# Portfolio Personalization Guide

## Step 1: Add Your Personal Information

### Update Your Name
In `index.html`, find line 49 and replace `[Your Name]` with your actual name:
```html
Hello, I'm <span class="text-blue-600">John Doe</span>
```

### Add Your Profile Photo
1. Add your profile photo to the `assets/` folder (name it `profile.jpg` or `profile.png`)
2. In `index.html`, line 46, replace:
```html
<img src="assets/profile-placeholder.svg" alt="Profile Photo" class="w-32 h-32 rounded-full mx-auto mb-6 shadow-lg border-4 border-white">
```
with:
```html
<img src="assets/profile.jpg" alt="Your Name Profile Photo" class="w-32 h-32 rounded-full mx-auto mb-6 shadow-lg border-4 border-white">
```

## Step 2: Customize Your Projects

### Add Your Machine Learning Projects
For each project (6 total), update the following in `index.html`:

1. **Project Title**: Replace `[Project Title X]` with your actual project name
2. **Project Description**: Replace the placeholder text with your project description
3. **Project Image**: Add project screenshots to `assets/` folder and update the src
4. **GitHub Link**: Replace `[YOUR_GITHUB_LINK]` with your actual GitHub repository URL
5. **Technology Tags**: Update the technology tags to match your project

Example for one project:
```html
<h3 class="text-xl font-bold text-gray-900 mb-2">Stock Price Predictor</h3>
<p class="text-gray-600 mb-4">
    Built an LSTM neural network to predict stock prices using historical data and technical indicators. Achieved 85% accuracy on test data.
</p>
<div class="flex space-x-2">
    <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded text-sm">Python</span>
    <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded text-sm">LSTM</span>
</div>
<a href="https://github.com/yourusername/stock-predictor" class="text-blue-600 hover:text-blue-800 transition-colors duration-200">
```

## Step 3: Add Your Resume

### Option 1: PDF File
1. Add your resume PDF to the root folder (name it `resume.pdf`)
2. In `script.js`, find line 138 and update:
```javascript
link.href = 'resume.pdf'; // Replace with your actual PDF file
```

### Option 2: Google Drive Link
1. Upload your resume to Google Drive and make it public
2. In `script.js`, replace the download functionality with:
```javascript
window.open('YOUR_GOOGLE_DRIVE_LINK', '_blank');
```

## Step 4: Update Contact Information

### Using FormSubmit (Recommended for free)
1. In `index.html`, find the contact form and update the action:
```html
<form id="contact-form" action="https://formsubmit.co/your-email@example.com" method="POST">
```

### Using Netlify Forms (Alternative)
1. Add `netlify` attribute to the form:
```html
<form id="contact-form" netlify>
```

## Step 5: Customize Skills Section

In `index.html`, update the skills tags to match your actual expertise:
- Replace or add technology names in the skill sections
- Update colors if desired (blue-100/blue-800, green-100/green-800, etc.)

## Step 6: Update About Section

In `index.html`, update the "My Journey" section with your actual background and experience.

## Deployment and LinkedIn Integration

### Deploy on Replit (Free)
1. Your portfolio is already running on Replit
2. Click the "Deploy" button in your Replit project
3. Choose "Replit Deployments" (free tier available)
4. Your site will be available at: `https://your-repl-name.your-username.repl.co`

### Alternative Free Deployment Options
1. **GitHub Pages**: Push to GitHub, enable Pages in repository settings
2. **Netlify**: Connect your GitHub repository for automatic deployment
3. **Vercel**: Similar to Netlify, free tier available

### Adding to LinkedIn
1. Once deployed, copy your website URL
2. Go to LinkedIn Profile → Contact Info → Website
3. Add your portfolio URL
4. You can also add it in your LinkedIn summary/about section

## Pro Tips
- Keep project descriptions concise but impactful
- Use action words (Built, Developed, Implemented, Achieved)
- Include metrics when possible (accuracy %, performance improvements)
- Ensure all links work before deploying
- Test on mobile devices for responsiveness