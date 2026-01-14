Consultation-SaaS-App

Consultation SaaS Application — A modern, full-stack Software-as-a-Service platform that helps users generate business ideas and access expert consultation content with authentication and interactive UI features.

🚀 Overview

The Consultation-SaaS-App is a scalable SaaS application built with a modern stack combining TypeScript, React/Next.js, Python, and other tools. It offers a polished landing page, integrated authentication, and dynamic idea generation features. The app is designed for developers, consultants, and startups who want an opinionated yet extensible foundation for consultation-based SaaS products.

✨ Features

✅ Responsive landing page with gradient design and authentication UI
✅ Multi-provider sign-in support
✅ Idea generation modules with real-time markdown rendering
✅ Configurable backend APIs for business logic
✅ Included Docker configuration for easy deployment
✅ Full support for development and production builds
⚙️ Ready for extension: payments, subscriptions, role-based access, multi-tenant support
📁 Current screens included under /screenshots directory

## ✨ Features Preview

### 1. **Landing Page**
Modern gradient design with authentication options
![Landing Page](./screenshots/Landingpage.png)

### 2. **AWS App-Runner page**
Seamless sign-in with multiple providers
<img src="./screenshots/AWS-Apprunner.png" width="600" alt="Authentication Animation">

### 3. **localrepo-page**
Real-time streaming responses with Markdown rendering
![Idea Generation](./screenshots/Local-Repo.png)



🧠 Tech Stack
Layer	Technology
Frontend	Next.js (React)
Styling	CSS, Tailwind (if configured)
Backend	Node.js / Python
Auth	NextAuth / Third-party Auth Providers
Containerization	Docker
Build Tools	ESLint, PostCSS
Languages	TypeScript, Python, CSS
Package Management	npm / yarn
📦 Getting Started (Local Development)

Follow these steps to run the app locally:

1. Clone the Repository
git clone https://github.com/Patrickmbaza/Consultation-SaaS-App.git
cd Consultation-SaaS-App

2. Install Dependencies
npm install

3. Configure Environment Variables

Create a .env.local file at the root, and set variables such as:

# Copy your values from .env.local
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_...
CLERK_SECRET_KEY=sk_test_...
CLERK_JWKS_URL=https://...
OPENAI_API_KEY=sk-...

# Add AWS configuration (use your chosen region from earlier) - us-east-1 or eu-west-1 etc
DEFAULT_AWS_REGION=
AWS_ACCOUNT_ID=


(Modify according to your authentication and API setup)

4. Run the Development Server
npm run dev


Open http://localhost:8000
 in your browser to preview the app.

🧪 Testing

(Add this section after introducing tests in your repo)

Run the test suite with:

npm test


Configure additional test scripts and coverage reports as needed.

📁 Project Structure
📦Consultation-SaaS-App
 ┣ 📂api/                # Backend endpoints & API logic
 ┣ 📂pages/              # Next.js page routes
 ┣ 📂public/             # Static assets
 ┣ 📂screenshots/        # UI preview images
 ┣ 📂styles/             # Global and component styles
 ┣ 📜Dockerfile          # Docker container definition
 ┣ 📜.gitignore          # Ignored files
 ┣ 📜package.json        # NPM dependencies & scripts
 ┣ 📜next.config.ts      # Next.js configuration
 ┣ 📜tsconfig.json       # TypeScript configuration

🔧 Deployment

Deploy the app using one of the following options:

⚡ Vercel (Recommended)

Connect your GitHub repo to Vercel.

Set environment variables in your Vercel project dashboard.

Deploy with one click — Vercel handles builds and CDN.

🚢 Docker
docker build -t consultation-saas-app .
docker run -d -p 8000:8000 consultation-saas-app

👥 Contributing

Contributions are welcome! To contribute:

Fork the repository.

Create a new branch (git checkout -b feature/your-feature).

Make your changes.

Open a Pull Request describing your changes.

Please ensure your code follows consistent conventions and is well-documented.