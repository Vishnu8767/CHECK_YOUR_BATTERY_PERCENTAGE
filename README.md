# Battery Status Checker 🔋

A simple, elegant web application that displays your device's battery percentage and charging status in real-time using the Battery Status API.

![Battery Checker Preview](https://img.shields.io/badge/Status-Active-brightgreen) ![HTML](https://img.shields.io/badge/HTML-5-orange) ![CSS](https://img.shields.io/badge/CSS-3-blue) ![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)

## ✨ Features

- **Real-time Battery Monitoring**: Displays current battery percentage with automatic updates
- **Visual Status Indicators**: Color-coded emojis representing different battery levels
- **Charging Detection**: Shows charging status with lightning bolt indicator
- **Responsive Design**: Clean, modern interface that works on all screen sizes
- **Browser Compatibility**: Works with browsers that support the Battery Status API

## 🎨 Design Highlights

- Gradient background with modern styling
- Clean white container with subtle shadow effects
- Dynamic emoji indicators based on battery level:
  - 🔋 Full battery (80%+)
  - 🟩 Medium battery (50-80%)
  - 🟨 Low battery (20-50%)
  - 🟥 Critical battery (below 20%)
  - ⚡ Charging indicator

## 🚀 Quick Start

### Option 1: Direct Download
1. Download or clone this repository
2. Open `index.html` in your web browser
3. Allow battery access permissions if prompted

### Option 2: Clone Repository
```bash
git clone https://github.com/Vishnu8767/battery-status-checker.git
cd battery-status-checker
open index.html
```

### Option 3: Live Demo
Simply open the HTML file in any modern web browser that supports the Battery Status API.

## 💻 Browser Support

The Battery Status API is supported in:
- ✅ Chrome (Android)
- ✅ Firefox (Desktop & Mobile)
- ✅ Opera
- ❌ Safari (not supported)
- ❌ iOS browsers (API restrictions)

**Note**: Due to privacy concerns, some browsers have limited or removed support for the Battery Status API.

## 🛠️ Technical Details

### File Structure
```
battery-status-checker/
│
├── index.html          # Main HTML file with embedded CSS and JavaScript
└── README.md           # Project documentation
```

### Key Technologies
- **HTML5**: Semantic structure and Battery API integration
- **CSS3**: Modern styling with gradients and flexbox layout
- **Vanilla JavaScript**: Battery API implementation and real-time updates

### Core Functionality
```javascript
// Main battery detection logic
if ('getBattery' in navigator) {
    navigator.getBattery().then(function(battery) {
        // Real-time battery monitoring
        function updateBatteryInfo() {
            const percent = (battery.level * 100).toFixed(0);
            const emoji = getBatteryEmoji(battery.level, battery.charging);
            // Update display with current status
        }
    });
}
```

## 🔧 Customization

You can easily customize the appearance by modifying the CSS variables:

- **Background Gradient**: Change the `background: linear-gradient()` property
- **Container Styling**: Modify padding, border-radius, and box-shadow
- **Colors**: Update the color scheme in the CSS section
- **Emojis**: Customize battery level indicators in the `getBatteryEmoji()` function

## 📱 Usage Examples

Perfect for:
- System monitoring dashboards
- Mobile web applications
- Educational projects about web APIs
- Battery awareness tools
- Kiosk applications

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Ideas for Contributions
- Add battery time remaining estimation
- Implement dark mode toggle
- Add more detailed battery information
- Create mobile app version
- Add battery health indicators

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Vishnu**
- GitHub: [@Vishnu8767](https://github.com/Vishnu8767)
- Feel free to reach out for questions or collaborations!

## 🙏 Acknowledgments

- Thanks to the web development community for Battery API documentation
- Inspired by the need for simple system monitoring tools
- Built with modern web standards and best practices


---

⭐ **Star this repository if you found it helpful!**

*Last updated: August 2025*
