# Recipe Page - Frontend Mentor Challenge

A responsive recipe page built with HTML and CSS for the Frontend Mentor challenge. This project displays a simple omelette recipe with preparation time, ingredients, instructions, and nutritional information.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Code Documentation](#code-documentation)
- [Responsive Design](#responsive-design)
- [Browser Support](#browser-support)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This is a solution to the [Frontend Mentor Recipe Page challenge](https://www.frontendmentor.io/challenges/recipe-page-FdpiXDJQ). The goal was to build a responsive recipe page that matches the provided design files and works across different screen sizes.

### Design Files

- `design/desktop-design.jpg` - Desktop layout reference
- `design/mobile-design.jpg` - Mobile layout reference
- `style-guide.md` - Design specifications and color palette

## ✨ Features

- **Responsive Design**: Adapts to desktop, tablet, and mobile screens
- **Semantic HTML**: Proper use of HTML5 semantic elements
- **Modern CSS**: Flexbox layout and CSS Grid for responsive design
- **Typography**: Google Fonts integration (Outfit and Young Serif)
- **Accessibility**: Alt text for images and semantic markup
- **Preparation Time Section**: Full-width background section that extends beyond card boundaries

## 📁 Project Structure

```
recipe-page-main/
├── assets/
│   ├── fonts/
│   │   ├── outfit/          # Outfit font family
│   │   └── young-serif/     # Young Serif font
│   └── images/
│       ├── favicon-32x32.png
│       └── image-omelette.jpeg
├── design/
│   ├── desktop-design.jpg
│   ├── mobile-design.jpg
│   └── style-guide.md
├── index.html              # Main HTML file
├── style.css              # Main CSS file
├── preview.jpg            # Project preview
└── README.md              # This file
```

## 🛠 Technologies Used

- **HTML5**: Semantic markup and structure
- **CSS3**: Styling and responsive design
- **Google Fonts**: Typography (Outfit and Young Serif)
- **Flexbox**: Layout system for centering and alignment

## 🚀 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/recipe-page.git
   cd recipe-page
   ```

2. Open the project:
   - Open `index.html` in your web browser
   - Or use a local development server

## 📖 Usage

Simply open `index.html` in any modern web browser to view the recipe page. The page is fully responsive and will adapt to different screen sizes.

## 📚 Code Documentation

### HTML Structure

#### Main Container

```html
<body class="overall-body">
  <div class="card">
    <!-- Recipe content -->
  </div>
</body>
```

#### Key Sections

1. **Header**: Recipe image and title
2. **Description**: Recipe overview
3. **Preparation Time**: Full-width background section
4. **Ingredients**: List of required ingredients
5. **Instructions**: Step-by-step cooking instructions
6. **Nutrition**: Nutritional information table

### CSS Architecture

#### Layout System

- **Flexbox**: Used for centering the main card and nutrition table layout
- **Responsive Units**: Mix of px, rem, and % for different purposes
- **Card-based Design**: Main content contained in a white card with rounded corners

#### Key CSS Classes

##### Layout Classes

- `.overall-body`: Main container with background and centering
- `.card`: Main content container with white background
- `.card-img`: Recipe image styling

##### Content Classes

- `.card-title`: Main recipe title (Young Serif font)
- `.card-description`: Recipe description text
- `.card-subtitle-div`: Preparation time section with full-width background
- `.Ingredients`, `.Instructions`, `.Nutrition`: Section containers

##### Typography Classes

- `.card-title`, `.Ingredients-title`, `.Instructions-title`, `.Nutrition-title`: Section headings
- `.card-description`, `.Nutrition-description`: Body text
- `.Ingredients-list`, `.Instructions-list`: List styling

#### Color Scheme

```css
/* Primary Colors */
--color-primary: hsl(14, 45%, 36%); /* Brown text */
--color-secondary: #991b47; /* Pink accent */
--color-background: #f5f5dc; /* Beige background */
--color-card-bg: #fff5f9; /* Light pink */
--color-border: #f5f5dc; /* Border color */
```

#### Typography

- **Primary Font**: "Outfit" (sans-serif) - Used for body text and descriptions
- **Secondary Font**: "Young Serif" (serif) - Used for headings and titles

## 📱 Responsive Design

### Breakpoints

The design uses multiple breakpoints for responsive behavior:

1. **Desktop (Default)**: 40% width card
2. **Large Tablet (≤1061px)**: 70% width
3. **Medium Tablet (≤1004px)**: 80% width
4. **Small Tablet (≤925px)**: 90% width
5. **Mobile (≤502px)**: 100px width (appears to be a typo)
6. **Small Mobile (≤444px)**: Special preparation time section styling

### Responsive Features

- **Fluid Typography**: Font sizes adjust for different screen sizes
- **Flexible Layout**: Card width adapts to screen size
- **Mobile-First**: Preparation time section extends full-width on mobile
- **Touch-Friendly**: Adequate spacing for mobile interaction

### Media Queries

```css
@media (max-width: 444px) {
  /* Small mobile adjustments */
}

@media (max-width: 502px) {
  /* Mobile layout */
}

@media (max-width: 925px) {
  /* Small tablet */
}

@media (max-width: 1004px) {
  /* Medium tablet */
}

@media (max-width: 1061px) {
  /* Large tablet */
}
```

## 🎨 Design System

### Spacing

- **Small**: 6px, 10px, 20px
- **Medium**: 25px, 30px, 35px
- **Large**: 40px, 100px (margins)

### Border Radius

- **Default**: 14px for cards and images

### Typography Scale

- **Large Headings**: 35px (card title)
- **Section Headings**: 25px
- **Body Text**: 16px
- **Small Text**: 11px (attribution)

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🔧 Known Issues

1. **Mobile Breakpoint**: The 502px breakpoint sets card width to 100px, which appears to be a typo
2. **Font Weight**: Some font-weight declarations use `px` instead of numeric values
3. **Inconsistent Units**: Mix of px, rem, and % without clear reasoning
4. **Magic Numbers**: Hardcoded breakpoint values without semantic meaning

## 🚀 Future Improvements

- [ ] Fix mobile breakpoint typo (502px → 100%)
- [ ] Consolidate media queries into logical breakpoints
- [ ] Implement CSS custom properties for better maintainability
- [ ] Add hover effects and transitions
- [ ] Improve accessibility with ARIA labels
- [ ] Add print styles
- [ ] Implement dark mode
- [ ] Add loading states and animations

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**x100-logical0z**

- Frontend Mentor Profile: [@x100-logical0z](https://www.frontendmentor.io/profile/x100-logical0z)

## 🙏 Acknowledgments

- [Frontend Mentor](https://www.frontendmentor.io/) for the challenge
- [Google Fonts](https://fonts.google.com/) for the typography
- The Frontend Mentor community for feedback and support

---

**Note**: This is a solution to a Frontend Mentor challenge. The design files and requirements are provided by Frontend Mentor.
