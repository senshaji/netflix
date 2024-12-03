# Netflix Clone 🎬

A **Netflix** clone application built using **Next.js**, designed to replicate the UI and some core features of Netflix. This project is containerized using Docker and follows best practices with linting and code formatting.

## 📂 Project Structure

```plaintext
📦 netflix
├── 📂 components       # Reusable UI components
├── 📂 config           # Application configuration files
├── 📂 context          # Context API for global state management
├── 📂 hooks            # Custom React hooks
├── 📂 pages            # Next.js pages and API routes
├── 📂 public           # Static files (images, icons, etc.)
├── 📂 styles           # Global and component-specific styles
├── 📂 types            # TypeScript type definitions
├── 📂 utils            # Utility functions
├── .eslintrc           # ESLint configuration
├── .gitignore          # Git ignored files
├── .prettierignore     # Prettier ignored files
├── .prettierrc.js      # Prettier configuration
├── Dockerfile          # Docker configuration file
├── next-env.d.ts       # Next.js environment types
├── next.config.js      # Next.js configuration
├── package.json        # Project dependencies and scripts
├── tsconfig.json       # TypeScript configuration
└── yarn.lock           # Yarn lock file for dependency management
```

## 🚀 Features

- **Next.js** framework for server-side rendering (SSR) and static site generation (SSG).
- **TypeScript** for type-safe code.
- **Context API** for global state management.
- **Custom hooks** to encapsulate reusable logic.
- **Styled Components** or CSS modules for styling.
- **Dockerized** for easy deployment and containerization.

## 🛠️ Technologies Used

- **Next.js** – React framework for building server-rendered applications.
- **TypeScript** – Strongly typed programming language for JavaScript.
- **ESLint & Prettier** – Code linting and formatting tools.
- **Docker** – Containerization platform for consistent development and deployment environments.

## 🐳 Docker Setup

To build and run the project inside a Docker container:

```bash
# Build the Docker image
docker build -t netflix-clone .

# Run the Docker container
docker run -p 3000:3000 netflix-clone
```

## 📦 Installation and Running Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/senshaji/netflix.git
   cd netflix
   ```

2. Install dependencies:

   ```bash
   yarn install
   ```

3. Run the development server:

   ```bash
   yarn dev
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser to see the app.

## ✅ Linting and Formatting

To lint and format the code:

```bash
# Lint the code
yarn lint

# Format the code
yarn format
```
