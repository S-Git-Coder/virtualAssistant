
# AI Virtual Assistant (MERN Stack)

A full-stack AI-powered virtual assistant web application built with the MERN stack, featuring real-time voice recognition, natural language understanding (Google Gemini AI), and customizable assistant profiles.

## 🚀 Features

- **Voice Recognition & Speech Synthesis:** Interact with your assistant using your voice, powered by the Web Speech API.
- **AI Command Processing:** Google Gemini AI integration for smart command understanding and categorization.
- **Customizable Assistant:** Set your assistant’s name and avatar image.
- **Authentication:** Secure JWT-based authentication with HTTP-only cookies.
- **User History:** Persistent storage and display of user command history.
- **Cloud Image Upload:** Upload and store assistant images using Cloudinary.
- **Responsive UI:** Modern, mobile-friendly interface with Tailwind CSS.
- **Real-time Actions:** Supports Google search, YouTube, calculator, social media, weather, and more.

## 🛠️ Tech Stack

**Frontend:**  
- React.js (Vite)
- Tailwind CSS
- React Router
- Axios

**Backend:**  
- Node.js & Express.js
- MongoDB & Mongoose
- JWT, bcryptjs
- Multer (file uploads)
- Cloudinary (image storage)
- Google Gemini AI API

**Other:**  
- Web Speech API (Speech Recognition & Synthesis)
- Render (deployment)

## 📦 Project Structure

```
virtualAssistant/
│
├── backend/
│   ├── config/           # DB, Cloudinary, JWT config
│   ├── controllers/      # Auth & user logic
│   ├── middlewares/      # Auth, multer, etc.
│   ├── models/           # Mongoose schemas
│   ├── routes/           # API endpoints
│   ├── public/           # Static files
│   └── index.js          # Entry point
│
└── frontend/
    ├── public/           # Static assets
    └── src/
        ├── assets/       # Images, gifs
        ├── components/   # Reusable UI
        ├── context/      # React Context API
        ├── pages/        # Main pages (Home, SignIn, SignUp, Customize)
        ├── App.jsx       # Main app
        └── main.jsx      # Entry point
```

## ⚡ How It Works

1. **User Authentication:**  
   Users sign up and log in securely. JWT tokens are stored in HTTP-only cookies.

2. **Assistant Customization:**  
   Users set their assistant’s name and upload an image (stored on Cloudinary).

3. **Voice Interaction:**  
   The assistant listens for voice commands, processes them with Gemini AI, and responds with speech.

4. **Command Execution:**  
   The assistant can perform searches, open apps/websites, answer questions, and more.

5. **History:**  
   All user commands are saved and displayed for review.

## 🖥️ Getting Started

### Prerequisites

- Node.js & npm
- MongoDB Atlas or local MongoDB
- Cloudinary account
- Google Gemini AI API key

### Backend Setup

```bash
cd backend
npm install
# Create a .env file with your credentials:
# MONGODB_URI=your_mongodb_uri
# JWT_SECRET=your_jwt_secret
# CLOUDINARY_CLOUD_NAME=your_cloud_name
# CLOUDINARY_API_KEY=your_api_key
# CLOUDINARY_API_SECRET=your_api_secret
# GEMINI_API_URL=your_gemini_api_url
npm run dev
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

### Deployment

- The app is ready for deployment on platforms like Render, Vercel, or Netlify.

## 📸 Screenshots

- Home page with voice assistant and history
- Assistant customization page
- Sign in/up pages

## 🤖 AI Integration

- Uses Google Gemini AI for natural language understanding and command categorization.
- Supports commands like: “What’s the weather?”, “Open YouTube”, “Search React tutorials”, “What’s today’s date?”, etc.

## 📝 License

This project is open-source and available under the MIT License.

---

**Made with ❤️ using MERN, AI, and modern web technologies.**
