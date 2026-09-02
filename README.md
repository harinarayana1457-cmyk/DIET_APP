<div align="center">

# 🥗 MEALMASTER (DIET APP)
### Minimalist Daily Nutrition, Macro Tracker & Calorie Dashboard

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)](https://697e1aedf75478204956edac--gilded-chaja-11a5c3.netlify.app)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org/)
[![Vite](https://img.shields.io/badge/Vite-5.x-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

<p align="center">
  <b>MealMaster</b> is a lightweight, responsive dietary management web application crafted to streamline personal nutrition tracking. Built with a focused, clutter-free terminal-inspired aesthetic, it allows users to set daily dietary targets, log meals seamlessly, and visualize macronutrient balances without the bloated overhead of commercial fitness trackers.
</p>

[🚀 Live Demo](https://697e1aedf75478204956edac--gilded-chaja-11a5c3.netlify.app) • [✨ Key Features](#-key-features) • [🏛️ Architecture](#-system-architecture) • [🛠️ Tech Stack](#️-tech-stack) • [📦 Quickstart](#-quickstart-guide) • [📁 Structure](#-project-structure)

</div>

---

## 🌟 Key Features

* **🎯 Dynamic Target & Goal Setting**: Configure personalized daily caloric intakes and target split ratios for proteins, carbohydrates, and fats.
* **🍽️ Categorized Meal Logging**: Log foods categorized across Breakfast, Lunch, Dinner, and Snacks with instantaneous nutritional total updates.
* **📊 Macro Balance Visualizer**: Dynamic visual progress meters and charts illustrating macro breakdown and remaining calorie budgets for the day.
* **⚡ Terminal-Brutalist Dark Mode**: High-contrast, sleek dark-themed interface built for reduced eye strain and maximum visual clarity.
* **📱 100% Mobile & Desktop Responsive**: Fluid CSS grid and flexbox layout optimized for fast entry whether on your phone in the kitchen or on your desktop.

---

## 🏛️ System Architecture

```mermaid
flowchart TD
    subgraph UserInputs ["User Interaction & Logging"]
        A[Goal Setting Form] --> D[Target Macronutrient Budget]
        B[Meal Entry Input] --> E[Item Calories, Protein, Carbs, Fats]
        C[Category Selector] --> E
    end

    subgraph StateEngine ["State Manager & Aggregator"]
        D & E --> F[Daily Nutrition Aggregator]
        F --> G[Compute Consumed Totals]
        F --> H[Compute Remaining Caloric & Macro Budget]
        F --> I[Compute % Target Accomplishment]
    end

    subgraph VisualPresentation ["Interactive Presentation Layer"]
        G & H --> J[Progress Bars & Macro Meter Cards]
        I --> K[Daily Calorie Ring / Gauge]
        E --> L[Chronological Meal Timeline List]
    end
```

---

## 🛠️ Tech Stack

| Layer | Technology |
| :--- | :--- |
| **Frontend Framework** | React.js (Single Page Application) |
| **Build Tool** | Vite (Ultra-fast development & production bundling) |
| **Styling** | Tailwind CSS with dark-mode aesthetic |
| **Hosting & CI/CD** | Netlify Continuous Deployment |
| **Code Quality** | ESLint 9 |

---

## 🚀 Quickstart Guide

### Prerequisites
* **Node.js 18.x or higher**
* **npm** or **yarn / pnpm**

### 1. Clone the Repository
```bash
git clone https://github.com/harinarayana1457-cmyk/DIET_APP.git
cd DIET_APP
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Run Development Server
```bash
npm run dev
```
Open `http://localhost:5173` in your browser to view the application.

### 4. Build for Production
```bash
npm run build
```
The compiled, production-ready static assets will be output to the `dist/` directory.

---

## 📁 Project Structure

```text
DIET_APP/
├── index.html                # HTML entrypoint
├── package.json              # Project metadata & dependencies
├── vite.config.js            # Vite configuration
├── eslint.config.js          # ESLint rules configuration
├── .gitignore                # Repository ignore rules
└── README.md                 # Project documentation
```

---

## 🔗 Connect & Links

* **Live Demo**: [MealMaster on Netlify](https://697e1aedf75478204956edac--gilded-chaja-11a5c3.netlify.app)
* **Author**: [Hari Narayana (@harinarayana1457-cmyk)](https://github.com/harinarayana1457-cmyk)
* **LinkedIn**: [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/hari-narayana-035ba1389/)
