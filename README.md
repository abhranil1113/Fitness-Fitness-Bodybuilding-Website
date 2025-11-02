# FitBuilder Pro - Fitness & Bodybuilding Website

A comprehensive React-based fitness website that provides personalized workout plans and calorie calculations for both home and gym workouts. The website offers separate programs for men and women with different fitness goals.

## Features

- 🏠 **Home Workouts**: Complete bodyweight exercise programs
- 🏋️ **Gym Workouts**: Equipment-based workout plans with proper form demonstrations
- 👥 **Gender-Specific Programs**: Separate workout plans for men and women
- 📊 **Calorie Calculator**: Personalized daily calorie targets based on goals
- 🎯 **Goal-Based Plans**: 
  - Fat Loss & Muscle Gain
  - Only Fat Loss
  - Only Muscle Gain
  - Gain Weight
  - Lose Weight Only
- 📸 **Exercise Form Images**: Visual demonstrations for proper exercise form
- 📱 **Responsive Design**: Works on desktop, tablet, and mobile devices

## Technology Stack

- **React 18.2.0** - Frontend framework
- **React Router DOM 6.8.1** - Navigation
- **HTML5, CSS3** - Structure and styling
- **JavaScript (ES6+)** - Functionality

## Project Structure

```
fitness_website/
├── public/
│   ├── index.html          # Main HTML file
│   └── manifest.json       # PWA manifest
├── src/
│   ├── components/
│   │   ├── Navbar.jsx      # Navigation component
│   │   ├── Navbar.css
│   │   ├── Footer.jsx      # Footer component
│   │   └── Footer.css
│   ├── pages/
│   │   ├── Home.jsx        # Home page
│   │   ├── Home.css
│   │   ├── UserForm.jsx    # User information form
│   │   ├── UserForm.css
│   │   ├── WorkoutPlan.jsx # Workout plan display
│   │   └── WorkoutPlan.css
│   ├── utils/
│   │   ├── calorieCalculator.js  # Calorie calculation logic
│   │   └── workoutData.js        # Workout plans database
│   ├── App.js              # Main app component
│   ├── App.css             # Global styles
│   ├── index.js            # Entry point
│   └── index.css           # Base styles
├── package.json            # Dependencies and scripts
└── README.md               # This file
```

## Setup Instructions

### Prerequisites

- Node.js (version 14 or higher)
- npm or yarn

### Installation

1. **Navigate to the project directory:**
   ```bash
   cd fitness_website
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm start
   ```

4. **Open your browser:**
   The app will automatically open at `http://localhost:3000`

### Build for Production

```bash
npm run build
```

This creates an optimized production build in the `build` folder.

## Platform Recommendation

**Use VS Code (Visual Studio Code)** for development.

VS Code is recommended because:
- ✅ Better React development experience
- ✅ Integrated terminal
- ✅ Excellent extensions (ES7+ React/Redux/React-Native snippets, Prettier, ESLint)
- ✅ Live preview capabilities
- ✅ Git integration
- ✅ Debugging tools

**Google Colab is NOT suitable** for React/web development as it's designed for Python data science and Jupyter notebooks.

## VS Code Folder Structure

When you open the project in VS Code, you'll see:

```
fitness_website/          # Root folder
├── .gitignore           # Git ignore file (create this)
├── node_modules/        # Dependencies (after npm install)
├── public/              # Static files
│   ├── index.html
│   └── manifest.json
├── src/                 # Source code
│   ├── components/      # Reusable components
│   ├── pages/           # Page components
│   ├── utils/           # Utility functions
│   ├── App.js
│   ├── App.css
│   ├── index.js
│   └── index.css
├── package.json         # Project configuration
└── README.md            # Documentation
```

## How to Use

1. **Start at Home Page**: Users see an overview of the website
2. **Fill User Form**: Enter height, weight, gender, current calories, and fitness goal
3. **Get Plan**: View personalized calorie target and workout plan
4. **Toggle Workout Type**: Switch between Home and Gym workouts
5. **Follow Exercises**: See exercise instructions and form images

## Key Components

### UserForm
- Collects user information (height, weight, gender, calories, goal)
- Validates all inputs
- Calculates calorie needs
- Stores data in localStorage

### WorkoutPlan
- Displays calculated calories
- Shows workout exercises with sets/reps
- Toggles between home and gym workouts
- Displays exercise form images

### Calorie Calculator
- Uses Mifflin-St Jeor equation for BMR calculation
- Adjusts based on activity level
- Modifies target based on user goal

### Workout Data
- Comprehensive exercise database
- Separate plans for men/women
- Home and gym variations
- Includes instructions and equipment needed

## Customization

### Adding Exercises
Edit `src/utils/workoutData.js` to add or modify exercises.

### Modifying Calorie Calculation
Edit `src/utils/calorieCalculator.js` to adjust calculation formulas.

### Styling
Modify CSS files in respective component folders or `App.css` for global styles.

## Future Enhancements

- User accounts and saved plans
- Progress tracking
- Meal planning integration
- Video demonstrations
- Workout schedule calendar
- Social sharing features

## License

This project is open source and available for personal use.

## Support

For questions or issues, please refer to the project documentation or create an issue in the repository.

