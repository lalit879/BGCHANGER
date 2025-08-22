# 🎨 React Background Changer

A simple yet elegant web application built with React and Tailwind CSS that allows users to dynamically change the background color of the page with the click of a button. This project serves as a great introduction to handling state in React using the `useState` hook.

![React Background Changer GIF](https://drive.google.com/file/d/1X89jcupjG_JyCOwJrbYoZLAkWO50pcWy/view?usp=drive_link)
*(Feel free to replace this GIF with your own screen recording!)*

---

## ✨ Features

-   **Interactive UI:** A clean and modern interface with a fixed button bar at the bottom.
-   **Multiple Color Options:** A curated palette of 12 distinct colors to choose from.
-   **Instant Feedback:** The background color updates instantly on button click.
-   **Responsive Design:** The layout is fully responsive and works seamlessly on all device sizes, from mobile phones to desktops.
-   **Smooth Transitions:** A subtle `duration-200` transition effect is applied for a smoother color change.

---

## 🛠️ Technologies Used

-   **[React](https://reactjs.org/)**: A JavaScript library for building user interfaces.
-   **[Vite](https://vitejs.dev/)**: A modern frontend build tool that provides a faster and leaner development experience.
-   **[Tailwind CSS](https://tailwindcss.com/)**: A utility-first CSS framework for rapid UI development.

---

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You need to have [Node.js](https://nodejs.org/) and `npm` (or `yarn`) installed on your machine.

### Installation

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/your-username/react-background-changer.git](https://github.com/your-username/react-background-changer.git)
    ```

2.  **Navigate to the project directory:**
    ```sh
    cd react-background-changer
    ```

3.  **Install NPM packages:**
    ```sh
    npm install
    ```

4.  **Run the development server:**
    ```sh
    npm run dev
    ```
    The application will be available at `http://localhost:5173` (or another port if 5173 is busy).

---

## 💡 How It Works

The core logic of the application is straightforward and relies on React's state management.

1.  **State Initialization:** The `App` component uses the `useState` hook to initialize a state variable called `color` with a default value (e.g., "olive").
    ```jsx
    const [color, setColor] = useState("olive");
    ```

2.  **Dynamic Styling:** The background color of the main `div` is dynamically set using an inline style that reads from the `color` state variable.
    ```jsx
    <div style={{ backgroundColor: color }}>
    ```

3.  **State Updates:** Each button in the UI has an `onClick` event handler. When a button is clicked, it calls the `setColor` function to update the `color` state to its respective value.
    ```jsx
    <button onClick={() => setColor("red")}>Red</button>
    ```
    When `setColor` is called, React re-renders the component, and the main `div`'s background is updated to the new color from the state.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
