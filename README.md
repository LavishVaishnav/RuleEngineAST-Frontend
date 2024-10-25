# Rule Engine AST - Frontend

Access the site here:- https://ruleengineast-frontend.onrender.com/

Welcome to the **Rule Engine AST** frontend! This project is built using **React** and provides an intuitive interface for creating, combining, and evaluating rules. The frontend communicates with the backend via **axios** to manage rule interactions seamlessly.

## Table of Contents
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Application](#running-the-application)
- [Building the Application](#building-the-application)
- [Deployment](#deployment)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)

## Features

- Create new rules by entering rule strings.
- Combine rules using logical operators (AND/OR).
- Evaluate rules based on user data input.
- Interact with the backend via RESTful APIs.

## Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (version 16 or above)
- **npm** or **yarn** (for managing dependencies)

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/your-username/RuleEngineAST-Frontend.git
   cd RuleEngineAST-Frontend
   ```

2. **Install dependencies**:

   Using npm:
   
   ```bash
   npm install
   ```
   
   Or using yarn:
   
   ```bash
   yarn install
   ```

## Configuration

The frontend communicates with the backend API. To set up the backend URL, create an `.env` file in the root of your project with the following content:

```
REACT_APP_API_BASE_URL=https://ruleengineast-backend.onrender.com
```

Replace `https://ruleengineast-backend.onrender.com` with the appropriate backend URL if needed.

## Running the Application

To start the application in development mode, run:

Using npm:

```bash
npm start
```

Or using yarn:

```bash
yarn start
```

The application will be available at `http://localhost:3000` by default.

## Building the Application

To build the application for production, use the following command:

Using npm:

```bash
npm run build
```

Or using yarn:

```bash
yarn build
```

This will create an optimized production build in the `build/` directory, ready for deployment.

## Deployment

You can deploy the frontend to services like Netlify, Vercel, or Render. For example, if you're using Render:

1. Push your code to GitHub or another Git hosting service.
2. Create a new web service on Render by selecting your repository.
3. Set the build command:
   
   ```bash
   npm install && npm run build
   ```
   
4. Set the publish directory to `build/`.
5. Deploy your app, and your frontend will be live.

## Tech Stack

- **React**: JavaScript library for building user interfaces.
- **Vite**: Fast development build tool.
- **Tailwind CSS**: Utility-first CSS framework.
- **Axios**: HTTP client for API communication.
- **PostCSS**: Tool for transforming CSS with JavaScript plugins.

## Project Structure

```
├── public
│   └── index.html                # Main HTML file
├── src
│   ├── assets                    # Images, icons, and static assets
│   ├── components                # Reusable React components
│   │   ├── CreateRule.jsx        # Component to create a rule
│   │   ├── CombineRules.jsx      # Component to combine rules
│   │   └── EvaluateRule.jsx      # Component to evaluate rules
│   ├── App.jsx                   # Main App component
│   ├── main.jsx                  # Application entry point
│   └── index.css                 # Global styles
├── package.json                  # Project metadata and dependencies
├── postcss.config.js             # PostCSS configuration for Tailwind CSS
├── tailwind.config.js            # Tailwind CSS configuration
├── vite.config.js                # Vite configuration
├── .env                          # Environment variables (API base URL)
├── README.md                     # Project documentation
```

