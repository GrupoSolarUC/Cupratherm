# CupraTherm Website

A modern, responsive website for the CupraTherm project - Advanced Thermal Energy Storage Solutions.

## Overview

CupraTherm is a research project focused on developing innovative thermal energy storage technology for a sustainable future. This website serves as a platform to showcase the project's technology, motivation, pilot implementations, simulation results, control systems, and publications.

## Website Structure

The website is a single-page application with the following sections:

- **Home**: Hero section with project introduction
- **Technology Concept**: Overview of the CupraTherm technology and its key features
- **Motivation**: The driving factors behind the project including climate action, energy security, cost efficiency, and research excellence
- **Pilot Project**: Gallery of lab setup images and pilot specifications
- **Simulation Results**: Visual representation of thermal performance, efficiency analysis, and stability studies
- **Control System**: Details about the control architecture, components, and features
- **Publications**: Links to relevant research papers published by the team

## File Structure

```
CupraTherm-website/
├── index.html          # Main HTML file
├── css/
│   └── styles.css      # Main stylesheet
├── js/
│   └── main.js         # JavaScript functionality
├── images/             # Directory for images (add your lab photos here)
└── README.md           # This file
```

## How to Use

1. **View Locally**: Simply open `index.html` in a web browser
2. **Deploy**: Upload the files to any web hosting service

## Customization

### Adding Images

Replace the placeholder images by:
1. Add your images to the `images/` directory
2. Update the `<div class="placeholder-image">` elements in `index.html` with proper `<img>` tags

Example:
```html
<!-- Before -->
<div class="placeholder-image gallery-image">
    <span>Lab Setup 1</span>
</div>

<!-- After -->
<img src="images/lab-setup-1.jpg" alt="Lab Setup 1" class="gallery-image">
```

### Adding Publications

Update the publications section in `index.html` with your actual paper details:
- Publication title
- Author names
- Journal name
- Publication year
- Link to the paper

### Updating Content

All text content can be modified directly in `index.html`. The website uses semantic HTML making it easy to locate and update specific sections.

## Features

- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Smooth Scrolling**: Navigation links scroll smoothly to sections
- **Animated Elements**: Cards and gallery items fade in as you scroll
- **Modern Styling**: Clean, professional design with copper-themed colors reflecting the "Cupra" name

## Technologies Used

- HTML5
- CSS3 (with CSS Custom Properties)
- Vanilla JavaScript
- Google Fonts (Inter)

## Browser Support

The website supports all modern browsers including:
- Chrome
- Firefox
- Safari
- Edge

## Créditos y Licencia de Imágenes

Las imágenes, gráficos y material visual incluidos en este sitio web pertenecen al **Grupo Solar UC** (Pontificia Universidad Católica de Chile) y son de uso exclusivo para el proyecto de postulación CupraTherm. 

Queda prohibida su reproducción, distribución o uso fuera del contexto de este proyecto sin autorización expresa del Grupo Solar UC.

## License

© 2024 CupraTherm Project. All rights reserved.