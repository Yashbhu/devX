🤖 AI GitHub Explorer & Contributor Assistant (work in progress/pending)

An open-source React Native app that helps developers explore GitHub repos, get AI-generated summaries, step-by-step build instructions, and contribution suggestions.
Users can also post their own projects and chat with contributors to collaborate more easily.

✨ Features

🔑 GitHub OAuth (via Clerk) – log in with your GitHub account.

📂 Browse & Search Repos – starred, trending, or by username.

🏷️ Categorize Projects – AI or GitHub topics (Frontend, Backend, ML, etc.).

📜 AI-Powered Repo Insights

Project summary

Step-by-step “How to build” guide

Suggested contribution tasks (beginner-friendly included)

Maintainer DM/issue templates

👥 Contributor Insights – see top contributors & activity.

💬 Contextual Chat – ask AI questions about a repo.

📌 Save & Track Repos – keep a list of repos you want to contribute to.

🚀 Community Projects – post your own project and invite contributors.

🛠️ Tech Stack

Frontend:

React Native (Expo) + TypeScript

NativeWind (Tailwind for RN)

React Navigation

Backend:

Node.js + Express (API proxy & AI calls)

Clerk (GitHub OAuth)

GitHub REST/GraphQL API

OpenAI/Gemini API (LLM integration)

Storage:

AsyncStorage / SQLite (local)

Supabase/Postgres (optional cloud sync)

📂 Project Structure
src/
  components/       # Reusable UI components
  screens/          # App screens (Login, RepoList, RepoDetail, Chat, Saved)
  services/         # API integrations (github.ts, ai.ts)
  context/          # Auth + Repo context providers
server/
  index.ts          # Express server
  routes/           # API routes (github, ai)
  utils/            # Helpers (auth, prompt builders)

🚀 Getting Started
1️⃣ Clone the repo
git clone https://github.com/your-username/ai-github-explorer.git
cd ai-github-explorer

2️⃣ Install dependencies
# frontend
cd app
npm install
# or yarn install

# backend
cd server
npm install

3️⃣ Setup environment variables

Create .env in server/

GITHUB_CLIENT_ID=your_github_oauth_client_id
GITHUB_CLIENT_SECRET=your_github_oauth_secret
OPENAI_API_KEY=your_openai_key
SESSION_SECRET=supersecret

4️⃣ Run the app
# Start backend
cd server
npm run dev

# Start frontend
cd app
npx expo start

🧠 AI Prompt Examples

Repo Summary → “Summarize the repo in 3 lines, list its stack, and complexity level.”

Build Guide → “Generate step-by-step setup instructions for this repo.”

Contribution Suggestions → “Suggest beginner-friendly tasks based on issues & README.”

DM Template → “Draft a polite message to the maintainer about contributing.”

📌 Roadmap

 GitHub OAuth login

 Fetch & display repos

 Repo detail page (README, issues, contributors)

 AI-generated summaries & build guides

 AI-based contribution task suggestions

 Repo-contextual chat with AI

 Project posting & community discussions

 Push notifications for saved repos

🤝 Contributing

Contributions are welcome!

Fork the repo

Create a feature branch (git checkout -b feature/awesome-feature)

Commit changes (git commit -m "Add awesome feature")

Push branch (git push origin feature/awesome-feature)

Open a Pull Request

📄 License

This project is licensed under the MIT License – feel free to use, modify, and share.
