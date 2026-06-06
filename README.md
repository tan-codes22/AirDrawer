# AirDrawer 🎨✋

AirDrawer is a browser-based augmented reality drawing application that lets users draw in the air using hand gestures tracked through their webcam. Built with React, Vite, and MediaPipe, it enables touchless drawing and gesture-based interaction directly in the browser.

## Features

* Real-time hand tracking using webcam input
* Air drawing with hand gestures
* Gesture-based controls for drawing interactions
* Stroke management and canvas manipulation
* Responsive web interface
* No additional hardware required

## Tech Stack

* React
* Vite
* JavaScript (ES6+)
* MediaPipe Hand Tracking
* HTML5 Canvas
* CSS3

## Project Structure

```text
src/
├── components/
│   ├── CameraView.jsx
│   ├── ControlPanel.jsx
│   ├── DrawingCanvas.jsx
│   └── HelpPanel.jsx
│
├── modules/
│   ├── drawingEngine.js
│   ├── gestureController.js
│   ├── gestureInterpreter.js
│   ├── handTracking.js
│   ├── interactionEngine.js
│   ├── strokeManager.js
│   └── transformEngine.js
│
├── App.jsx
└── main.jsx
```

## Installation

### Prerequisites

* Node.js 18+
* npm 9+

### Clone the Repository

```bash
git clone https://github.com/tan-codes22/AirDrawer.git
cd AirDrawer/AirDrawer-main
```

### Install Dependencies

```bash
npm install
```

### Start Development Server

```bash
npm run dev
```

The application will start locally:

```text
http://localhost:5173
```

## Usage

1. Launch the application.
2. Allow camera permissions when prompted.
3. Position your hand within the camera frame.
4. Use supported gestures to begin drawing.
5. Use gesture controls to modify, move, or manipulate strokes.

## How It Works

The application processes webcam frames in real time and uses MediaPipe hand landmark detection to identify finger positions and gestures.

Workflow:

1. Webcam captures live video.
2. Hand tracking module detects landmarks.
3. Gesture interpreter classifies user actions.
4. Drawing engine converts gestures into strokes.
5. Canvas renders the resulting artwork.

## Available Scripts

### Start Development Server

```bash
npm run dev
```

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

### Run Linting

```bash
npm run lint
```

## Future Improvements

* Multi-hand collaborative drawing
* Shape recognition
* Gesture customization
* Save and export drawings
* Undo/redo functionality
* AI-assisted sketch enhancement
* AR object placement

## Troubleshooting

### Camera Not Working

* Ensure browser camera permissions are enabled.
* Close applications that may be using the webcam.
* Use the latest version of Chrome or Edge.

### Hand Tracking Not Detected

* Improve lighting conditions.
* Keep your hand fully visible in the camera frame.
* Maintain a reasonable distance from the webcam.

### Dependency Errors

```bash
rm -rf node_modules package-lock.json
npm install
```

## License

This project is intended for educational and experimental purposes.

## Author

Developed by Tanisha Gotadke.
