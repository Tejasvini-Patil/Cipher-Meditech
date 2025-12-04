# Cipher Meditech LLP Website

A professional, modern website for Cipher Meditech LLP - a medical devices distributor. This website showcases the company's product portfolio and allows potential customers to get in touch.

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, professional healthcare aesthetic with smooth animations
- **Product Portfolio**: Showcases medical device categories with detailed descriptions
- **Contact Form**: Easy-to-use contact form for inquiries
- **Fast Loading**: Lightweight, optimized code with no heavy frameworks

## Quick Start

### Option 1: Open Directly
Simply double-click `index.html` to open the website in your default browser.

### Option 2: Local Development Server

Using Python:
```bash
# Python 3
python -m http.server 8000

# Then open http://localhost:8000 in your browser
```

Using Node.js (with npx):
```bash
npx serve .

# Or with live-server for auto-reload
npx live-server
```

Using VS Code:
- Install the "Live Server" extension
- Right-click on `index.html` and select "Open with Live Server"

## File Structure

```
cipher/
├── index.html      # Main HTML file
├── styles.css      # All styles
├── script.js       # JavaScript functionality
└── README.md       # This file
```

## Customization

### Updating Company Information

1. **Contact Details**: Edit the contact section in `index.html`
   - Address
   - Phone numbers
   - Email addresses

2. **Products**: Modify the product cards in the Products section of `index.html`

3. **Statistics**: Update the hero stats (500+ products, 200+ partners, etc.)

### Changing Colors

Edit the CSS variables in `styles.css`:

```css
:root {
    --color-primary: #0d6e6e;      /* Main teal color */
    --color-primary-dark: #085454;  /* Darker shade */
    --color-accent: #c4a35a;        /* Gold accent */
    /* ... more colors */
}
```

### Adding Product Images

To add images to product cards:

1. Create an `images` folder
2. Add your images
3. Update the product cards in `index.html` to include `<img>` tags

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome for Android)

## Deployment

### Static Hosting Options

This website can be deployed to any static hosting service:

- **GitHub Pages**: Push to a GitHub repository and enable Pages
- **Netlify**: Drag and drop the folder or connect to Git
- **Vercel**: Import the project from Git
- **Firebase Hosting**: Use Firebase CLI to deploy
- **Traditional Web Hosting**: Upload files via FTP

### Example: Deploy to Netlify

1. Go to [netlify.com](https://netlify.com)
2. Sign up or log in
3. Drag and drop the `cipher` folder onto the deploy area
4. Your site will be live in seconds!

## Form Handling

The contact form currently logs submissions to the console. To make it functional:

### Option 1: Formspree (Easiest)
1. Sign up at [formspree.io](https://formspree.io)
2. Create a new form and get your endpoint
3. Update the form action in `index.html`:
```html
<form action="https://formspree.io/f/your-form-id" method="POST">
```

### Option 2: Netlify Forms
If hosting on Netlify, add `netlify` attribute to the form:
```html
<form name="contact" netlify>
```

### Option 3: Custom Backend
Modify the form submission in `script.js` to send data to your API.

## License

© 2024 Cipher Meditech LLP. All rights reserved.

---

Made with ❤️ for better healthcare

