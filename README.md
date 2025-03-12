# Workout Timer App 💪⏱️

Welcome to the Workout Timer App, a simple React-based application designed to help you plan and time your workouts
based on the time of day! 🌞🌙 The app dynamically adjusts workout routines and includes a real-time clock and sound
toggle functionality. 🎶

## Table of Contents 📋

- [Overview 👀](#overview-)
- [Features ✨](#features-)
- [Installation 🛠️](#installation-)
- [Usage 🚀](#usage-)
- [Components 🧩](#components-)
- [Code Structure 📁](#code-structure-)
- [Key Logic 🧠](#key-logic-)
- [Contributing 🤝](#contributing-)
- [License 📜](#license-)

## Overview 👀

The Workout Timer App displays the current time ⏰ and offers a selection of workout routines with varying exercise
counts based on whether it's AM or PM. It includes a sound toggle feature 🎵 and integrates a Calculator component to
assist with workout planning. 🧮

Built with React ⚛️, this app uses hooks like `useState` and `useEffect` to manage state and side effects efficiently.
🚀

## Features ✨

- **Real-Time Clock ⏲️**: Updates every second to display the current time (e.g., "Mar 25, 12:34:56 PM").
- **Dynamic Workouts 🏋️**: Adjusts the number of exercises based on the time of day (AM/PM).
- **Sound Toggle 🔊**: Enable or disable sound effects with the ToggleSounds component.
- **Workout Calculator 📊**: Displays workout details and allows interaction via the Calculator component.
- **Responsive Design 📱**: Simple and clean UI for easy use.

## Installation 🛠️

To run this app locally, follow these steps:

### Prerequisites ✅

- Node.js (v14 or higher) 🖥️
- npm or Yarn 🧶

### Steps 🚶‍♂️

1. Clone the Repository (or use your own project files):
    ```bash
    git clone <repository-url>
    cd workout-timer-app
    ```

2. Install Dependencies 📦:
    ```bash
    npm install
    ```
   Or, if using Yarn:
    ```bash
    yarn install
    ```

3. Run the App 🎉:
    ```bash
    npm start
    ```
   Or with Yarn:
    ```bash
    yarn start
    ```
4. Open your browser 🌐 and navigate to [http://localhost:3000](http://localhost:3000).

## Usage 🚀

- Upon launching, the app displays the current time ⏰ and a list of workout options. 🏃‍♂️
- The number of exercises for "Full-body workout" and "Core only" changes based on whether it's AM 🌅 (morning) or PM 🌃 (
  afternoon/evening).
- Use the **Toggle Sounds** button 🔇 to enable/disable sound effects.
- Interact with the **Calculator component** 🧮 to plan your workout (functionality depends on the Calculator
  implementation).

Example time display:

For your workout on Mar 12, 25 03:45:12 PM ⏳

## Components 🧩

- **App 🌟**: The main component that manages state (`allowSound`, `time`) and renders the UI.
- **ToggleSounds 🔈**: A component to toggle sound on/off (passed `allowSound` and `setAllowSound` props).
- **Calculator ➕**: A component that handles workout calculations (passed `workouts` and `allowSound` props).

## Code Structure 📁

```plaintext
src/
├── App.js              # Main app component 🌟
├── Calculator.js       # Workout calculator component ➕
├── ToggleSounds.js     # Sound toggle component 🔊
└── index.js            # Entry point for React 🚪
```

## Key Logic 🧠

- **formatTime ⏱️**: Formats the current date into a readable string using `Intl.DateTimeFormat`.
- **useEffect ⚡**: Sets up a `setInterval` to update the time every second and cleans up on unmount.
- **workouts 🏋️‍♀️**: An array of workout objects with dynamic `numExercises` based on `partOfDay`.

## Contributing 🤝

Contributions are welcome! 🎉 To contribute:

1. Fork the repository 🍴.
2. Create a new branch (`git checkout -b feature-branch`) 🌿.
3. Make your changes and commit (`git commit -m "Add feature"`) ✍️.
4. Push to your branch (`git push origin feature-branch`) 📤.
5. Open a pull request 🙌.

Please ensure your code follows standard React practices and includes appropriate comments. 📝

## License 📜

This project is licensed under the MIT License. Feel free to use, modify, and distribute it as needed! 🎁


