
# Sprint05 Project

This project is a React application built with Vite. It showcases a tutorial card slider with responsive design, Tailwind CSS for styling, and animations for smooth transitions between cards.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)

## Features

- **React**: Utilizes React for building the user interface.
- **Responsive Design**: Ensures the application looks great on all devices.
- **Tailwind CSS**: Uses Tailwind CSS for styling and utility classes.
- **Animations**: Smooth transitions between tutorial cards using CSS animations.

## Installation

1. **Clone the repository**:
   ```sh
   git clone https://github.com/jorditer/5.1-Onboarding-digital-Nivell3.git
   cd Onboarding-digital-Nivell3
   ```

2. **Install dependencies**:
   ```sh
   npm install
   ```

3. **Run the development server**:
   ```sh
   npm run dev
   ```

## Usage

1. **Start the development server**:
   ```sh
   npm run dev
   ```

2. **Open your browser** and navigate to `http://localhost:3000` to see the application in action.

## Technologies Used

- **React**: A JavaScript library for building user interfaces.
- **Vite**: A fast build tool for modern web projects.
- **Tailwind CSS**: A utility-first CSS framework for rapid UI development.
- **CSS Animations**: Used for smooth transitions between tutorial cards.
- **Keyboard Navigation**: Use the left and right arrow keys to navigate through the cards.

## Detailed Explanation

### React

This project uses React to build the user interface. The main component is `App.jsx`, which renders the `Card` component.

### Responsive Design

The application is designed to be responsive, ensuring it looks great on all devices. Tailwind CSS utility classes are used to handle different screen sizes.

### Tailwind CSS

Tailwind CSS is used for styling the application. It provides utility classes for common CSS properties, making it easy to build responsive and consistent designs.

### Animations

CSS animations are used to create smooth transitions between tutorial cards. The animations are defined in the `input.css` file and applied conditionally in the `Card` component.

#### Example Animation

```css
@keyframes slideOutLeft {
  from {
    transform: translateX(0);
    opacity: 1;
  }
  to {
    transform: translateX(-100%);
    opacity: 0;
  }
}

@keyframes slideInRight {
  from {
    transform: translateX(100%);
    opacity: 0;
  }
  to {
    transform: translateX(0);
    opacity: 1;
  }
}

.slide-out-left {
  animation: slideOutLeft 0.5s forwards;
}

.slide-in-right {
  animation: slideInRight 0.5s forwards;
}
```

These animations are applied in the `Card` component to create a smooth sliding effect when navigating between tutorial steps.
```