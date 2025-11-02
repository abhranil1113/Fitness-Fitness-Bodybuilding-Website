# Quick Setup Guide

## Step-by-Step Setup

### 1. Open in VS Code
- Open VS Code
- File → Open Folder → Select `fitness_website` folder

### 2. Install Dependencies
Open terminal in VS Code (Ctrl + `) and run:
```bash
npm install
```

### 3. Start Development Server
```bash
npm start
```

### 4. Open in Browser
The app will automatically open at: `http://localhost:3000`

## Project Structure in VS Code

```
fitness_website/
├── 📁 public/
│   ├── index.html          ← Main HTML file
│   └── manifest.json       ← PWA config
│
├── 📁 src/
│   ├── 📁 components/
│   │   ├── Navbar.jsx      ← Navigation bar
│   │   └── Footer.jsx      ← Footer component
│   │
│   ├── 📁 pages/
│   │   ├── Home.jsx        ← Landing page
│   │   ├── UserForm.jsx    ← User input form
│   │   └── WorkoutPlan.jsx ← Workout display
│   │
│   ├── 📁 utils/
│   │   ├── calorieCalculator.js  ← Calories calculation
│   │   └── workoutData.js        ← Exercise database
│   │
│   ├── App.js              ← Main React app
│   └── index.js            ← Entry point
│
├── package.json            ← Dependencies
└── README.md               ← Full documentation
```

## VS Code Recommended Extensions

Install these extensions for better development:

1. **ES7+ React/Redux/React-Native snippets** - Code snippets
2. **Prettier - Code formatter** - Auto-format code
3. **ESLint** - Code linting
4. **Auto Rename Tag** - Auto rename HTML/JSX tags
5. **GitLens** - Git integration

## Running the Project

```bash
# Development mode (with hot reload)
npm start

# Build for production
npm run build

# Run production build locally
npx serve -s build
```

## Troubleshooting

### Port Already in Use
If port 3000 is busy:
- The app will ask to use another port
- Or kill the process using port 3000

### Node Modules Issues
```bash
# Delete node_modules and reinstall
rm -rf node_modules
npm install
```

### Build Errors
Make sure you have Node.js 14+ installed:
```bash
node --version
```

## Next Steps

1. ✅ Install dependencies
2. ✅ Start the server
3. ✅ Fill out the user form
4. ✅ View your personalized workout plan
5. 🎉 Start your fitness journey!

