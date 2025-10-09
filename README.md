# 🚀 CodeVerse

**A Modern Online Code Editor & Execution Platform**

CodeVerse is a full-stack web application that allows users to write, execute, save, and collaborate on code in multiple programming languages. Built with React and Node.js, it features real-time collaboration, user authentication, and code snippet management.

![CodeVerse Preview](https://img.shields.io/badge/Status-Production%20Ready-brightgreen)
![License](https://img.shields.io/badge/License-MIT-blue)
![Node.js](https://img.shields.io/badge/Node.js-18%2B-green)
![React](https://img.shields.io/badge/React-18.3-blue)

---

## ✨ Features

### 💻 **Code Execution**
- **Multi-language Support**: JavaScript, Java, Python, C, C++, Go, Ruby, TypeScript, PHP
- **Real-time Execution**: Instant code compilation and execution
- **Custom Input**: Support for program input via interactive modal
- **Execution Timer**: Performance monitoring for code execution

### 🎨 **Modern UI/UX**
- **Monaco Editor**: VS Code-like editing experience with syntax highlighting
- **Dark/Light Mode**: Toggle between themes
- **Responsive Design**: Works seamlessly on desktop and mobile
- **Glass-morphism UI**: Modern, elegant interface design

### 👥 **Collaboration Features**
- **Real-time Collaboration**: Multiple users can edit code simultaneously
- **WebSocket Integration**: Live synchronization using Yjs and Socket.IO
- **Room-based Sessions**: Create or join collaboration rooms
- **User Awareness**: See other users' cursors and selections

### 🔐 **User Management**
- **JWT Authentication**: Secure user registration and login
- **Profile Management**: User profiles with photo upload support
- **Password Security**: Bcrypt hashing for secure password storage

### 📚 **Code Management**
- **Save Snippets**: Save code with custom titles and descriptions
- **History Tracking**: View and manage previously saved code
- **Code Sharing**: Generate shareable links for code snippets
- **Snippet Templates**: Pre-built code examples for quick start

### 🛡️ **Security & Performance**
- **Rate Limiting**: API protection against abuse
- **Input Validation**: Comprehensive data validation
- **Error Handling**: Robust error management
- **File Cleanup**: Automatic temporary file management

---

## 🛠️ Technology Stack

### **Frontend**
| Technology | Version | Purpose |
|------------|---------|---------|
| React | 18.3.1 | UI Framework |
| Vite | 6.3.5 | Build Tool & Dev Server |
| Monaco Editor | 4.7.0 | Code Editor |
| Axios | 1.9.0 | HTTP Client |
| Socket.IO Client | 4.8.1 | Real-time Communication |
| Yjs | 13.6.27 | Collaborative Editing |
| Heroicons | 2.2.0 | Icons |

### **Backend**
| Technology | Version | Purpose |
|------------|---------|---------|
| Node.js | 18+ | Runtime Environment |
| Express | 5.1.0 | Web Framework |
| MongoDB | 8.7.0 | Database |
| Socket.IO | 4.8.1 | WebSocket Server |
| JWT | 9.0.2 | Authentication |
| Bcrypt | 5.1.1 | Password Hashing |
| Multer | 2.0.0 | File Upload |
| UUID | 11.1.0 | Unique ID Generation |

---

## 🚀 Quick Start

### **Prerequisites**
- Node.js 18+ and npm
- MongoDB (local installation or MongoDB Atlas)
- Git

### **Installation**

1. **Clone the repository**
   ```bash
   git clone https://github.com/krishyadav90/CODING-PLATFORM.git
   cd CODING-PLATFORM
   ```

2. **Setup Backend**
   ```bash
   cd backend
   npm install
   ```

3. **Setup Frontend**
   ```bash
   cd ../frontend
   npm install
   ```

4. **Environment Configuration**
   
   Create `backend/.env` file:
   ```env
   MONGO_URI=mongodb://localhost:27017/coding-platform
   JWT_SECRET=your_super_secret_jwt_key_here
   PORT=5000
   ```

5. **Start Development Servers**
   
   **Backend** (Terminal 1):
   ```bash
   cd backend
   npm run dev
   ```
   
   **Frontend** (Terminal 2):
   ```bash
   cd frontend
   npm run dev
   ```

6. **Access the Application**
   - Frontend: [http://localhost:5173](http://localhost:5173)
   - Backend API: [http://localhost:5000](http://localhost:5000)

---

## 📁 Project Structure

```
CodeVerse/
├── backend/                 # Express.js Backend
│   ├── index.js            # Main server file
│   ├── package.json        # Backend dependencies
│   ├── tsconfig.json       # TypeScript configuration
│   ├── Dockerfile          # Docker configuration
│   └── .env                # Environment variables
│
├── frontend/               # React Frontend
│   ├── src/
│   │   ├── App.jsx         # Main application component
│   │   ├── main.jsx        # Entry point
│   │   ├── snippets.js     # Code templates
│   │   ├── useNotification.jsx # Custom hook
│   │   └── [Modal Components] # UI modals
│   ├── index.html          # HTML template
│   ├── vite.config.js      # Vite configuration
│   └── package.json        # Frontend dependencies
│
└── README.md               # Documentation
```

---

## 🔌 API Endpoints

### **Authentication**
- `POST /register` - User registration
- `POST /login` - User login
- `GET /profile` - Get user profile

### **Code Management**
- `POST /run` - Execute code
- `POST /save-code` - Save code snippet
- `GET /history` - Get user's code history
- `DELETE /delete-snippet/:id` - Delete code snippet

### **Sharing & Collaboration**
- `POST /share-code` - Create shareable link
- `GET /share/:shareId` - Access shared code
- `POST /collaborate` - Create collaboration room
- `POST /collaborate/join` - Join collaboration room

### **File Upload**
- `POST /upload-profile-photo` - Upload profile picture

---

## 🎯 Supported Languages

| Language | Compiler/Runtime | File Extension |
|----------|------------------|----------------|
| JavaScript | Node.js | `.js` |
| TypeScript | ts-node | `.ts` |
| Java | javac + java | `.java` |
| Python | python3 | `.py` |
| C | gcc | `.c` |
| C++ | g++ | `.cpp` |
| Go | go run | `.go` |
| Ruby | ruby | `.rb` |
| PHP | php | `.php` |

---

## 🚢 Production Deployment

### **Environment Variables**
```env
NODE_ENV=production
MONGO_URI=mongodb+srv://username:password@cluster.mongodb.net/codeverse
JWT_SECRET=your_production_jwt_secret
PORT=5000
```

### **Build Commands**
```bash
# Frontend build
cd frontend && npm run build

# Backend start
cd backend && npm start
```

### **Docker Support**
```bash
# Build and run with Docker
docker build -t codeverse-backend ./backend
docker run -p 5000:5000 codeverse-backend
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Krishna Yadav**
- GitHub: [@krishyadav90](https://github.com/krishyadav90)
- Repository: [CODING-PLATFORM](https://github.com/krishyadav90/CODING-PLATFORM)

---

## 🙏 Acknowledgments

- Monaco Editor for the powerful code editing experience
- Yjs for real-time collaborative editing
- MongoDB for reliable data storage
- React ecosystem for modern UI development

---

## 🐛 Known Issues & Roadmap

### **Current Known Issues**
- Large bundle size warning (can be optimized with code splitting)
- TypeScript execution requires ts-node dependency

### **Future Enhancements**
- [ ] Code formatting and auto-completion
- [ ] Plugin system for custom languages
- [ ] Advanced collaboration features (comments, chat)
- [ ] Code execution analytics
- [ ] Mobile app version
- [ ] Integration with GitHub/GitLab

---

<div align="center">

**⭐ Star this repository if you found it helpful!**

[Report Bug](https://github.com/krishyadav90/CODING-PLATFORM/issues) · [Request Feature](https://github.com/krishyadav90/CODING-PLATFORM/issues) · [Documentation](https://github.com/krishyadav90/CODING-PLATFORM/wiki)

</div>