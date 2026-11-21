# 🎨 Imagify – AI-Powered Image Generator

Imagify is a full-stack AI-powered image generation platform that transforms text prompts into creative and high-quality images. It allows users to generate images using AI, manage their generation credits, and purchase additional credits through secure online payments.

The platform provides a simple and intuitive interface where users can explore their creativity by converting their ideas into AI-generated visuals.

## 🌟 Key Features

- **AI Image Generation:** Generate creative images from text descriptions using the Clipdrop API.
- **User Authentication:** Secure user registration and login functionality using JWT authentication.
- **Credit-Based System:** Users receive credits that are consumed when generating images.
- **Online Payment Integration:** Purchase additional credits securely through Razorpay.
- **User Dashboard:** Manage credits and access image generation functionality.
- **Image Preview:** View and download generated images.
- **Responsive Design:** Modern and responsive user interface for desktop and mobile devices.
- **RESTful APIs:** Backend APIs for authentication, image generation, and payment management.

## 🛠️ Tech Stack

### Frontend
- React.js – Component-based UI development.
- Vite – Fast development and build tooling.
- Tailwind CSS – Responsive styling.
- Axios – API communication.

### Backend
- Node.js – Server-side JavaScript runtime.
- Express.js – REST API development.
- MongoDB – Database for storing user and application data.
- Mongoose – MongoDB object modeling.
- JWT – Secure authentication and authorization.

### APIs & Integrations
- **Clipdrop API:** AI-powered image generation.
- **Razorpay:** Secure payment processing.

## 📂 Project Structure

```text
imagify/
│
├── client/                 # Frontend application
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   ├── pages/
│   │   └── App.jsx
│   └── package.json
│
├── server/                 # Backend application
│   ├── config/              # Database configuration
│   ├── controllers/         # API controllers
│   ├── middleware/          # Authentication middleware
│   ├── models/              # Database models
│   ├── routes/              # API routes
│   ├── server.js
│   └── package.json
│
└── README.md
```

## ⚙️ How It Works

1. Users register or log in to the platform.
2. Users enter a text prompt describing the image they want to generate.
3. The backend processes the request and communicates with the Clipdrop API.
4. The generated image is returned and displayed to the user.
5. Credits are deducted based on image generation usage.
6. Users can purchase additional credits through Razorpay when their balance is low.

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/faisalkhan8433/imagify.git
cd imagify
```

### 2. Install Frontend Dependencies

```bash
cd client
npm install
```

### 3. Install Backend Dependencies

```bash
cd ../server
npm install
```

### 4. Configure Environment Variables

Create a `.env` file inside the `server` directory:

```env
PORT=4000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLIPDROP_API=your_clipdrop_api_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
```

Create a `.env` file inside the `client` directory:

```env
VITE_BACKEND_URL=http://localhost:4000
```

Add your actual API keys and database credentials.

### 5. Run the Application

**Start Backend:**

```bash
cd server
npm run server
```

**Start Frontend:**

Open another terminal:

```bash
cd client
npm run dev
```

Open the local URL provided by Vite to access the application.

## 🔐 Security

- JWT-based authentication for protected routes.
- Environment variables for sensitive credentials.
- Backend-side API handling to protect secret keys.
- Payment verification through the backend.

## 🔮 Future Enhancements

- Support for multiple AI image generation models.
- Advanced image editing and customization.
- Image generation history and gallery.
- Multiple image resolution options.
- Social sharing and public image collections.

## 👨‍💻 Author

**Faisal Khan**

- GitHub: [@faisalkhan8433](https://github.com/faisalkhan8433)
- Project Repository: [Imagify](https://github.com/faisalkhan8433/imagify)

---

If you find this project useful or interesting, don't forget to ⭐ the repository!

**Built with ❤️ using React, Node.js and AI.**
