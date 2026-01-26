# Binary Upload Boom - Social Network

A full-stack social media application where users can share images, create posts, and interact through comments. Built as part of the 100Devs bootcamp curriculum, demonstrating modern web development practices with Node.js and MongoDB.

## 🌐 Live Demo

**[https://binary-upload-boom-d56c.onrender.com]**

## 🌐 Features

- **User Authentication** - Secure signup, login, and session management
- **Image Upload** - Upload and share images via Cloudinary integration
- **Social Posts** - Create, view, and manage posts with images
- **Comments System** - Interactive commenting on posts
- **Responsive Design** - Works seamlessly across all devices
- **Secure Sessions** - Protected routes and user data management

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** MongoDB with Mongoose ODM
- **Authentication:** Passport.js with local strategy
- **File Upload:** Multer with Cloudinary storage
- **Template Engine:** EJS
- **Session Management:** Express-session with MongoDB store
- **Styling:** CSS3
- **Development:** Morgan logging, Nodemon

## 📋 Project Structure

```
binary-upload-boom/
├── config/                 # Configuration files
│   ├── database.js        # MongoDB connection
│   └── passport.js        # Passport authentication config
├── controllers/           # Route handlers and business logic
│   ├── auth.js           # Authentication controllers
│   ├── comments.js       # Comment CRUD operations
│   ├── home.js           # Home page controller
│   └── posts.js          # Post CRUD operations
├── middleware/           # Custom middleware
│   ├── auth.js          # Authentication middleware
│   ├── cloudinary.js    # Cloudinary configuration
│   └── multer.js        # File upload middleware
├── models/              # Database schemas
│   ├── Comment.js       # Comment model
│   ├── Post.js          # Post model
│   └── User.js          # User model
├── public/              # Static assets
│   ├── css/
│   └── imgs/
├── routes/              # Express routes
│   ├── comments.js      # Comment routes
│   ├── main.js          # Main/auth routes
│   └── posts.js         # Post routes
├── views/               # EJS templates
│   ├── partials/        # Reusable template parts
│   └── *.ejs           # Page templates
└── server.js           # Main application entry point
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- MongoDB database
- Cloudinary account for image storage

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/binary-upload-boom
   cd binary-upload-boom
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Configuration**
   
   Create a `.env` file in the `config/` folder with the following variables:
   ```env
   PORT = 2121
   DB_STRING = your_mongodb_connection_string
   CLOUD_NAME = your_cloudinary_cloud_name
   API_KEY = your_cloudinary_api_key
   API_SECRET = your_cloudinary_api_secret
   ```

4. **Start the application**
   
   **Development mode:**
   ```bash
   npm run dev
   ```
   
   **Production mode:**
   ```bash
   npm start
   ```

5. **Open in browser**
   ```
   http://localhost:2121
   ```

## 🔧 Development

### Key Scripts

- `npm start` - Start production server
- `npm run dev` - Start development server with nodemon
- `npm test` - Run tests (currently not implemented)

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `PORT` | Server port number | Yes |
| `DB_STRING` | MongoDB connection URI | Yes |
| `CLOUD_NAME` | Cloudinary cloud name | Yes |
| `API_KEY` | Cloudinary API key | Yes |
| `API_SECRET` | Cloudinary API secret | Yes |

## 📱 Application Flow

1. **Homepage** - Landing page with login/signup options
2. **Authentication** - Secure user registration and login
3. **Feed** - View all posts from users
4. **Profile** - Personal dashboard with user's posts
5. **Create Post** - Upload images and create new posts
6. **Post Details** - View individual posts with comments
7. **Comments** - Add and view comments on posts

## 🎯 Key Features Implemented

- **MVC Architecture** - Clean separation of concerns
- **RESTful Routes** - Standard HTTP methods for CRUD operations
- **File Upload** - Secure image upload with validation
- **User Sessions** - Persistent login sessions
- **Password Hashing** - Secure password storage with bcrypt
- **Input Validation** - Server-side validation for all forms
- **Error Handling** - Comprehensive error management
- **Flash Messages** - User feedback for actions

## 🔒 Security Features

- **Password Encryption** - Bcrypt hashing
- **Session Security** - Secure session configuration
- **Route Protection** - Authentication middleware
- **Input Sanitization** - Mongoose validation
- **File Upload Security** - Multer file filtering

## 🌟 Learning Objectives

This project demonstrates:
- **Full-stack Development** - Complete CRUD application
- **Database Integration** - MongoDB with Mongoose
- **Authentication Systems** - Passport.js implementation
- **File Upload Handling** - Image processing and storage
- **Template Rendering** - Server-side rendering with EJS
- **Middleware Usage** - Custom and third-party middleware
- **RESTful API Design** - Standard REST principles

## � Future Improvements

Given more development time, I would implement the following enhancements:

### Core Features
- **Real-time Messaging** - Chat system between users using Socket.io
- **Like/Dislike System** - Interactive voting on posts and comments
- **Follow/Following** - Social connections between users
- **Image Filters** - Built-in photo editing capabilities
- **Video Upload** - Support for video content alongside images
- **Stories Feature** - Temporary 24-hour content sharing

### User Experience
- **Dark Mode Toggle** - Theme switching functionality
- **Advanced Search** - Filter posts by user, tags, or date
- **Infinite Scroll** - Seamless content loading
- **Push Notifications** - Real-time alerts for interactions
- **Mobile App** - React Native companion app
- **Email Notifications** - Digest emails for activity

### Technical Enhancements
- **API Documentation** - Swagger/OpenAPI integration
- **Caching Layer** - Redis implementation for performance
- **Image Optimization** - Automatic compression and resizing
- **Rate Limiting** - API abuse prevention
- **Two-Factor Authentication** - Enhanced security
- **Microservices Architecture** - Service separation for scalability

### Analytics & Admin
- **Admin Dashboard** - Content moderation panel
- **Analytics Dashboard** - User engagement metrics
- **Content Reporting** - Community moderation tools
- **Backup System** - Automated data backup strategies

## �📧 Contact

- **Email:** [jackgermainbusiness@gmail.com](mailto:jackgermainbusiness@gmail.com)
- **LinkedIn:** [linkedin.com/in/jack-germain](https://www.linkedin.com/in/jack-germain/)
- **GitHub:** [github.com/JackGer26](https://github.com/JackGer26)

## 📄 License

This project is licensed under the MIT License.

---

**Built with ❤️ as part of 100Devs**
