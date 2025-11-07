# Garage Sale Website

A simple, responsive static website for showcasing garage sale items with images.

## Features

- Responsive image gallery that works on desktop, tablet, and mobile
- Clean, modern design with hover effects
- Easy to customize and add new items
- GitHub Pages ready

## Setup Instructions

### 1. Add Your Images

1. Place all your item photos in the `images/` directory
2. Name them descriptively (e.g., `coffee-maker.jpg`, `bike.jpg`, `bookshelf.jpg`)
3. Supported formats: JPG, PNG, GIF, WebP

### 2. Customize the Content

Edit `index.html` to:

- Update the sale date, time, and location
- Add your contact email
- Add items to the gallery by copying the gallery-item template:

```html
<div class="gallery-item">
    <img src="images/your-item.jpg" alt="Description">
    <div class="item-info">
        <h3>Item Name</h3>
        <p class="price">$XX.XX</p>
        <p class="description">Brief description of the item</p>
    </div>
</div>
```

### 3. Deploy to GitHub Pages

#### Option A: Via GitHub Website

1. Create a new repository on GitHub
2. Upload all files (index.html, styles.css, images folder, README.md)
3. Go to Settings > Pages
4. Under "Source", select "Deploy from a branch"
5. Select the `main` branch and `/ (root)` folder
6. Click Save
7. Your site will be available at: `https://[username].github.io/[repository-name]`

#### Option B: Via Command Line

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Garage sale website"

# Add your GitHub repository as remote
git remote add origin https://github.com/[username]/[repository-name].git

# Push to GitHub
git branch -M main
git push -u origin main
```

Then follow steps 3-7 from Option A.

## Local Testing

To test locally, you can use any local web server. Here are a few options:

### Python 3
```bash
python3 -m http.server 8000
```

### Python 2
```bash
python -m SimpleHTTPServer 8000
```

### Node.js (with npx)
```bash
npx serve
```

Then open `http://localhost:8000` in your browser.

## Customization Tips

### Change Colors

Edit `styles.css` to customize colors:
- Header gradient: Lines 13-14
- Accent color: Search for `#667eea` and replace
- Price color: Line 115 (currently green `#28a745`)

### Add More Information

You can add additional sections to `index.html` such as:
- Payment methods accepted
- Parking information
- Special instructions

### Image Optimization

For faster loading, consider:
- Resizing images to max 1200px width
- Compressing images with tools like TinyPNG or ImageOptim
- Using WebP format for better compression

## File Structure

```
garagesale/
├── index.html          # Main HTML file
├── styles.css          # Stylesheet
├── images/             # Directory for item photos
│   └── .gitkeep        # Placeholder to track empty directory
└── README.md           # This file
```

## Browser Support

Works on all modern browsers including:
- Chrome/Edge
- Firefox
- Safari
- Mobile browsers

## License

Feel free to use and modify this template for your own garage sale or similar purposes.
