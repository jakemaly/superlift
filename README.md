# Superlift

## MVP Scope
- Add workouts (name, date, notes)
- Add exercises to workouts
- Add sets (reps, weight, RPE)
- View workout history
- View simple analytics (weekly volume chart)

## Tech Stack
- `React Native (Expo)`
- `SQLite` for local data storage
- `Zustand` for state management
- `Victory Native` for charts

## Stretch Goals
- Firebase cloud sync
- Authentication
- ML analytics (Python backend)

## Next Steps
- [ ] Design database schema
- [ ] Create "Log Workout" screen
- [ ] Hook SQLite + Zustand
- [ ] Display past workouts

---

## Superlift Collaboration Workflow

This guide explains how to work on the Superlift project collaboratively without breaking the `main` branch.

### 1. Set Up
- Make sure Git is installed on your machine.
- Clone the repository:
  ```sh
  git clone https://github.com/jakemaly/superlift.git
  cd superlift
  ```
- Add yourself as a collaborator on GitHub (for the repo owner):
  - Go to **Settings → Collaborators & teams → Add people**
  - Invite your partner by GitHub username or email.

### 2. Branching Strategy
- Always create a new branch for your work. **Never work directly on `main`.**
  ```sh
  git checkout -b feature/your-feature-name
  ```
  Example:
  ```sh
  git checkout -b feature/tab-screens
  ```

### 3. Making Changes
- Work on your branch.
- Add and commit your changes regularly:
  ```sh
  git add .
  git commit -m "feat: added new Tab screens"
  ```

### 4. Syncing with Remote
- Push your branch to GitHub:
  ```sh
  git push -u origin feature/your-feature-name
  ```
- Pull the latest changes from `main` regularly to avoid conflicts:
  ```sh
  git checkout main
  git pull origin main
  git checkout feature/your-feature-name
  git merge main
  ```

### 5. Merge Back to Main
- When your feature is ready:
  - Push your branch to GitHub.
  - Open a Pull Request (PR) on GitHub from your branch into `main`.
  - Review changes, resolve any conflicts, and merge the PR.
- After merging, update your local `main`:
  ```sh
  git checkout main
  git pull origin main
  ```

### 6. Tips
- Use descriptive commit messages (e.g., `feat: add login screen` or `fix: button alignment`).
- Communicate before making major changes to avoid conflicts.
- Keep PRs small and focused for easier review.