# Technical Documentation

## Overview
This is a personal portfolio website for Alshayma Alarfaj, a computer science student at KFUPM. The site is a single-page application featuring multiple sections including a real-time clock, personal information, interests, skills, projects, book recommendations, GitHub activity integration, and a contact form. The site includes responsive design, dark/light theme toggle, and a complete user authentication system with persistent sessions.

## File Structure
- `index.html` – Main document containing navigation, clock section, about me, interests, skills, projects, books, and contact form
- `css/styles.css` – Responsive styling with mobile-first design and dark mode support
- `js/script.js` – Theme toggle functionality and real-time clock with typing effects
- `assets/images/` – Personal photos and placeholder images for books and projects

## HTML Layout (`index.html`)
- `<nav>` provides fixed navigation with anchors to six main sections: About Me, Interests, Skills, Projects, Books, and Contact
- Dynamic auth buttons: "Login" and "Sign Up" visible when logged out, user info visible when logged in
- User profile display: username, account age (updated every second), and logout button
- Welcome banner: Slides in with "Welcome [username]!" or "Welcome Back [username]!" greeting, auto-hides after 5 seconds
- `<main>` contains seven primary `<section>` elements:
  - `#clock-section` displays a real-time clock with typing animation and hero image
  - `#about-me` contains personal introduction and profile information
  - `#interests` showcases four interest areas with icon cards (Web Development, App Development, Game Development, Cybersecurity)
  - `#skills` displays technical skills in a grid layout (HTML, CSS, JavaScript, React, SQL, R, Python, etc.)
  - `#github-activity` displays GitHub contribution heatmap and clickable repository cards
  - `#projects` features project showcase in a responsive grid
  - `#books` displays book recommendations with sorting dropdown, search functionality, release dates, and "Add to TBR" buttons
  - `#contact` contains a contact form with name, email, and message fields
- Auth modals: `#login-modal` and `#signup-modal` with form validation and error messages
- Auth overlay: Semi-transparent backdrop for modal focus
- Theme toggle button with SVG sun/moon icons for dark/light mode switching
- Toast notification container for user feedback

## Styling System (`css/styles.css`)
- Uses Google Fonts (Epilogue and Poppins) for typography
- Implements mobile-first responsive design with three breakpoints:
  - ≤599px: Single-column layout for mobile devices
  - 600-1024px: Tablet layout with adjusted spacing and grid layouts
  - ≥1025px: Desktop layout with centered content and expanded grids
- Dark mode implementation using `body.dark-mode` class
- Component-specific styling for cards, grids, forms, and interactive elements
- Smooth transitions for theme switching and hover effects
- **Auth Modal Styles**: 
  - `.auth-overlay`: Semi-transparent background with fade animation
  - `.auth-modal`: Centered modal with smooth slide-down animation
  - `.auth-form-group`: Form field layout with reduced label spacing (0.3rem margin-bottom)
  - `.auth-error`: Error message display with red text
- **Welcome Banner**: Gradient background with slide-down animation, 5-second display duration
- **GitHub Activity**: Heatmap grid visualization and clickable repository cards
- **Book Sorting**: Dropdown selector with light styling
- **Release Year Badges**: Styled inline-block badges for book metadata

## JavaScript Behavior (`js/script.js`)
- **Theme Toggle**: Detects system preferences, manages localStorage persistence, and applies dark/light mode
- **Real-time Clock**: Displays current time with typing/erasing animation effects, updates every second
- **Authentication System**:
  - User signup with email validation and duplicate checking
  - Login with email/password verification
  - Session persistence using localStorage (`user-session` and `app-users` keys)
  - Account creation timestamps stored in ISO format
  - Automatic session restoration on page load
- **User Profile**:
  - Dynamic account age calculation with plural/singular unit formatting (secs/mins/hours/days/months/years)
  - Real-time age display updated every second in navigation
  - Welcome banner display on login/signup (hidden on session restoration)
- **GitHub Integration**:
  - Fetches public repositories via GitHub REST API
  - Displays contribution heatmap based on recent activity
  - Clickable repository cards linking to GitHub
- **Book Management**:
  - Search functionality by title and keywords
  - Sorting options: alphabetical (A-Z), date (newest first), date (oldest first), author (A-Z)
  - Release year display for each book (1998-2023)
  - TBR (To Be Read) system with localStorage persistence
  - Book cover fetching from Google Books and Open Library APIs
- **Toast Notifications**: User feedback system for auth events, form submissions, and TBR actions
- **Form Handling**: 
  - Contact form validation and submission feedback
  - Form data persistence between page refreshes
  - Error message display with user guidance
- **Interactive Elements**: Handles all user interactions with smooth animations and transitions
- **Accessibility**: Maintains proper ARIA attributes and keyboard navigation support

## Key Features
- **Real-time Clock**: Animated clock display with typing effect showing current time
- **Responsive Design**: Optimized for mobile, tablet, and desktop viewing
- **Theme Toggle**: Persistent dark/light mode with system preference detection
- **User Authentication**: Complete signup/login system with session persistence
- **User Profile**: Dynamic account age display with real-time updates
- **GitHub Activity**: Public repository showcase and contribution visualization
- **Interactive Cards**: Hover effects on interest, skill, and repository cards
- **Book Recommendations**: 11 curated books with cover art, metadata, sorting, and TBR functionality
- **Welcome Banner**: Dynamic greeting message with auto-hide
- **Contact Form**: Form validation and status messaging (frontend only)
- **Toast Notifications**: Non-intrusive user feedback system

## Setup Instructions
1. Download or clone the repository
2. Open `index.html` in any modern web browser
3. Navigate using the fixed navigation bar at the top
4. Contact form is frontend-only (backend not implemented)

## Browser Compatibility
- Supports modern browsers with CSS Grid and Flexbox
- Requires JavaScript for theme toggle and clock functionality
- Uses CSS custom properties for theming

