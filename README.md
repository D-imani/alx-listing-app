# ALX Listing App
## Project Description
The ALX Listing App project aims to scaffold and lay the foundational structure for a modern Airbnb clone. It focuses on setting up a well-organized and scalable codebase using Next.js, TypeScript, TailwindCSS, and ESLint. By establishing a clean folder structure, reusable components, and adhering to best practices, the project ensures a solid starting point for building a dynamic, responsive, and user-friendly property listing page.</br>

**Project Goal**</br>
To create an Airbnb clone listing page.

## Project Structure
The project consists of the following components and directories:
- `components/common/` - Reusable UI components (e.g., Card, Button)
- `interfaces/` - TypeScript interfaces and prop definitions
- `constants/` - Centralized constants (API URLs, text labels)
- `public/assets/` - Static assets (images, SVGs, etc.)



## How to run the project locally.
1. **Creating the Next.js App**
   - Scaffold a new Next.js application named alx-listing-app with the following options:
   - Enable TypeScript to enforce type safety across the project.
   - Enable ESLint for linting and maintaining clean, readable code.
   - Install TailwindCSS for styling and building responsive UIs.
   - Disable the AppRouter (use the Pages Router instead).
   - Do not create a src directory (place files directly under the project root).
   - Do not customize the default import alias</br>
     **Command** : npx create-next-app@latest alx-listing-app --typescript --tailwind --eslint --no-app-router --no-src-dir
  2. **Confirm and Configure Tailwind CSS**
   - Confirm the content of your tailwind.config.js, it should be as below : </br>
     module.exports = {
  content: [
    './pages/**/*.{ts,tsx}',
    './components/**/*.{js,ts,jsx,tsx}',
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
- In styles/globals.css, import Tailwind’s base, components, and utilities only, all other content should be removed and the below is what its contents should be:</br>
     @tailwind base; </br>
     @tailwind components; </br>
     @tailwind utilities; </br>

3. **Create the Required Folder Structure**
     Create the following components and directories inside the root project(alx-listing-app) to establish the project foundation:
- components/common/Card.tsx: This file will define a reusable Card component that will be used across the project to display information about various properties.
- components/common/Button.tsx: This file will define a reusable Button component, which will be used for actions like “Book Now,” “Details,” etc.
- interfaces/index.ts: Define all TypeScript interfaces related to the project. Start by creating placeholder interfaces for CardProps and ButtonProps.
- constants/index.ts: Set up constants to store any reusable data or strings such as API URLs, configuration settings, or UI text

4. **Handle Assets**
     Export all assets (images, SVGs, etc.) into the public/assets folder:
- Create a folder public/assets and place the necessary images and SVG files that will be used across the project (such as placeholder property images).
- Ensure assets are organized for easy access.

5. **Running the Project**
   - To run the project Locally, use the command :
     + npm run dev
   - On the terminal
