# 👥 Facebook Clone - Full Stack Social Media Application

A fully responsive Facebook clone featuring authentication, home feed, post creation, stories, and interactive elements. Built with modern web technologies to replicate the core Facebook experience.

![Project Status](https://img.shields.io/badge/Status-Complete-brightgreen)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

## 🔗 Live Demo

[View Live Demo](https://facebook-clone-by-abdulrafay.vercel.app/)

## ✨ Features

### 🔐 **Authentication System**
- **Login Page**: Email/phone and password authentication
- **Sign Up Page**: Complete registration form with:
  - First name and surname fields
  - Email/mobile number input
  - Password creation
  - Date of birth selection
  - Gender selection (Male/Female/Other)
  - Terms and policy agreements
- **Password Recovery**: "Forgotten Password" link
- **Simple Authentication**: Hardcoded demo credentials for testing

### 🏠 **Home Feed Interface**
- **Navigation Bar**:
  - Facebook logo and search bar
  - Navigation icons (Home, Friends, Watch, Marketplace, Groups)
  - Messenger and notification icons with badges
  - Profile menu
  - Sticky header with dark theme

- **Left Sidebar**:
  - User profile section
  - Meta AI integration
  - Quick access menu (Friends, Memories, Saved, Groups, Video, Marketplace)
  - Shortcuts section with app icons
  - Sticky positioning

- **Center Content**:
  - Create post section with modal
  - Stories carousel
  - Dynamic posts feed
  - Image/video upload support
  - Post interactions (Like, Comment, Share)

- **Right Sidebar**:
  - Sponsored content section
  - Contacts list with online status
  - Video call and search options

### 📝 **Post Creation System**
- **Create Post Modal**:
  - Rich text area for post content
  - Privacy settings (Public, Friends, Only Me)
  - Photo/video upload with preview
  - Multiple file support
  - Post options (Tag people, Feelings, Check-in, Life events)
  - Character counter
  - Image preview with drag-and-drop

- **Post Features**:
  - Profile picture and name display
  - Timestamp generation
  - "See More/See Less" for long text (200+ characters)
  - Image galleries with responsive layouts
  - Post menu (ellipsis icon)

### 📖 **Stories Section**
- Horizontal scrollable stories carousel
- "Create Story" option
- Story preview with user avatars
- Hover effects and transitions
- Gradient overlays

### 💬 **Interactive Features**
- **Like System**:
  - Toggle like/unlike functionality
  - Real-time like counter
  - Color change on interaction
  
- **Share System**:
  - Share counter increment
  - Share animation

- **Comment System**:
  - Comment input boxes
  - Comment display with avatars
  - Reply and like on comments

### 🎨 **Design & UI**
- **Dark Theme**: Facebook's signature dark mode (#18191a background)
- **Responsive Design**: 
  - Desktop (3-column layout)
  - Tablet (2-column layout)
  - Mobile (single column with optimized navigation)
- **Modern Styling**:
  - Glassmorphism effects
  - Smooth transitions and hover states
  - Custom scrollbars
  - Shadow effects and depth
- **Accessibility**: Semantic HTML and proper ARIA labels

## 🚀 Technologies Used

### Frontend
- **HTML5**: Semantic markup structure
- **CSS3**: 
  - Flexbox and Grid layouts
  - CSS Variables
  - Custom animations
  - Media queries for responsiveness
- **JavaScript (ES6+)**:
  - DOM manipulation
  - Event handling
  - Dynamic content creation
  - Local state management
- **Bootstrap 5.3.0**: Modal components and utilities
- **Font Awesome 6.4.0**: Icon library

## 📦 Installation

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Code editor (VS Code recommended)
- Live Server extension (optional)

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/abdulrafay1402/FacebookClone.git
   cd FacebookClone
   ```

2. **Project Structure**
   ```
   FacebookClone/
   ├── index.html              # Login page
   ├── styles.css              # Login page styles
   ├── signup.html             # Sign up page
   ├── signupstyle.css         # Sign up page styles
   ├── home.html               # Main feed page
   ├── home.css                # Home page styles
   ├── app.js                  # JavaScript functionality
   ├── profile.jpg             # User profile image
   ├── metaAi.png             # Meta AI icon
   ├── candycrush.png         # Shortcut icons
   ├── angrybird.png
   ├── criminalcase.png
   └── README.md              # Project documentation
   ```

3. **Run the project**
   ```bash
   # Using VS Code Live Server
   Right-click on index.html → Open with Live Server
   
   # Or simply open in browser
   Double-click index.html
   ```

4. **Test Login**
   ```
   Email: abdulrafay1402@hotmail.com
   Password: abcd1234
   ```

## 🎯 Key Components

### Authentication Flow
```javascript
// Login validation in app.js
login() → Validates credentials → Redirects to home.html
```

### Post Creation
```javascript
createPost() → Captures text/files → Generates HTML → Updates feed
```

### Interactive Elements
```javascript
toggleLike() → Updates icon/count → Changes color
sharePost() → Increments share count
toggleText() → Expands/collapses long posts
```

## 📱 Responsive Breakpoints

| Device        | Width         | Layout Changes                    |
|---------------|---------------|-----------------------------------|
| Desktop       | > 1200px      | Full 3-column layout              |
| Large Tablet  | 992px - 1200px| 2-column layout, hidden center nav|
| Tablet        | 768px - 992px | Single column, compact navigation |
| Mobile        | < 768px       | Full mobile optimization          |
| Small Mobile  | < 576px       | Minimal UI, hidden elements       |

## 🎨 Color Palette

```css
/* Dark Theme */
--background: #18191a
--surface: #242526
--surface-hover: #3a3b3c
--text-primary: #e4e6eb
--text-secondary: #b0b3b8
--accent-blue: #2374e1
--accent-green: #42b72a
--accent-red: #e41e3f
```

## 🔧 Customization

### Adding New Posts
Posts are dynamically generated. Modify the `createPost()` function in `app.js` to customize post structure.

### Changing Theme
Update CSS variables in `home.css`:
```css
body {
  background: #your-color;
  color: #your-text-color;
}
```

### Adding Features
- Comments: Implement comment storage and display
- Reactions: Add different reaction types
- Real-time updates: Integrate WebSocket or polling
- Backend: Connect to database and API

## 🐛 Known Limitations

- **No Backend**: All data is stored in memory (resets on refresh)
- **No Database**: No persistent storage
- **Single User**: Hardcoded authentication
- **Static Content**: Stories and sponsored posts are placeholder data
- **No Real-time**: Updates require page refresh

## 🚀 Future Enhancements

- [ ] Backend integration (Node.js + Express)
- [ ] Database implementation (MongoDB/PostgreSQL)
- [ ] User authentication with JWT
- [ ] Real-time notifications
- [ ] Chat/Messenger functionality
- [ ] Profile pages
- [ ] Friend system
- [ ] News feed algorithm
- [ ] Image upload to cloud storage
- [ ] Video support
- [ ] Search functionality
- [ ] Settings and preferences

## 👨‍💻 Developer

**Abdul Rafay**  
🎓 Software Engineer  
💻 [GitHub Profile](https://github.com/abdulrafay1402)  
📧 Email: abdulrafay14021997@gmail.com

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/AmazingFeature`
3. Commit your changes: `git commit -m 'Add some AmazingFeature'`
4. Push to the branch: `git push origin feature/AmazingFeature`
5. Open a Pull Request

### Contribution Ideas
- Add backend functionality
- Implement user authentication
- Create additional pages (Profile, Groups, etc.)
- Improve mobile responsiveness
- Add unit tests
- Optimize performance
- Fix bugs and issues

## 📄 License

This project is for **educational purposes only**.

- Facebook® trademarks, design elements, and brand assets belong to **Meta Platforms, Inc.**
- This clone is created for **learning frontend development** and should not be used commercially
- Not affiliated with or endorsed by Meta/Facebook

## 🙏 Acknowledgments

- **Facebook/Meta** for the original design inspiration
- **Bootstrap** for modal components
- **Font Awesome** for icons
- **Picsum** and **RandomUser** for placeholder images
- Web development community for tutorials and resources

## 📸 Screenshots

### Login Page
Clean authentication interface with Facebook branding

### Home Feed
Full-featured social media feed with posts, stories, and navigation

### Post Creation
Rich modal interface for creating posts with media

### Responsive Design
Optimized layouts for all device sizes

---

## 🔍 Technical Details

### Browser Support
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Performance
- Lightweight CSS (no preprocessors)
- Vanilla JavaScript (no heavy frameworks)
- Optimized images
- Minimal dependencies

### Code Quality
- Semantic HTML5
- BEM-like CSS naming
- ES6+ JavaScript
- Commented code sections
- Responsive design patterns

---

⭐ **If you found this project helpful, please give it a star!**

📝 **Note**: This is a frontend demonstration project. For production use, implement proper backend, security, and data persistence.

---

*Built with ❤️ for learning web development*