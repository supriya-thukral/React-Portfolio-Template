# React-Portfolio-Template

Build a stunning portfolio website with our modern React Portfolio Template. Showcase your skills, projects, and experiences in a clean layout. Fully responsive and customizable to match your style. Start sharing your work with the world today!

## How to Use This Template

This template is designed to help you quickly create your own portfolio website. Follow these steps to get started:

1. **Clone the Repository**: Start by cloning this repository to your local machine. You can do this by clicking the "Code" button on the GitHub page and copying the repository URL. Then, use the `git clone` command in your terminal to create a local copy.

2. **Install Dependencies**: After cloning the repository, navigate to the project's root folder and run `npm install` to install all the necessary dependencies.

3. **Customize Content**: Replace the placeholder content in the existing components with your own information. Update the images, text, and links to reflect your portfolio, experience, and projects.

4. **Add Your Projects**: Create new components or pages for each of your projects and experiences. You can use the existing components as a reference for structuring your content.

5. **Styling and Theming**: Customize the styling and theming of the website to match your personal preferences. You can modify the SCSS files in the `src/styles` folder to change colors, fonts, and overall design.

6. **Configure Navigation**: Update the navigation bar in the `src/Components/TopNav.tsx` file to include links to your different sections or projects.

7. **Test Locally**: Use `npm start` to run the development server locally and see how your changes look in the browser.

8. **Deploy to GitHub Pages**: When you're ready to publish your portfolio, follow the steps to deploy the website to GitHub Pages. You can do this by running the `npm run deploy` command, which will build the project and publish it to the `gh-pages` branch of your repository.

9. **Custom Domain (Optional)**: If you have a custom domain, you can set it up with GitHub Pages to use your own domain for the portfolio.

10. **Share Your Work**: Once your portfolio website is ready, share it with the world! Add the link to your GitHub repository to your resume, LinkedIn profile, or personal website to showcase your projects and experiences.

Remember to keep your repository updated and maintain your portfolio as you complete new projects and gain more experiences.

Happy coding and best of luck with your portfolio! 🚀

## Components

### Page Component

The `Page` component represents a single page in the portfolio website. It is used to display the main content of a page along with an optional image and children. The component is designed to be flexible and customizable to fit various types of content.

**Props:**

- `title`: The title of the page.
- `content`: The main content of the page, typically provided as React nodes.
- `className` (optional): Additional classes for styling the page.
- `image` (optional): An optional image to be displayed on the page.
- `children` (optional): Optional children to be rendered inside the page.
- `href` (optional): An optional href for creating anchor links to the page.

The `Page` component is used in conjunction with the `CardComponent` to create visually appealing pages with consistent styling across the portfolio website.

### PageWithChildren Component

The `PageWithChildren` component represents a page in the portfolio website that contains children elements. It is used to wrap other components and sections within a page, allowing for the creation of complex and structured layouts.

**Props:**

- `children`: The content to be rendered inside the page.
- `className` (optional): Additional classes for styling the page.
- `id`: The unique ID for the page, which can be used for anchor links or other purposes.

The `PageWithChildren` component is a versatile building block that enables the creation of visually appealing and organized pages in the portfolio website.

### TopNav Component

The `TopNav` component renders the top navigation bar on the portfolio website. It displays the logo and navigation links to different sections of the website. The active section is highlighted based on the user's scroll position.

**Props:**

- None

**Usage:**

Simply include the `TopNav` component in your application to display the top navigation bar.

**Example:**

```tsx
import React from "react";
import TopNav from "./TopNav";

const App: React.FC = () => {
  return (
    <div>
      {/* Other components and content */}
      <TopNav />
      {/* Other components and content */}
    </div>
  );
};

export default App;
```

### ProjectCard Component

The `ProjectCard` component is a reusable component that renders a project card with an icon, title, link, description, and an optional badge. It is commonly used to showcase projects on the portfolio website.

**Props:**

- `icon` (IconProp) - The FontAwesome icon to display in the card header.
- `title` (string) - The title of the project.
- `link` (string) - The link to the project.
- `description` (string) - The description of the project.
- `badge` (Optional string) - The badge content to display in the card header.

**Usage:**

To use the `ProjectCard` component, pass the necessary props as shown in the example below:

```tsx
import React from "react";
import ProjectCard from "./ProjectCard";

const App: React.FC = () => {
  return (
    <div>
      {/* Other components and content */}
      <ProjectCard
        icon={/* FontAwesome icon */}
        title="Project Title"
        link="https://example.com/project"
        description="This is the project description. It may contain keywords like React, TypeScript, etc."
        badge="WIP"
      />
      {/* Other components and content */}
    </div>
  );
};

export default App;
```

### BackToTopButton Component

The `BackToTopButton` component is a reusable component that renders a "Back to Top" button that appears when the user scrolls down the page. The button allows users to quickly scroll back to the top of the page when clicked.

**Usage:**

To use the `BackToTopButton` component, simply import it and include it in your JSX where you want the "Back to Top" button to appear:

```tsx
import React from "react";
import BackToTopButton from "./BackToTopButton";

const App: React.FC = () => {
  return (
    <div>
      {/* Other components and content */}
      <BackToTopButton />
    </div>
  );
};

export default App;
```
