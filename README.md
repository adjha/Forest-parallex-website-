# 🌲 Forest Parallax Website

A stunning parallax scrolling website featuring a forest theme with smooth animations and interactive elements. Built with pure HTML, CSS, and JavaScript.

## 🌟 Features

- **Parallax Scrolling Effects**: Multiple layers move at different speeds creating depth
- **Smooth Animations**: Birds, forest elements, and text respond to scroll position
- **Responsive Design**: Optimized for various screen sizes
- **Modern UI**: Clean navigation with hover effects
- **Performance Optimized**: Lightweight and fast loading

## 🛠️ Technologies Used

- **HTML5** - Structure and content
- **CSS3** - Styling and animations
- **Vanilla JavaScript** - Parallax effects and interactions
- **Google Fonts** - Typography (Poppins & Rancho)

## 📁 Project Structure

```
forest-parallax-website/
│
├── index.html          # Main HTML file
├── style.css           # CSS styles and animations
├── script.js           # JavaScript for parallax effects
└── README.md           # Project documentation
```

## 🚀 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/forest-parallax-website.git
   ```

2. **Navigate to project directory**
   ```bash
   cd forest-parallax-website
   ```

3. **Open in browser**
   ```bash
   # Simply open index.html in your preferred browser
   # Or use a local server
   python -m http.server 8000
   # Then visit http://localhost:8000
   ```

## 🎨 Parallax Elements

The website includes several parallax layers:

| Element | Movement Direction | Speed Factor |
|---------|-------------------|--------------|
| Header | Downward | 0.5x |
| Main Text | Upward | -0.1x |
| Bird 1 | Up & Left | -1.5x, -5x |
| Bird 2 | Up & Right | -1.5x, 2x |
| Forest | Downward | 0.25x |
| Rocks | Upward | -0.12x |
| Explore Button | Downward | 1.5x |

## 🎯 How It Works

The parallax effect is achieved by:

1. **Scroll Event Listener**: JavaScript detects scroll position
2. **Transform Properties**: Elements are moved using CSS transforms
3. **Speed Variations**: Different elements move at different rates
4. **Layered Positioning**: Z-index creates depth perception

### Key JavaScript Code:
```javascript
window.addEventListener('scroll', function () {
    let value = window.scrollY;
    
    // Apply different movement speeds to create parallax
    text.style.top = 50 + value * -.1 + '%';
    bird1.style.left = value * -5 + 'px';
    bird2.style.left = value * 2 + 'px';
    // ... more transformations
});
```

## 🎨 Customization

### Colors
The project uses CSS custom properties for easy theming:
```css
:root {
    --primary: #094b65; /* Main theme color */
}
```

### Images
Replace the image URLs in `index.html` with your own:
- Bird images
- Forest background
- Rock formations
- Water elements

### Content
Modify the text content in the `.sec` section for your own project description.

## 📱 Browser Support

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

## 🔧 Performance Tips

1. **Optimize Images**: Compress images for faster loading
2. **Use WebP Format**: Modern image format for better compression
3. **Lazy Loading**: Implement lazy loading for images
4. **CSS Transforms**: Use transforms instead of changing layout properties

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📋 Future Enhancements

- [ ] Add more interactive elements
- [ ] Implement smooth scroll behavior
- [ ] Add mobile touch gestures
- [ ] Create additional sections
- [ ] Add loading animations
- [ ] Implement dark/light mode toggle




---

⭐ **Star this repo if you found it helpful!** ⭐
