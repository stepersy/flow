# 🌸 Flow — Supportive Friend Cycle Tracker

A mobile-friendly web application (designed for iOS & Android browsers) created to help friends — particularly male friends — track and understand the menstrual cycles of their female friends. **Flow** delivers real-time phase insights, personalized recommendations on how to support each friend, and customized lists of their favorite treats and comfort preferences.

---

## 📱 Features

### 1. 🏠 Main Dashboard ("Current Situation")
- **Live Phase Cards**: Instant overview of every friend's cycle phase with clear status banners:
  - *"Alissa is currently in PMS phase"*
  - *"Cecil is on the last day of her period"*
  - *"It's Sophie's ovulation day!"*
- **Expandable Actionable Advice**: Tap any friend's card to reveal:
  - **✅ What to do**: Empathetic, supportive action items tailored to her current phase.
  - **⛔ What NOT to do**: Things to avoid (e.g. demanding strenuous workouts during period, arguing during PMS).
  - **💡 Pro Tip**: Concise guidance on mood and physical energy.
  - **🍽️ Quick Favorites**: Immediate view of her preferred comfort food and drinks.
  - **📅 Quick Period Update**: Update her period start date directly from the dashboard.

### 2. 📅 Interactive Calendar View
- **Color-Coded Visuals**: Highlights every phase of the cycle on a monthly calendar (Period, Follicular, Ovulation, Luteal, PMS).
- **Friend Selector**: Switch between friends easily using top tabs.
- **"Period started this day / today?"**: Recalibrate cycle calculations instantly by clicking any date or tapping the update button.

### 3. ⚙️ Friend Customization & Settings
- **Per-Friend Interests & Preferences**:
  - 🍕 **Comfort Food** (e.g., Cheesecake, Matcha & Sushi, Chocolate)
  - 🍿 **Favorite Snack** (e.g., Dark Chocolate Pretzels, Salted Caramel Ice Cream)
  - 🥤 **Favorite Drink** (e.g., Chai Tea Latte, Iced Matcha)
  - 🤝 **Preferred Support Style** (e.g., quiet company, running errands, low-key plans)
  - ❌ **Dislikes / Triggers** (e.g., sudden plan changes, noisy places)
  - 📝 **Personal Notes & Reminders**
- **Cycle Customization**: Configure default cycle length (e.g. 28 days) and period duration (e.g. 5 days).

### 4. ➕ Multi-Friend Management
- Easily add new friends using the floating pink `+` button in the mobile navigation bar.

---

## 🧬 Cycle Phase Model & Advice Guide

| Phase | Icon | Days (28-day cycle) | What to Do (Supportive Advice) |
|---|---|---|---|
| **Period** | 🩸 | Days 1 – 5 | Bring comfort food, send gentle check-in texts, keep plans low-key & flexible, offer heat pads/treats. |
| **Follicular** | 🌱 | Days 6 – 13 | Energy is rising! Plan active dates, outdoor activities, try new things together. |
| **Ovulation** | ✨ | Day 14 | Peak energy & attraction window. Plan special dinners, dress up, compliment her. |
| **Luteal** | 🌤️ | Days 15 – 25 | Energy winding down. Offer cozy movie nights, board games, and relaxed low-pressure activities. |
| **PMS** | 🌙 | Days 26 – 28 | Cravings & mood swings are real. Surprise her with comfort food, be extra gentle, avoid argument or high stress. |

---

## 🛠️ Tech Stack

- **Framework**: [React 19](https://react.dev/) + [Vite 8](https://vite.dev/)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/) with `@tailwindcss/vite`
- **Icons**: [Lucide React](https://lucide.dev/)
- **Date Calculations**: [date-fns](https://date-fns.org/)
- **Design System**: Mobile-first responsive UI (max-width 480px viewport container, smooth gradient phase styling, iOS/Android safe area support).

---

## 🚀 Getting Started

### Prerequisites
Make sure you have **Node.js** (v18 or higher recommended) and **npm** installed.

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/period-tracker.git
   cd period-tracker
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the local development server**:
   ```bash
   npm run dev
   ```
   Open your browser and navigate to `http://localhost:5173`.

4. **Build for Production**:
   ```bash
   npm run build
   ```
   The compiled output will be generated in the `dist/` directory, ready to deploy to Vercel, Netlify, GitHub Pages, or any static host.

5. **Preview Production Build**:
   ```bash
   npm run preview
   ```

---

## 📁 Project Structure

```text
period-tracker/
├── public/                # Static public assets
├── src/
│   ├── assets/            # Images & icons
│   ├── components/        # React UI components
│   │   ├── BottomNav.js   # Mobile navigation bar & floating add button
│   │   ├── Dashboard.js   # Main overview dashboard
│   │   └── FriendCard.js  # Expandable card with phase advice & advice lists
│   ├── data/
│   │   └── initialData.js # Phase definitions & initial friend data (Alissa, Cecil, Sophie)
│   ├── utils/
│   │   ├── adviceEngine.js    # Per-phase suggestions (Do's, Don'ts, Pro Tips)
│   │   └── phaseCalculator.js # Cycle phase mathematical calculation model
│   ├── App.jsx            # Main app container & view router
│   ├── index.css          # Tailwind CSS directives & mobile container layout
│   └── main.jsx           # React app root entry point
├── package.json           # Dependencies and npm scripts
├── vite.config.js         # Vite & Tailwind CSS configuration
└── README.md              # Project documentation
```

---

## 🔒 Privacy Notice

All data in **Flow** is processed client-side in the browser. No personal information or cycle details are transmitted to external servers.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
