# Netflix Clone 🎬

A **Netflix** clone application built using **Next.js**, designed to replicate the UI. This project is containerized using Docker and follows best practices with linting and code formatting.

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

🐳 For Docker Permissions
If you want to run Docker as a non-root user, then you need to add your user to the docker group.

Create the docker group if it does not exist:

```bash
$ sudo groupadd docker
```
Add your user to the docker group:
```bash
$ sudo usermod -aG docker $USER
```
Create a TMDB Account:
Go to The Movie Database (TMDB) and create an account if you don’t have one.
https://www.themoviedb.org/

Request API Key:

After logging in, go to your Account Settings by clicking on your profile icon.
Select API from the left menu.
Click Create under the API key section.
Fill out the form (application purpose) and submit your request.
Once approved, your API Key will be displayed. Copy it.
Build Docker Image with API Key:
Use the following command to build the Docker image and pass the API key as a build argument:

## 📦 Installation and Running Locally

1. Clone the repository:

```bash
git clone https://github.com/senshaji/netflix.git
cd netflix
```
```bash
# Build the Docker image
docker build --build-arg API_KEY="YOUR_TMDB_API_KEY" -t netflix .

# Run the Docker container
docker run -p 3000:3000 netflix-clone
```
Replace YOUR_TMDB_API_KEY with the actual API key you received from TMDB.
4. Open [http://localhost:3000](http://localhost:3000) in your browser to see the app.

Credits : Ayushi Gupta
