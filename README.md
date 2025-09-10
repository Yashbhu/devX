🤖 AI GitHub Explorer & Contributor Assistant
An open-source React Native app designed to help developers explore GitHub repositories, get AI-generated summaries, step-by-step build instructions, and actionable contribution suggestions. Users can also feature their own projects and connect with contributors to foster collaboration.

<br/>

📸 Screenshots
(Add your app screenshots or GIFs here to give a visual preview of the project)

Login Screen	Repo List	Repo Detail

Export to Sheets
<br/>

✨ Features
🔑 GitHub OAuth (via Clerk) – Securely log in with your GitHub account.

📂 Browse & Search Repos – Discover starred, trending, or user-specific repositories.

🏷️ Smart Categorization – Projects are automatically categorized using AI or existing GitHub topics (e.g., Frontend, Backend, ML).

📜 AI-Powered Repo Insights:

Concise project summary.

Step-by-step “How to Build” guide for local setup.

Suggested contribution tasks, including beginner-friendly options.

Pre-written templates for direct messaging maintainers or creating issues.

👥 Contributor Insights – View top contributors and their recent activity within a repository.

💬 Contextual Chat – Ask the AI specific questions about a repository's codebase or purpose.

📌 Save & Track Repos – Maintain a personal list of repositories you're interested in contributing to.

🚀 Community Projects – Showcase your own project and invite the community to contribute.

🛠️ Tech Stack
Category	Technology
Frontend	React Native (Expo), TypeScript, NativeWind (Tailwind CSS for RN), React Navigation
Backend	Node.js, Express.js
Services	Clerk (GitHub OAuth), GitHub REST/GraphQL API, OpenAI / Gemini API (LLM Integration)
Storage	AsyncStorage / SQLite (for local device storage), Supabase / PostgreSQL (for optional cloud sync and features)

Export to Sheets
🚀 Getting Started
Follow these instructions to get a local copy up and running for development and testing purposes.

Prerequisites
Node.js (v18 or later)

Yarn or npm

Git

1️⃣ Clone the Repository
Bash

git clone https://github.com/your-username/ai-github-explorer.git
cd ai-github-explorer
2️⃣ Install Dependencies
This project is a monorepo with a separate frontend (app) and backend (server).

Bash

# Install backend dependencies
cd server
npm install

# Install frontend dependencies
cd ../app
npm install
3️⃣ Setup Environment Variables
You'll need to create a .env file in the server/ directory. Copy the example below and replace the placeholder values with your actual API keys and secrets.

server/.env

Code snippet

# GitHub OAuth App Credentials
GITHUB_CLIENT_ID=your_github_oauth_client_id
GITHUB_CLIENT_SECRET=your_github_oauth_client_secret

# AI Service API Key
OPENAI_API_KEY=your_openai_or_gemini_api_key

# Session Secret for Express
SESSION_SECRET=a_long_and_random_secret_string
4️⃣ Run the Application
You need to run the backend and frontend in separate terminal windows.

Bash

# Terminal 1: Start the backend server
cd server
npm run dev
Bash

# Terminal 2: Start the frontend Expo app
cd app
npx expo start
This will open the Expo Developer Tools. You can then run the app on an iOS simulator, Android emulator, or on your physical device using the Expo Go app.

🧠 AI Prompt Examples
This app leverages a Large Language Model (LLM) for its core features. Here are some examples of the prompts used:

Repo Summary → “Summarize this repository in 3 lines. List its primary tech stack and estimate its complexity level for a new contributor (Beginner, Intermediate, Advanced).”

Build Guide → “Based on the README.md and package.json files, generate a concise, step-by-step guide for setting up and running this project locally.”

Contribution Suggestions → “Analyze the open issues with 'help wanted' or 'good first issue' labels. Suggest 3 beginner-friendly contribution tasks. If none exist, suggest tasks based on improving the README or adding documentation.”

DM Template → “Draft a polite and professional message to the repository maintainer expressing interest in contributing to a specific issue. Include a brief introduction.”

📌 Roadmap
[x] GitHub OAuth login flow

[x] Fetch and display user's starred/trending repositories

[x] Implement repo detail page (README, issues, contributors)

[ ] Integrate AI-generated summaries & build guides

[ ] Implement AI-based contribution task suggestions

[ ] Build the repo-contextual AI chat interface

[ ] Develop the feature for users to post their own projects

[ ] Implement community discussion and chat features

[ ] Add push notifications for updates on saved repos

🤝 Contributing
Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request

Please make sure to update tests as appropriate.

📄 License
This project is distributed under the MIT License. See LICENSE.txt for more information. Feel free to use, modify, and share.
