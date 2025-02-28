# Ambient

![Ambient Logo](https://img.shields.io/badge/Ambient-Real--time%20Object%20Detection-00FFFF?style=for-the-badge)

Ambient is a web-based real-time object detection system that leverages your device's camera to identify and categorize objects in your environment. Built with privacy in mind, all processing happens directly in your browser with no data transmitted to external servers.

## Features

- **Real-time object detection** using TensorFlow.js and the COCO-SSD model
- **Privacy-focused** - all processing happens locally in your browser
- **No installation required** - runs entirely in modern web browsers
- **Weapon detection alerts** with customizable confidence thresholds
- **Responsive design** that works across different devices
- **Simple, intuitive interface** with adjustable detection settings

## Demo

To try Ambient:

1. Clone this repository or download the HTML file
2. Open `index.html` in a modern web browser
3. Click "Start Camera" and grant camera permissions
4. Point your camera at objects to see real-time detection

## How It Works

Ambient uses TensorFlow.js to run the COCO-SSD (Common Objects in Context - Single Shot MultiBox Detection) model directly in your browser. This model can detect and classify 80 common object categories.

The application:
1. Accesses your camera with your permission via WebRTC
2. Processes video frames in real-time using TensorFlow.js
3. Identifies objects and their confidence scores
4. Draws bounding boxes around detected objects
5. Applies special highlighting for potentially dangerous items

## Special Weapon Detection

Ambient includes enhanced detection for potentially dangerous objects:
- Higher confidence threshold to minimize false positives
- Red highlighting and thicker bounding boxes
- Prominent warning notification
- Customizable detection sensitivity

## Privacy

Ambient is designed with privacy as a core principle:
- All processing occurs locally on your device
- No video or image data is stored or transmitted
- No server-side components or analytics
- Camera access requires explicit user permission

## Technical Details

This project uses:
- **TensorFlow.js** for in-browser machine learning
- **COCO-SSD model** pre-trained on a large dataset of common objects
- **WebRTC** / `getUserMedia` for camera access
- **HTML5 Canvas** for drawing detection overlays
- **Vanilla JavaScript** with no additional framework dependencies

## Browser Compatibility

Ambient works best in modern browsers that support WebRTC and JavaScript modules:
- Google Chrome (recommended)
- Microsoft Edge
- Firefox
- Safari

## Development

Want to modify or extend Ambient? The entire application is contained in a single HTML file making it easy to customize:

- Adjust detection thresholds in the initialization code
- Modify the list of weapon classes to detect additional items
- Change the visual styling through the CSS section
- Add new features by extending the JavaScript portion

## License

This project is released under the MIT License - see the LICENSE file for details.

## Acknowledgments

- TensorFlow.js team for enabling browser-based machine learning
- COCO-SSD model contributors
- Modern browser vendors for implementing WebRTC standards

---

Made with ❤️ for safer environments
