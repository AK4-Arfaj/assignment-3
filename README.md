# Alshayma Alarfaj - Portfolio Website

A modern, responsive portfolio website showcasing the work and interests of Alshayma Alarfaj, a Computer Science student at KFUPM. The site features a clean design with dark/light theme toggle, real-time clock animation, user authentication system, GitHub activity integration, and interactive sections highlighting skills, projects, and book recommendations.

## Features

- **Real-time Clock**: Animated typing effect displaying current time
- **Responsive Design**: Optimized for mobile, tablet, and desktop devices
- **Dark/Light Theme Toggle**: Persistent theme switching with system preference detection
- **User Authentication**: Signup/login system with persistent sessions and localStorage
- **User Profile**: Dynamic account age display updating in real-time
- **GitHub Activity Integration**: Public repositories showcase and activity heatmap
- **Interactive Sections**: About Me, Interests, Skills, Projects, Books, and Contact
- **Book Recommendations**: Personal reading list with sorting (by title, release date, author), search functionality, and "To Be Read" feature
- **Welcome Banner**: Dynamic greeting on login/signup with auto-hide after 5 seconds
- **Contact Form**: Frontend contact form with validation and toast notifications
- **Toast Notifications**: User feedback system for auth and form actions

## Technologies Used

- **HTML5**: Semantic markup and accessibility features
- **CSS3**: Responsive design with Flexbox/Grid, custom properties, and animations
- **JavaScript**: Theme management, real-time clock, authentication, and interactive features
- **GitHub API**: Integration with public repos and activity data
- **Web APIs**: localStorage for session persistence and book preferences
- **Google Fonts**: Poppins and Epilogue typography

## Setup Instructions

### Running Locally
1. **Download or Clone Repository**
   ```bash
   git clone https://github.com/AK4-Arfaj/assignment-2.git
   ```

2. **Open in Browser**
   - Navigate to the project folder
   - Right-click on `index.html` and select "Open with" your preferred browser
   - Alternatively, drag `index.html` into your browser window

3. **Navigate the Site**
   - Use the fixed navigation bar to jump between sections
   - Try the theme toggle button (sun/moon icon) to switch between light and dark modes
   - Click "Sign Up" to create an account or "Login" to access your account
   - Your account age is displayed dynamically in the navigation bar
   - Explore the GitHub activity section showing public repositories
   - Sort and search books by title, author, or release date
   - Add books to your "To Be Read" list and track your reading goals

### File Structure
```
├── index.html          # Main HTML file
├── css/
│   └── styles.css      # Responsive styling and themes
├── js/
│   └── script.js       # Interactive functionality
├── assets/
│   └── images/         # Photos and placeholder images
└── docs/
    └── technical-documentation.md
    └── ai-usage-report.md
```

## Browser Compatibility

- Modern browsers with CSS Grid and Flexbox support
- JavaScript enabled for theme toggle and clock functionality
- Responsive design tested on mobile, tablet, and desktop viewports

## Development Notes

- **Frontend Primary**: Mainly a frontend application with client-side authentication using localStorage
- **Contact Form**: Currently frontend-only, form submissions are not processed to a backend
- **Session Persistence**: User sessions are stored in browser localStorage (not production-grade security)
- **GitHub Integration**: Uses public GitHub API (no authentication required)
- **Book Covers**: Fetches book covers from multiple APIs (Google Books, Open Library)

## AI Usage Summary

AI tools (ChatGPT and GitHub Codex) were utilized for:
- Code debugging and optimization
- Implementation suggestions and best practices
- Feature development assistance

## Future Enhancements

- Backend integration for contact form processing and user data persistence
- Secure password hashing and proper authentication (bcrypt, JWT tokens)
- Project showcase with live demos and GitHub links
- Blog section for technical articles
- Enhanced animations and micro-interactions
- Email verification for user registration
- User profile customization and preferences
- Social media integration

## Live Demo

🔗 **Live Site**: TBD (Deployment pending)
