# ASCII: Custom ASCII Art Generator

A modern, responsive web application for generating ASCII art from images with advanced customization options.

![image](https://github.com/user-attachments/assets/53f186da-b1d8-4e82-a7f4-96da62d512ce)


## Features

- **Image to ASCII Conversion**: Transform any image into detailed ASCII art
- **Multiple Dithering Algorithms**: Floyd-Steinberg, Atkinson, Noise, and Ordered dithering
- **Edge Detection Options**: Sobel edge detection and DoG (Difference of Gaussians) contour detection
- **Theme Support**: Toggle between dark and light modes
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Various Character Sets**: Detailed, standard, blocks, binary, hexadecimal, and custom characters
- **Advanced Image Adjustments**: Controls for brightness, contrast, blur, and color inversion
- **Export Options**: Copy to clipboard or download as PNG

## Architecture

### Frontend Technology Stack

- **HTML5**: Semantic markup for better accessibility and SEO
- **CSS3**: Modern styling with CSS variables for theming
- **JavaScript (ES6+)**: Client-side processing without external dependencies
- **Canvas API**: For efficient image manipulation and processing

### Core Components

1. **Image Processing Engine**:
   - Direct pixel manipulation using Canvas API
   - Grayscale conversion with luminance weighting (0.299R + 0.587G + 0.114B)
   - Implementation of multiple dithering algorithms
   - Edge detection using Sobel operators and Difference of Gaussians

2. **UI Framework**:
   - CSS custom properties for consistent theming
   - Flexbox layout for responsive design
   - Custom form controls with enhanced accessibility

3. **File Handling System**:
   - HTML5 File API for image uploads
   - Drag-and-drop functionality
   - Client-side image processing
   - Export capabilities (copy to clipboard, PNG download)

## Responsiveness Optimizations

The application is carefully optimized for various device sizes:

### Desktop (>991px)
- Full sidebar view with all controls permanently visible
- Horizontal layout with controls on the left and output on the right
- Precise controls optimized for mouse input
- Scrollable output area with adjustable zoom

### Tablet (768px-991px)
- Collapsible sidebar that slides in from the left
- Hamburger menu toggle in the top left
- Close (X) button in the top right of the sidebar
- Overlay background when sidebar is open
- Collapse All/Expand All functionality for sections
- Optimized touch targets for better usability

### Mobile (<768px)
- Full-width, vertically stacked layout
- Touch-optimized controls with larger hit areas
- Enhanced padding in the header for better thumb accessibility
- Full-width buttons for easier tapping
- Simplified control sections with collapsible panels
- Optimized scrolling behavior

### Common Responsive Features
- Fluid typography that scales with the viewport
- Flexible image containers
- Media queries for targeted styling at different breakpoints
- Touch-friendly UI elements
- Adaptive layout changes based on available screen space

## Installation

No installation required! This is a fully client-side application:

1. Clone the repository
2. Open `index.html` in any modern browser
3. Start generating ASCII art!

## Usage

1. Upload an image using the file picker or drag-and-drop
2. Adjust the settings in the control panel to customize your ASCII art
3. Use the zoom control to view at different sizes
4. Copy to clipboard or download as PNG

![og-ascii](https://github.com/user-attachments/assets/5b4cef3a-471c-4de5-be40-9d06bc1c1eaa)


## License

Copyright 2025 DrBaph, UK

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License. 
