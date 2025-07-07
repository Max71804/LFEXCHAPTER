# LFEXCHAPTER
Lambda Phi Epsilon - UIUC Chapter Website
This repository contains the front-end interface for the Lambda Phi Epsilon (ΛΦΕ) International Fraternity, University of Illinois Urbana-Champaign Chapter. It's a modern, responsive single-page application built with React and styled using Tailwind CSS, designed to showcase the fraternity's values, brotherhood, philanthropy, and events.

Features
Responsive Design: Optimized for various screen sizes (mobile, tablet, desktop).

Smooth Navigation: Fixed header with scroll-to-section functionality.

About Us Section: Information about the fraternity's history and the UIUC chapter's vision.

Interactive Pillars: Clickable sections detailing the core pillars: Scholarship, Service, Leadership, and Brotherhood.

Brotherhood Section: Highlights the strong bonds and shared experiences, including a dynamic Brother Spotlight with clickable profiles and modals.

Meet the E-Board: Introduces the current executive board members.

Philanthropy & Service: Details the chapter's commitment to community service, including support for the Leukemia & Lymphoma Society (LLS).

Upcoming Events: Displays a list of future chapter events.

Recruitment Section: An interest form for prospective members.

Contact Information: Easy access to email and social media links.

Modern UI: Clean, aesthetically pleasing design using Tailwind CSS with a blue and gold color scheme.

Technologies Used
React: A JavaScript library for building user interfaces.

Tailwind CSS: A utility-first CSS framework for rapid UI development.

Lucide React: A collection of beautiful and customizable open-source icons.

Setup and Local Development
To get this project up and running on your local machine, follow these steps:

Clone the repository:

git clone <your-repository-url>
cd <your-project-directory>

Install dependencies:
Make sure you have Node.js and npm (or Yarn) installed.

npm install
# or
yarn install

Start the development server:

npm start
# or
yarn start

This will open the application in your browser, usually at http://localhost:3000.

Customization
Images: Replace placeholder images (https://placehold.co/...) with actual photos of the UIUC chapter. You'll find image src attributes in components like Hero Section, About Section, Brother Spotlight, and Philanthropy Section.

Content: Update the text content in all sections to reflect accurate information, events, and brother bios.

Social Media Links: Modify the href attributes in the Contact Section to point to the official Instagram, Facebook, or other social media pages.

Recruitment Form: The recruitment form is currently a static HTML form. To make it functional, you'll need to implement a backend solution (e.g., a serverless function, Firebase Functions, or a simple email service) to handle form submissions.

Deployment
This React application is a static site and can be easily deployed to various hosting services. Here are a few popular options:

1. Netlify
Netlify offers continuous deployment from Git repositories, a global CDN, and a generous free tier.

Push your code to GitHub/GitLab/Bitbucket.

Sign up for Netlify (https://www.netlify.com/).

From your Netlify dashboard, click "Add new site" -> "Import an existing project."

Connect your Git provider and select your repository.

Netlify will usually auto-detect the build settings (Build command: npm run build, Publish directory: build). Confirm and deploy.

2. Vercel
Vercel is another excellent choice, known for its performance and developer experience, especially with React applications.

Push your code to GitHub/GitLab/Bitbucket.

Sign up for Vercel (https://vercel.com/).

From your Vercel dashboard, click "New Project."

Connect your Git provider and select your repository.

Vercel will also typically auto-detect the build settings (Build command: npm run build, Output directory: build). Confirm and deploy.

3. GitHub Pages
A free option for hosting static sites directly from your GitHub repository.

Install gh-pages:

npm install --save-dev gh-pages
# or
yarn add --dev gh-pages

Add homepage to package.json:

// In your package.json file, at the top level
"homepage": "https://<your-github-username>.github.io/<your-repo-name>",

Add deploy scripts to package.json:

// In the "scripts" section of your package.json
"scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build"
}

Push your code to GitHub.

Deploy:

npm run deploy
# or
yarn deploy

Go to your GitHub repository's Settings -> Pages and ensure the source is set to the gh-pages branch.

4. Firebase Hosting
Ideal if you plan to integrate with other Firebase services in the future.

Create a Firebase Project (https://console.firebase.google.com/).

Install Firebase CLI: npm install -g firebase-tools.

Log in: firebase login.

Initialize Firebase in your project: Navigate to your project root and run firebase init hosting.

Select your Firebase project.

Set build as the public directory.

Configure as a single-page app (Y).

Build your React app: npm run build.

Deploy: firebase deploy --only hosting.
