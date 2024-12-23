# Smart Job Portal AI Project

This README provides an overview of the Smart Job Portal AI Project, including its backend, frontend, and Android application components. Each section details the work done so far and the technologies used.

---

## **Backend**

### **Technologies Used**
- **Node.js**: Backend runtime environment
- **Express.js**: Web framework for building REST APIs
- **MongoDB**: NoSQL database for data storage
- **OpenAI API**: For chatbot functionality
- **JWT**: For user authentication
- **Styled Components**: For email styling

### **Key Features Implemented**
1. **User Authentication**:
   - User login and signup with secure password hashing using bcrypt.
   - Token-based authentication using JWT.

2. **Chatbot API**:
   - Integrated OpenAI API to implement an intelligent chatbot interface.
   - Dynamic responses based on user input.

3. **Job Management**:
   - API endpoints for CRUD operations on job listings.
   - Filtering and search functionalities for job seekers.

4. **Database Integration**:
   - MongoDB setup with schema models for Users, Jobs, and Chat sessions.
   - Dummy data seeded into the database for testing.

5. **Error Handling**:
   - Centralized error-handling middleware for better debugging.

### **Directory Structure**
```
backend/
├── src/
│   ├── controllers/
│   │   ├── authController.js
│   │   ├── chatController.js
│   │   └── jobController.js
│   ├── models/
│   │   ├── User.js
│   │   ├── Job.js
│   │   └── ChatSession.js
│   ├── routes/
│   │   ├── auth.js
│   │   ├── chat.js
│   │   └── jobs.js
│   ├── middleware/
│   │   └── authMiddleware.js
│   └── app.js
├── config/
│   └── dbConfig.js
└── server.js
```

---

## **Frontend**

### **Technologies Used**
- **React.js**: Frontend library for building the user interface
- **Styled Components**: For modern and reusable styling
- **Axios**: For API calls
- **React Router**: For navigation

### **Key Features Implemented**
1. **Login and Signup Pages**:
   - User-friendly forms styled with Styled Components.
   - Integrated with backend APIs for authentication.

2. **Job Listings**:
   - Dynamic rendering of job cards fetched from the backend.
   - Search and filter options to narrow down job searches.

3. **Chatbot Interface**:
   - Chat interface designed using Styled Components.
   - Real-time integration with the chatbot API.

4. **Responsive Design**:
   - Mobile-first design for compatibility across devices.
   - CSS media queries for responsiveness.

5. **Theming**:
   - Implemented light and dark themes using Styled Components' ThemeProvider.

### **Directory Structure**
```
frontend/
├── src/
│   ├── components/
│   │   ├── Chatbot.js
│   │   ├── JobCard.js
│   │   └── Navbar.js
│   ├── pages/
│   │   ├── Login.js
│   │   ├── Signup.js
│   │   └── JobListing.js
│   ├── styles/
│   │   ├── globalStyles.js
│   │   └── theme.js
│   ├── App.js
│   ├── index.js
└── package.json
```

---

## **Android Application**

### **Technologies Used**
- **Java**: Primary programming language
- **XML**: For UI design
- **Retrofit**: For REST API integration
- **MVVM Architecture**: Clean code structure

### **Key Features Implemented**
1. **Login and Signup**:
   - Integrated with the backend authentication API.
   - Secure token storage using SharedPreferences.

2. **Job Listings**:
   - Fetch and display job listings dynamically from the backend.
   - Filter and search functionality.

3. **Chatbot Integration**:
   - Chat interface for interacting with the AI chatbot.
   - Smooth and responsive UI.

4. **Empty Views Activity**:
   - Placeholder screens for unimplemented features to maintain user experience.

5. **Responsive Design**:
   - Adaptable layouts for various screen sizes and orientations.

### **Directory Structure**
```
android-app/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/smartjobportal/
│   │   │       ├── activities/
│   │   │       │   ├── LoginActivity.java
│   │   │       │   ├── SignupActivity.java
│   │   │       │   └── JobListActivity.java
│   │   │       ├── adapters/
│   │   │       └── models/
│   │   ├── res/
│   │   │   ├── layout/
│   │   │   ├── values/
│   │   │   └── drawable/
└── build.gradle
```

---

## **Setup Instructions**

### **Backend**
1. Navigate to the `backend/` directory.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the server:
   ```bash
   npm start
   ```
4. Ensure MongoDB is running locally or update the connection string in `config/dbConfig.js`.

### **Frontend**
1. Navigate to the `frontend/` directory.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```

### **Android Application**
1. Open the project in Android Studio.
2. Sync Gradle files.
3. Run the application on an emulator or physical device.

---

## **Future Enhancements**
- Implement real-time notifications for job updates.
- Add user role-based access (Job Seeker and Employer).
- Enhance chatbot capabilities with advanced NLP models.
- Integrate payment gateway for premium features.

---

## **Contributors**
- **Frontend Developer**: [JayakrishnaDara]
- **Backend Developer**: [JayakrisnaDara, ChandraShekar Mekala]
- **Android Developer**: [ChandraShekar Mekala]

---

Feel free to suggest further improvements or enhancements!

