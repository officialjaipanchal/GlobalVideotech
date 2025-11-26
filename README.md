# GlobalVideotech - Portfolio Website

A professional portfolio website for GlobalVideotech, a wedding photography and videography company based in Mehsana, Gujarat, India.

## 🎬 About

GlobalVideotech specializes in capturing life's most precious moments through professional photography and videography services. This website showcases their work and provides a platform for clients to get in touch.

### Services Offered
- Pre-Wedding Photography & Videography
- Marriage Photography
- Full Marriage Videography

## 🚀 Features

- **Responsive Design**: Fully responsive layout that works on all devices
- **Portfolio Showcase**: Display of recent work with modal popups
- **Contact Form**: Integrated contact form for client inquiries
- **Smooth Scrolling**: Smooth navigation between sections
- **Modern UI**: Clean and professional design using Bootstrap 4
- **Social Media Integration**: Links to social media profiles

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- [npm](https://www.npmjs.com/) (comes with Node.js)

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd GlobalVideoTech
   ```

2. **Install dependencies**
   ```bash
   npm install --ignore-scripts
   ```
   
   Note: The `--ignore-scripts` flag is used to skip the build process for `node-sass`, which has compatibility issues with newer Node.js versions. The CSS files are already compiled and ready to use.

## 🎯 Usage

### Development Server

Start the development server:

```bash
npm start
```

This will:
- Start an HTTP server on port 3001
- Automatically open the website in your default browser
- Serve the static files for local development

The website will be available at `http://localhost:3001`

### Build Tasks (Optional)

If you need to compile SCSS or minify JavaScript, you can use Gulp:

```bash
# Watch for changes and rebuild
npm run watch

# Or use Gulp directly
npx gulp build
```

**Note**: The Gulp build process requires `node-sass`, which may not work with Node.js v22+. The project uses `sass` (Dart Sass) as an alternative, but the Gulp configuration may need additional updates for full compatibility.

## 📁 Project Structure

```
GlobalVideoTech/
├── css/                 # Compiled CSS files
├── img/                 # Images and assets
│   ├── portfolio/      # Portfolio images
│   └── avataaars.svg    # Avatar image
├── js/                  # JavaScript files
├── mail/                # Contact form PHP handler
├── scss/                # Source SCSS files
├── vendor/              # Third-party libraries
│   ├── bootstrap/       # Bootstrap framework
│   ├── fontawesome-free/ # Font Awesome icons
│   └── jquery/          # jQuery library
├── index.html           # Main HTML file
├── package.json         # Node.js dependencies
├── gulpfile.js          # Gulp build configuration
└── README.md            # This file
```

## 🎨 Customization

### Updating Content

- **Company Information**: Edit `index.html` to update company details, location, and contact information
- **Portfolio Items**: Add or modify portfolio items in the "Our Work" section
- **About Section**: Update the motto and responsibilities in the About section
- **Contact Form**: Configure the contact form email in `mail/contact_me.php`

### Styling

- **Colors & Themes**: Modify SCSS variables in `scss/base/_variables.scss`
- **Layout**: Edit SCSS files in `scss/layout/` directory
- **Components**: Customize components in `scss/components/` directory

After making SCSS changes, compile them using:
```bash
npx gulp css
```

## 📧 Contact Form

The contact form requires a PHP server to function. The form handler is located in `mail/contact_me.php`. To configure:

1. Update the email address in `mail/contact_me.php` (line 19)
2. Ensure your server has PHP enabled
3. The form will send emails to the configured address

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 Technologies Used

- **HTML5**: Structure and content
- **CSS3/SCSS**: Styling and responsive design
- **Bootstrap 4.3.1**: CSS framework
- **jQuery 3.4.1**: JavaScript library
- **Font Awesome 5.10.2**: Icons
- **Gulp 4.0.2**: Build tool (optional)
- **http-server**: Development server

## 🔧 Troubleshooting

### Port Already in Use

If port 3001 is already in use, you can change it in `package.json`:
```json
"start": "http-server -p <your-port> -o"
```

### Node-sass Build Errors

If you encounter `node-sass` build errors, this is expected with newer Node.js versions. The project uses pre-compiled CSS files, so you can safely ignore these errors or use `npm install --ignore-scripts`.

### Gulp Watch Not Working

The Gulp watch task may not work due to `node-sass` compatibility issues. Use `npm start` instead, which uses `http-server` and doesn't require compilation.

## 📄 License

This project is based on the [Start Bootstrap Freelancer](https://startbootstrap.com/template-overviews/freelancer/) template, which is released under the MIT License.



**Copyright © GlobalVideotech 2020-2021**
