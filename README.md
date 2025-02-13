# 📱 React Native Real Estate App

This is a React Native real estate application built with **Expo**, **React Navigation**, and **React Query**. It allows users to browse a list of homes, view detailed property information, and securely log in to the app.

---

## 🚀 Features
- **Welcome Screen:** A warm welcome with a beautiful background image and a "Get Started" button.  
- **Login Screen:** User authentication with input validation.  
- **Home List:** Displays a list of properties with images, addresses, and descriptions.  
- **Home Detail:** Shows detailed information about a selected property with a stylish UI.  
- **Navigation:** Smooth navigation between screens using React Navigation.  
- **API Integration:** Fetches property data using Axios and React Query.  

---

## 📱Screenshot
<p align="center">
  <img src="https://github.com/Perwez087/RealEstate/blob/4762bfc942d6424265a4eb96b4e6a95b1a1e10ce/screenshot1.jpg" alt="screenshot1" width="300">
  <img src="https://github.com/Perwez087/RealEstate/blob/4762bfc942d6424265a4eb96b4e6a95b1a1e10ce/screenshot2.jpg" alt="screenshot2" width="300">
</p>

<p align="center">
  <img src="https://github.com/Perwez087/RealEstate/blob/4762bfc942d6424265a4eb96b4e6a95b1a1e10ce/screenshot3.jpg" alt="screenshot3" width="300">
  <img src="https://github.com/Perwez087/RealEstate/blob/4762bfc942d6424265a4eb96b4e6a95b1a1e10ce/screenshot4.jpg" alt="screenshot4" width="300">
</p>


---

## 🧭 File Descriptions

### 1. `App.js`
- **Path:** `MyNewProject/App.js`  
- **Purpose:** Main entry point of the application. Configures navigation and React Query client.  
- **Key Features:**  
  - Sets up navigation stack using `createNativeStackNavigator()`.  
  - Initializes **React Query** using `QueryClientProvider`.  
  - Defines routes for `Welcome`, `Login`, `HomeList`, and `HomeDetail` screens.  

---

### 2. `Welcome.jsx`
- **Path:** `MyNewProject/Components/Welcome.jsx`  
- **Purpose:** Displays a warm welcome screen with an attractive background image and a **Get Started** button.  
- **Key Features:**  
  - Uses `ImageBackground` to set a full-screen background.  
  - **Get Started** button navigates to the `Login` screen.  
  - Modern and clean UI design with centered text and button.  
- **Navigation:** Redirects to `Login` screen.

---

### 3. `Login.jsx`
- **Path:** `MyNewProject/Components/Login.jsx`  
- **Purpose:** User authentication screen with email and password validation.  
- **Key Features:**  
  - **Form Validation**: Checks for valid email format and minimum password length.  
  - **Login Button**: Navigates to `HomeList` on successful validation.  
  - **Error Messages**: Displays red error text for invalid inputs.  
- **Navigation:** Redirects to `HomeList` on successful login.  

---

### 4. `HomeList.jsx`
- **Path:** `MyNewProject/Components/HomeList.jsx`  
- **Purpose:** Displays a list of homes fetched from a remote API.  
- **Key Features:**  
  - **API Integration:** Fetches property data using `axios` and `React Query`.  
  - **FlatList Component:** Efficiently renders a list of property cards with images and descriptions.  
  - **Navigation:** Navigates to `HomeDetail` when a property is tapped.  
  - **Loading and Error Handling:** Shows a loading spinner or error message when needed.  
- **Navigation:** Redirects to `HomeDetail` with selected property details.  

---

### 5. `HomeDetail.jsx`
- **Path:** `MyNewProject/Components/HomeDetail.jsx`  
- **Purpose:** Displays detailed information about a selected home.  
- **Key Features:**  
  - **Image and Content Layout:** Image displayed at the top with property details below.  
  - **Back Button:** Navigates back to the `HomeList` screen.  
  - **Unlock Home Button:** A green button for unlocking the home (UI only, no functionality).  
  - **Clean UI Design:** Modern and consistent styling.  
- **Navigation:** Returns to `HomeList` when back button is pressed.  

---

Design and UI
- Consistent Design Language: The app maintains a clean and consistent design throughout all screens.
- Responsive Layouts: Optimized for both iOS and Android devices.
- Modern Components: Uses TouchableOpacity, FlatList, and ImageBackground for modern UI/UX.

## 🧩 Dependencies
Ensure to install the following dependencies:

```bash
npx expo install @react-navigation/native @react-navigation/native-stack
npx expo install @tanstack/react-query axios
npx expo install @expo/vector-icons

🙌 Acknowledgments
React Native for the amazing mobile development framework.
Unsplash for free-to-use images.
MockAPI for providing test data.

✨ Author
Developed with ❤️ by Perwez Alam

