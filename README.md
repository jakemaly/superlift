# superlift
Workout tracker app - React Native + Firebase

🏋️ Workout Tracker App
A React Native + Firebase app for logging workouts, tracking progress, and analyzing trends.
🚀 Project Goal


MVP (Phase 1):
Log workouts → exercises → sets (weight, reps, time, notes).
View past workout logs.
Keep design simple, clean, functional.


Future (Phase 2+):
Progress graphs.
User accounts with login/authentication.
AI insights (muscle imbalance, periodization, trends).


🛠️ Tech Stack
Frontend: React Native (Expo)
Backend/Database: Firebase Firestore
Optional (later): Firebase Authentication


📂 Project Structure (Planned)
/workout-tracker
  /src
    /components      → Reusable UI parts (buttons, input fields)
    /screens         → App screens (WorkoutLog, History, Settings)
    /services        → Firebase queries & data handling
  /docs
    db-schema.md     → Database design
  App.js


🗄️ Database Schema (Draft)
users (collection)
userId (doc)
workouts (subcollection)
workoutId (doc: { date, title, notes })
exercises (subcollection)
exerciseId (doc: { name, muscleGroup })
sets (subcollection)
setId (doc: { weight, reps, time, notes })


👉 MVP can skip users (just store workouts directly).
⚡ Setup Instructions


1. Clone Repo
git clone https://github.com/YOUR-USERNAME/workout-tracker.git
cd workout-tracker


2. Install Dependencies
npm install


3. Run App
npx expo start
Open in Expo Go app (iOS/Android).


5. Firebase Setup
Create a Firebase project.
Enable Firestore.
(Optional) Enable Authentication.


Copy your config into a .env file:
FIREBASE_API_KEY=xxxx
FIREBASE_AUTH_DOMAIN=xxxx
FIREBASE_PROJECT_ID=xxxx
FIREBASE_STORAGE_BUCKET=xxxx
FIREBASE_MESSAGING_SENDER_ID=xxxx
FIREBASE_APP_ID=xxxx
Import config in your app via firebaseConfig.js.

✅ Weekend Deliverables
 Repo initialized with Expo project.
 Firebase project created.
 db-schema.md documented.
 Both partners can run the app locally.
 Kanban board with Phase 0 tasks.
 
📌 Next Steps (Phase 0 → Phase 1)
Connect Firebase to app.
Create WorkoutLog screen with form.
Create History screen pulling workouts from Firestore.
Push/pull updates via GitHub PRs.
