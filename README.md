# React Portfolio

A responsive personal portfolio website built with React and Vite to present projects, skills, GitHub activity, and contact information in a clean multi-page experience.

## Internship Project

This repository contains the React portfolio project developed as part of my web development internship/training. The project focuses on applying modern front-end development practices, component-based design, client-side routing, state management, form validation, responsive styling, and API-based data fetching.

## Live Demo

[View the Portfolio](https://chirantan-react-portfolio.netlify.app/)

## Features

- Responsive portfolio interface for desktop and mobile screens
- Home page with hero section, about content, and featured projects
- Dedicated About page with skills and live GitHub activity
- Projects page with category filtering (`All`, `Web`, `Design`)
- Project detail route with dynamic project lookup
- Contact form with controlled inputs, validation, loading state, and success feedback
- Light/dark theme toggle with the selected theme saved in `localStorage`
- GitHub profile statistics fetched from the GitHub API with loading and error handling
- Custom Not Found page for unknown routes
- Reusable React components for navigation, footer, cards, grids, forms, and sections

## Tech Stack

- React 19
- React DOM
- React Router DOM 7
- Vite
- JavaScript (ES6+)
- CSS3
- ESLint
- Git & GitHub

## Project Structure

```text
React-portfolio/
├── public/
├── src/
│   ├── components/
│   │   ├── AboutSection/
│   │   ├── ContactForm/
│   │   ├── Footer/
│   │   ├── GitHubStats/
│   │   ├── Hero/
│   │   ├── Navbar/
│   │   ├── ProjectCard/
│   │   ├── ProjectGrid/
│   │   └── SkillCard/
│   ├── data/
│   │   └── projects.js
│   ├── pages/
│   │   ├── Home.jsx
│   │   ├── About.jsx
│   │   ├── Projects.jsx
│   │   ├── ProjectDetail.jsx
│   │   ├── Contact.jsx
│   │   └── NotFound.jsx
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
└── eslint.config.js
```

## Application Architecture

The application uses React Router for client-side navigation. The main application shell contains the shared Navbar and Footer, while routes render the appropriate page component. Theme state is maintained in `App.jsx` and persisted with `localStorage`.

The project data is kept separately in `src/data/projects.js`, where each project includes a title, description, technology list, category, featured flag, and links. The Projects page filters this data according to the selected category.

## GitHub Integration

The About page includes a GitHub Activity section. The `GitHubStats` component requests the GitHub user profile API and handles loading, error, and successful data states before displaying the profile image, name, public repository count, and follower count.

## Contact Form

The contact form is implemented as a controlled React form. It validates the name, email format, and message length on the client side, then provides sending and success states with user feedback.

## Running Locally

### Prerequisites

- Node.js and npm installed
- Git installed

### Installation

```bash
git clone https://github.com/Chirantan112/React-portfolio.git
cd React-portfolio
npm install
```

### Start Development Server

```bash
npm run dev
```

Vite will start the local development server and display the address in the terminal.

### Production Build

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

### Lint

```bash
npm run lint
```

## Learning Outcomes

Through this project, I practiced:

- Building reusable React components
- Managing component state with React hooks
- Implementing client-side routing with React Router
- Structuring a front-end application by pages, components, and data modules
- Handling API requests with loading and error states
- Creating controlled forms and client-side validation
- Persisting UI preferences with browser storage
- Developing responsive interfaces with CSS
- Using Git and GitHub for source control and project collaboration

## Internship Outcome

The project provided practical experience in taking a portfolio idea from structure and design through component development, routing, state handling, API integration, validation, responsive styling, and deployment. It also helped strengthen my understanding of how a maintainable React application is organized in a real project repository.

## Author

**Chirantan K**  
GitHub: [@Chirantan112](https://github.com/Chirantan112)

## License

This project is intended as a personal internship/training portfolio project.
