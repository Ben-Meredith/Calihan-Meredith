# Calahan-Meredith Web Development Website

A professional web development business website built with Flask, HTML, CSS, and JavaScript.

## Features

- **Responsive Design** - Works on all devices
- **Top Info Bar** - Contact information and social links
- **Hero Carousel** - Eye-catching image slider
- **Services Page** - Detailed service descriptions
- **About Page** - Company information and technologies
- **Portfolio Page** - Showcase of past projects
- **Contact Form** - Easy way for clients to reach out
- **Professional Footer** - Organized information and links

## File Structure

```
/mnt/user-data/outputs/
├── app.py                      # Flask application
├── templates/                   # HTML templates
│   ├── base.html               # Base template (header, footer, navbar)
│   ├── index.html              # Home page
│   ├── services.html           # Services page
│   ├── about.html              # About page
│   ├── portfolio.html          # Portfolio page
│   └── contact.html            # Contact page
├── static/                      # Static files
│   ├── css/
│   │   └── style.css           # Main stylesheet
│   ├── js/
│   │   └── script.js           # JavaScript functionality
│   └── images/                 # Images folder (add your images here)
└── README.md                    # This file
```

## How to Run

### Option 1: Run with Flask (Development Server)

1. Make sure you have Python installed
2. Install Flask:
   ```bash
   pip install flask
   ```
3. Navigate to the project directory:
   ```bash
   cd /mnt/user-data/outputs
   ```
4. Run the Flask app:
   ```bash
   python app.py
   ```
5. Open your browser and go to: `http://localhost:5000`

### Option 2: Deploy to a Web Server

You can deploy this to any hosting service that supports Flask:
- **Heroku**
- **PythonAnywhere**
- **DigitalOcean**
- **AWS**
- **Google Cloud**

## Customization

### Update Contact Information

1. Edit `templates/base.html`:
   - Change email address (line 21)
   - Change phone number (line 24)
   - Update social media links (lines 29-32)
   - Update location (line 91)

### Add Your Logo

1. Place your logo image in `static/images/logo.png`
2. Uncomment line 40 in `templates/base.html`:
   ```html
   <img src="{{ url_for('static', filename='images/logo.png') }}" alt="Logo" height="40">
   ```

### Change Colors

Edit `static/css/style.css` (lines 2-7):
```css
:root {
    --primary-color: #667eea;     /* Main purple color */
    --primary-hover: #5568d3;     /* Hover state */
    --secondary-color: #764ba2;   /* Secondary purple */
    --bg-color: #f8f9fa;          /* Background color */
    --text-color: #2f2f2f;        /* Text color */
    --dark-bg: #1a1a1a;           /* Dark background */
}
```

### Replace Carousel Images

Edit `templates/index.html` (lines 9-21):
- Replace the Unsplash URLs with your own images
- Or place images in `static/images/` and update paths

### Update Portfolio Projects

Edit `templates/portfolio.html`:
- Replace placeholder images and descriptions
- Add your actual project screenshots
- Update project details

## Technologies Used

- **Backend**: Flask (Python)
- **Frontend**: HTML5, CSS3, JavaScript
- **Framework**: Bootstrap 5
- **Icons**: Font Awesome
- **Fonts**: System fonts (Segoe UI, etc.)

## Next Steps

1. **Add Real Content**: Replace placeholder text with your actual information
2. **Add Real Images**: Replace placeholder images with your own photos
3. **Set Up Email**: Configure the contact form to send emails
4. **Add Database**: Store contact form submissions
5. **Deploy**: Host on a production server
6. **Add Analytics**: Install Google Analytics
7. **SEO**: Optimize for search engines

## Support

For questions or issues, contact: contact@calahan-meredith.com

---

© 2025 Calahan-Meredith Web Development. All rights reserved.
