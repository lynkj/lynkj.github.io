# IDSLab Website

A professional, distinctive academic laboratory website for the Intelligent Data Science Laboratory at Seoul National University.

## Features

- **Modern Editorial Design**: Clean, refined aesthetic with distinctive typography and warm color palette
- **Responsive Layout**: Fully responsive design that works on all devices
- **Two Main Pages**:
  - Home page with lab introduction, director info, and publications
  - People page with current members and alumni
- **Smooth Animations**: Subtle scroll-based animations and transitions
- **Easy to Update**: Simple HTML structure for easy content updates

## File Structure

```
lynkj.github.io/
├── index.html          # Main page
├── members.html        # People page
├── css/
│   └── style.css      # Main stylesheet
├── js/
│   └── script.js      # JavaScript for interactions
└── README.md          # This file
```

## Deployment to GitHub Pages

1. **Initialize Git Repository** (if not already done):
   ```bash
   git init
   git add .
   git commit -m "Initial commit - IDSLab website"
   ```

2. **Connect to GitHub**:
   ```bash
   git remote add origin https://github.com/lynkj/lynkj.github.io.git
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to your repository settings on GitHub
   - Navigate to "Pages" section
   - Under "Source", select "main" branch
   - Click "Save"
   - Your site will be live at: https://lynkj.github.io

## Customization Guide

### 1. Update Laboratory Information

**In `index.html`**:
- Update the "About the Lab" section with your actual lab description
- Modify research areas to match your lab's focus
- Update Professor Park's contact information and bio

### 2. Add Publications

**In `index.html`**, find the publications section and add your papers:

```html
<article class="publication">
    <div class="pub-meta">
        <span class="pub-type">Journal Article</span>
    </div>
    <h4 class="pub-title">Your Paper Title Here</h4>
    <p class="pub-authors">Author, A., Author, B., & Author, C.</p>
    <p class="pub-venue"><em>Journal Name</em>, Volume(Issue), Pages.</p>
    <div class="pub-links">
        <a href="DOI_URL" class="pub-link">DOI</a>
        <a href="PDF_URL" class="pub-link">PDF</a>
    </div>
</article>
```

### 3. Update Team Members

**In `members.html`**:

Add current members:
```html
<div class="member-card">
    <div class="member-info">
        <h4 class="member-name">Student Name</h4>
        <p class="member-year">Year Joined: 2024</p>
        <p class="member-research">Research interests: Your interests here</p>
        <div class="member-contact">
            <a href="mailto:email@snu.ac.kr">email@snu.ac.kr</a>
        </div>
    </div>
</div>
```

Add alumni:
```html
<div class="alumni-row">
    <div class="alumni-col name-col">Alumni Name</div>
    <div class="alumni-col year-col">2023</div>
    <div class="alumni-col position-col">Current Position, Company/University</div>
</div>
```

### 4. Customize Colors

**In `css/style.css`**, modify the color variables at the top:

```css
:root {
    --color-primary: #2C1810;      /* Main dark color */
    --color-accent: #C17C4A;       /* Accent color */
    --color-background: #FDFBF7;   /* Page background */
    /* ... other colors ... */
}
```

### 5. Change Fonts

To use different fonts, update the Google Fonts link in both HTML files:

```html
<link href="https://fonts.googleapis.com/css2?family=YourFont:wght@...&display=swap" rel="stylesheet">
```

Then update the CSS variables:
```css
--font-display: 'YourDisplayFont', serif;
--font-body: 'YourBodyFont', sans-serif;
```

## Adding New Pages

1. Create a new HTML file (e.g., `research.html`)
2. Copy the header and navigation from `index.html`
3. Add your content
4. Update the navigation links in all pages to include the new page

## Tips for Maintenance

- **Keep it simple**: The site is designed to be easy to update manually
- **Test locally**: Open `index.html` in your browser before pushing changes
- **Backup regularly**: Commit changes to Git frequently
- **Images**: Create an `images/` folder for any photos or graphics you want to add
- **Publications**: Keep publications in reverse chronological order (newest first)

## Browser Support

The website works on all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

## License

Feel free to customize this template for your laboratory's needs.

## Support

For issues or questions about customization, refer to:
- HTML basics: https://developer.mozilla.org/en-US/docs/Web/HTML
- CSS styling: https://developer.mozilla.org/en-US/docs/Web/CSS
- GitHub Pages: https://docs.github.com/en/pages

---

**IDSLab** - Intelligent Data Science Laboratory  
Graduate School of Business, Seoul National University
