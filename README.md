I am on Node.js
$ node -v
v20.14.0

---

## Deployment: https://madhav-tech-blog.onrender.com/

# MERN Blog App

## Project Setup

### Overview

This project is a full-stack MERN (MongoDB, Express, React, Node.js) application for a blog. It features user authentication, post management, and dynamic routing using React Router. The frontend is built with React, utilizing various libraries for state management, UI components, and routing.

### Technologies Used

- **React**: Frontend JavaScript library for building user interfaces.
- **React Router DOM**: Declarative routing for React applications.
- **PrivateRoute and OnlyAdminPrivateRoute**: Custom components for handling authenticated and admin-only routes.
- **Tailwind CSS**: Utility-first CSS framework used for styling components.
- **ScrollToTop**: Component to scroll to the top of the page on route change.

### Project Structure

The frontend directory (`client`) structure is organized as follows:

- **Pages**: Contains individual pages rendered for different routes:

  - `Home`: Landing page.
  - `About`: About page.
  - `SignIn` and `SignUp`: User authentication pages.
  - `Dashboard`: User dashboard page (protected route).
  - `CreatePost` and `UpdatePost`: Pages for creating and updating blog posts (admin-only routes).
  - `PostPage`: Page displaying a single blog post.
  - `Search`: Page for searching blog content.

- **Components**: Reusable UI components:
  - `Header` and `Footer`: Navigation and footer components displayed across all pages.
  - Various other UI components used for form inputs, buttons, etc.

### Routing

- **BrowserRouter**: Wraps the entire application to enable client-side routing with React Router.
- **Routes**: Defines routes using `<Routes>` and `<Route>` components from React Router DOM.
  - Basic routes for `Home`, `About`, `SignIn`, `SignUp`, `Search`, and `PostPage`.
  - Protected routes (`PrivateRoute`) for `Dashboard` accessible only after authentication.
  - Admin-only routes (`OnlyAdminPrivateRoute`) for `CreatePost` and `UpdatePost`.

### Setup Instructions

1. **Clone Repository**: https://github.com/madhavgupta07/Madhav-tech-blog.git
2. **Install Dependencies**: Navigate to the `client` directory and run `npm install` to install required packages.
3. **Install Dependencies**: Navigate to the `route` directory and run `npm install` to install required packages for BE.
4. **Start Development Server**: Run `npm run dev` to start the Vite development server for frontend development.

5. **Explore Routes**: Access different routes such as `/`, `/about`, `/sign-in`, `/sign-up`, `/search`, `/dashboard`, `/create-post`, `/update-post/:postId`, and `/post/:postSlug` in the browser.

### Additional Notes

- Ensure the backend server (`api/index.js`) is running concurrently for full application functionality.
- Use `npm run build` to build the frontend for production deployment.

---
