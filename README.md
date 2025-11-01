# 🖼️ React Dynamic Image Gallery

A responsive image gallery application built with React. The project's primary goal was to implement client-side pagination from scratch and manage asynchronous data fetching using the `useEffect` hook.

The application fetches a list of images from an API and displays them in a paginated grid, allowing users to navigate through different pages of content.

---

## 📸 App Preview

<img width="1863" height="988" alt="image" src="https://github.com/user-attachments/assets/976eb318-d3c6-49e2-bcfb-dfa44a8e8e43" />

---

## ✨ Core Features

* **Dynamic Data Fetching:** Images are loaded from a remote API when the application starts.
* **Image Grid Layout:** A clean, responsive grid that displays the fetched images.
* **Client-Side Pagination:** A fully functional pagination control to navigate through the image set.
* **Loading State:** A simple indicator is shown while the images are being fetched.

## 🎯 Key Technical Concepts Implemented

This project was a focused exercise in mastering two fundamental React concepts:

### 1. Data Fetching with `useEffect`

The `useEffect` hook was used to handle the asynchronous API call for the image data.
* It triggers the data fetch only once when the component first mounts, thanks to the empty dependency array (`[]`).
* It manages the application's state, including the image array and a `loading` state to improve user experience.

### 2. Custom Pagination Logic

The pagination was built entirely on the client-side to practice state management and data manipulation.
* **State Management:** The `useState` hook tracks the `currentPage`.
* **Data Slicing:** On each page, the correct subset of images is calculated and sliced from the main array to be displayed.
* **Dynamic Controls:** The "Next" and "Previous" buttons are conditionally disabled when the user is on the first or last page, respectively.

## 💻 Technologies Used

* **React:** For building the user interface and managing component state.
* **Vite:** As the front-end build tool and development server.
* **JavaScript (ES6+):** For the application logic.
* **CSS:** For custom styling and the responsive grid layout.
