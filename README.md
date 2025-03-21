# Git-Search-Match

# Candidate Search Application

## Overview
The **Candidate Search** application is a front-end project built with TypeScript and React. It integrates with an existing API that retrieves data from the GitHub API to search for potential candidates. The application allows users to browse GitHub users and store potential candidates in local storage.

## Features
- Fetches random GitHub users using the GitHub API
- Allows searching for specific GitHub users by username
- Stores shortlisted candidates in local storage
- Uses Vite for development and bundling
- Deployed to Render

## Technologies Used
- **Front-end**: React, TypeScript, Vite
- **API Integration**: GitHub API
- **State Management**: useState, useEffect
- **Storage**: Local Storage
- **Deployment**: Render

## Installation

1. **Clone the Repository**
   ```sh
   git clone https://github.com/your-username/candidate-search.git
   cd candidate-search
   ```

2. **Install Dependencies**
   ```sh
   npm install
   ```

3. **Set Up Environment Variables**
   - Create a `.env` file in the project root
   - Add your GitHub API token:
     ```sh
     VITE_GITHUB_TOKEN=your_github_personal_access_token
     ```

4. **Run the Application**
   ```sh
   npm run dev
   ```

## API Endpoints
The application interacts with GitHub’s API:
- **Fetch random users:** `https://api.github.com/users?since={start}`
- **Fetch user details:** `https://api.github.com/users/{username}`

Headers include:
```json
{
  "Authorization": "Bearer YOUR_GITHUB_TOKEN"
}

## Issues & Debugging
### **GitHub Token Issues**
- Ensure `.env` file exists
- Restart the Vite dev server after changes:
  ```sh
  npm run dev
  ```
- Check if the token is exposed in `import.meta.env.VITE_GITHUB_TOKEN`

### **Git Issues**
- If branch switch fails:
  ```sh
  git stash
  git checkout main
  git stash pop
  ```



