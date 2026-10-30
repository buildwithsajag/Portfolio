# Personal Portfolio Website

A fast, lightweight, and responsive personal portfolio built with semantic HTML5, modern vanilla CSS, and vanilla JavaScript. Designed specifically for an aspiring Agentic AI Engineer, it showcases projects, core technical competencies, and an integrated contact form—with zero build tools, frameworks, or runtime dependencies required.

---

## Folder Structure

```text
Portfolio/
├── index.html              # Main HTML5 document containing all sections
├── README.md               # Project documentation and deployment guide
├── robots.txt              # Search engine crawler instructions and sitemap link
├── assets/
│   ├── icons/
│   │   └── favicon.svg     # Custom SVG site favicon (teal circle with initials)
│   └── images/             # Folder for avatar portrait and project screenshots
├── css/
│   └── styles.css          # Design system, CSS reset, layout, and interactive styles
└── js/
    └── script.js           # Navigation scrollspy, mobile menu, and reveal animations
```

---

## Step-by-Step Deployment Guide (Netlify Drag & Drop)

Deploying this portfolio to the web takes less than a minute using Netlify's free static hosting. No command line or account setup is required to get a live preview URL.

### Step 1: Open Netlify Drop
1. In your web browser, navigate to:  
   👉 **[app.netlify.com/drop](https://app.netlify.com/drop)**
2. (Optional but recommended) Sign in or create a free Netlify account so you can manage your site and custom domains later.

### Step 2: Upload Your Project Folder
You can upload the project using either method:
- **Direct Folder Upload (Chrome / Edge / Brave / Safari)**: Drag the entire `Portfolio` folder directly from your file explorer into the dashed box on the Netlify Drop page.
- **ZIP File Upload**: Right-click the `Portfolio` folder on your computer, choose **Compress to ZIP**, and drag the resulting `.zip` file into Netlify Drop.

### Step 3: Wait for Instant Deployment
- Netlify will automatically upload your files and generate a live URL within seconds (e.g., `https://random-name-12345.netlify.app`).

### Step 4: Rename Your Site to a Custom Name
1. Once deployed, click on **Site configuration** (or **Site settings**).
2. Click **Change site name**.
3. Enter your preferred subdomain (for example: `sajag-ai-portfolio` or `yourname-dev`).
4. Click **Save**. Your site is now live at:  
   `https://your-custom-name.netlify.app`

### Step 5: Copy and Share Your Live URL
- Copy your new live URL from the top of the Netlify dashboard and test it across desktop and mobile devices.

---

## Enabling Contact Form Submissions with Netlify Forms

To receive messages submitted through the contact form directly in your Netlify dashboard and via email:

1. Open `index.html` in your text editor.
2. Locate the `<form class="contact-form" ...>` element (around line 300).
3. Add the `data-netlify="true"` and `name="contact"` attributes:
   ```html
   <form class="contact-form reveal" name="contact" method="post" data-netlify="true">
     <!-- Hidden input required by Netlify for static HTML forms -->
     <input type="hidden" name="form-name" value="contact">
     ...
   </form>
   ```
4. Save and re-upload the folder to Netlify.
5. In your Netlify dashboard under **Site > Forms**, you will now see every message sent from your site. You can also configure email notifications under **Form notifications**.

---

## Local Development & Preview

Because this project uses pure HTML, CSS, and vanilla JS, you can run it locally with any simple static server:

```bash
# Using Python 3
python3 -m http.server 8000

# Or using Node.js npx serve
npx serve .
```

Open `http://127.0.0.1:8000` in your web browser.
# Portfolio
