# Abhishek Sinha - Personal Portfolio Website

A modern, responsive personal portfolio website showcasing professional experience, skills, and achievements in IT/Software Pre-Sales and Enterprise Architecture.

## 🌟 Features

- **Responsive Design**: Fully optimized for desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean white theme with professional blue accents
- **Interactive Elements**: Smooth animations, hover effects, and mobile-friendly navigation
- **Performance Optimized**: Fast loading with optimized images and efficient CSS
- **Cross-Browser Compatible**: Works seamlessly across all modern browsers
- **Touch-Friendly**: Optimized for mobile touch interactions

## 📱 Sections

1. **Hero Section**: Professional introduction with profile picture and social links
2. **About**: Personal background and professional summary
3. **Statistics**: Key career metrics and achievements
4. **Experience**: Detailed work history and accomplishments
5. **Skills**: Technical and professional competencies with progress indicators
6. **Education**: Academic background and qualifications
7. **Certifications**: Professional certifications and credentials
8. **Gallery**: Personal and professional photo collection
9. **Contact**: Multiple ways to get in touch

## 🛠️ Technologies Used

- **HTML5**: Semantic markup and modern web standards
- **CSS3**: Advanced styling with Flexbox, Grid, and responsive design
- **JavaScript**: Interactive functionality and mobile menu
- **Font Awesome**: Professional icons
- **Google Fonts**: Inter and Playfair Display typography

## 📂 Project Structure

```
theabhisheksinha.com/
├── index.html          # Main HTML file
├── pictures/           # Image assets
│   ├── Abhishek-Profile-noBG.png
│   ├── gallery images...
│   └── ...
└── README.md          # Project documentation
```

## 🚀 Getting Started

### Prerequisites

- A modern web browser
- Python 3.x (for local development server)
- Text editor or IDE

### Local Development

1. **Clone or download the project**
   ```bash
   git clone <repository-url>
   cd theabhisheksinha.com
   ```

2. **Start a local server**
   ```bash
   python3 -m http.server 8000
   ```

3. **Open in browser**
   Navigate to `http://localhost:8000`

### File Editing

- **Content Updates**: Edit the HTML content in `index.html`
- **Styling Changes**: Modify the CSS within the `<style>` tags
- **Images**: Replace images in the `pictures/` directory
- **Contact Info**: Update social links and contact details in the HTML

## 🌐 Deployment

### AWS S3 Static Website Hosting

1. **Create S3 Bucket**
   - Choose a unique bucket name
   - Uncheck "Block all public access"
   - Enable static website hosting

2. **Upload Files**
   - Upload `index.html` to bucket root
   - Upload `pictures/` folder maintaining structure

3. **Configure Bucket Policy**
   ```json
   {
     "Version": "2012-10-17",
     "Statement": [
       {
         "Sid": "PublicReadGetObject",
         "Effect": "Allow",
         "Principal": "*",
         "Action": "s3:GetObject",
         "Resource": "arn:aws:s3:::your-bucket-name/*"
       }
     ]
   }
   ```

4. **Access Website**
   Your site will be available at: `http://your-bucket-name.s3-website-region.amazonaws.com`

### Other Hosting Options

- **GitHub Pages**: Push to GitHub and enable Pages
- **Netlify**: Drag and drop deployment
- **Vercel**: Connect GitHub repository
- **Traditional Web Hosting**: Upload via FTP

## 📱 Mobile Optimization

The website includes comprehensive mobile optimization:

- **Responsive Breakpoints**: 1024px, 768px, 480px, 320px
- **Mobile Navigation**: Hamburger menu with smooth animations
- **Touch Optimization**: Proper touch targets and interactions
- **Performance**: Optimized for mobile networks
- **Typography**: Scalable fonts for all screen sizes

## 🎨 Customization

### Color Scheme
The website uses a professional white theme with blue accents:
- Primary: `#3182ce` (Blue)
- Background: `#f7fafc` (Light gray)
- Text: `#2d3748` (Dark gray)
- Cards: `#ffffff` (White)

### Typography
- **Headings**: Playfair Display (serif)
- **Body Text**: Inter (sans-serif)
- **Responsive**: Scales appropriately on all devices

### Images
- **Profile Picture**: `pictures/Abhishek-Profile-noBG.png`
- **Gallery**: Various personal and professional photos
- **Format**: JPEG and PNG supported
- **Optimization**: Images should be web-optimized for best performance

## 🔧 Browser Support

- Chrome 60+
- Firefox 60+
- Safari 12+
- Edge 79+
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📊 Performance Features

- **Optimized CSS**: Efficient selectors and minimal redundancy
- **Image Optimization**: Proper sizing and formats
- **Font Loading**: Optimized Google Fonts loading
- **Smooth Animations**: Hardware-accelerated transitions
- **Mobile Performance**: Touch-optimized interactions

## 🤝 Contributing

This is a personal portfolio website. For suggestions or improvements:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

This project is for personal use. Please respect the content and images.

## 📞 Contact

**Abhishek Sinha**
- **LinkedIn**: [theabhisheksinha](https://www.linkedin.com/in/theabhisheksinha/)
- **GitHub**: [theabhisheksinha](https://github.com/theabhisheksinha)
- **YouTube**: [@the.abhisheksinha](https://www.youtube.com/@the.abhisheksinha)

---

*Built with ❤️ using modern web technologies*