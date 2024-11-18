
# Real-Time Chat Application

This project is a real-time chat application built using **React.js** and **Firebase**.
It enables messaging, image sharing, user profile management, and real-time updates.
The application is user-friendly and scalable, offering seamless interaction with a responsive design.

---

## **Features**
### **Real-Time Updates**
- Instant updates for chats and messages using Firebase's `onSnapshot`.

### **Dynamic Chat Management**
- View a list of all active chats.
- Search for users and start new conversations.

### **Media Sharing**
- Upload and share images in chats, stored securely in Firebase Storage.

### **User Profiles**
- View detailed profiles, including avatars, bios, and online status.

### **Responsive Design**
- A clean and intuitive UI for smooth navigation and interactions.

---

## **How the Project Works**
### **1. Firebase Integration**
- **Firestore Database**: Manages user and chat data.
- **Firebase Storage**: Handles image uploads.
- **Firebase Authentication**: Manages user login and logout.

### **2. Global State Management**
- Uses Context API to manage shared states across components:
  - `userData`: Current user details.
  - `chatUser`, `messagesId`: Active chat data.
  - `messages`: Messages in the active chat.

### **3. Component Breakdown**
#### **ChatBox.jsx**
- **Messaging**: Send and receive real-time text and image messages.
- **Rendering**: Displays sent/received messages with timestamps.
- **Image Uploads**: Stores images in Firebase Storage and updates the chat in Firestore.

#### **LeftSidebar.jsx**
- **Chat List**: Displays all active chats for the current user.
- **Search**: Search for users to start new chats.
- **Start New Chat**: Creates new chat documents in Firestore.

#### **RightSidebar.jsx**
- **Profile View**: Displays user details and online status.
- **Media Gallery**: Shows all shared images in a chat.

---

## **Project Workflow**
1. **Login**: Users log in via Firebase Authentication.
2. **Chat Management**:
   - View and manage chats.
   - Start new conversations.
3. **Messaging**:
   - Send text and image messages in real time.
   - Updates are synchronized instantly.
4. **Profile & Media**:
   - View user profiles.
   - Browse media shared in the chat.

---


## **Firebase Configuration**
### **1. Authentication**
- Enable **Email & Password** authentication in Firebase.

### **2. Firestore Database**
- Create a Firestore database in **test mode**.
- Adjust rules to extend expiry dates.

### **3. Storage**
- Set up Firebase Storage in **test mode**.
- Modify rules to extend expiry dates.

---


## **Tech Stack**
- **Frontend**: React.js
- **Backend**: Firebase (Firestore, Storage, Authentication)
- **Styling**: CSS
- **State Management**: Context API

---
