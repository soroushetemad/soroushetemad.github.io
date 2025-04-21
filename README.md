# Personal Website

This repository contains the source code for a personal website, built with HTML, CSS, and potentially JavaScript.

## Structure

- `index.html`: The main landing page (Homepage).
- `projects.html`: Page dedicated to showcasing projects (e.g., Robotics, Computer Vision, AI).
- `cooking.html`: Page for sharing cooking interests, recipes, etc.
- `photography.html`: Page for displaying a photography gallery.
- `contact.html`: Contact information and a contact form structure.
- `style.css`: Contains all the styling rules for the website.
- `script.js`: Placeholder for JavaScript code to add interactivity.
- `README.md`: This file.

## Content to Add

- **Replace Placeholders:** Go through each `.html` file and replace placeholder text (like "Your Name", "your.email@example.com", project descriptions, photo sources/alt text, etc.) with your actual content.
- **Add Images:** Add your actual photos to the `photography.html` gallery and potentially other pages. You might want to create an `images` folder to keep them organized.
- **Project Details:** Flesh out the `projects.html` page with detailed descriptions, links to repositories (GitHub), and potentially images or videos of your projects.
- **Cooking Content:** Add recipes, photos, or blog-style entries to `cooking.html`.
- **Contact Form Backend:** The contact form in `contact.html` requires a backend service to actually send emails. For GitHub Pages (a static host), popular options include:
    - [Formspree](https://formspree.io/)
    - [Netlify Forms](https://docs.netlify.com/forms/setup/) (if you deploy via Netlify instead of directly on GitHub Pages)
    - Other third-party services.
    You will need to sign up for one of these services and update the `action` attribute in the `<form>` tag in `contact.html` with the endpoint URL they provide.

## Deployment to GitHub Pages

1.  **Create a GitHub Repository:** If you haven't already, create a new public repository on GitHub. A common convention for a user/organization site is `your-github-username.github.io`. For a project site, you can name it anything (e.g., `personal-website`).
2.  **Push Code:** Add these files to your repository and push them to GitHub.
    ```bash
    git init
    git add .
    git commit -m "Initial website structure"
    git branch -M main # Or master, depending on your default
    git remote add origin https://github.com/your-github-username/your-repository-name.git
    git push -u origin main # Or master
    ```
3.  **Enable GitHub Pages:**
    - Go to your repository on GitHub.
    - Click on the "Settings" tab.
    - In the left sidebar, click on "Pages".
    - Under "Build and deployment", select "Deploy from a branch" as the source.
    - Choose the branch you pushed your code to (`main` or `master`).
    - Choose `/ (root)` as the folder.
    - Click "Save".
4.  **Wait:** GitHub Actions will build and deploy your site. It might take a minute or two. Your site will be available at `https://your-github-username.github.io/your-repository-name/` (if it's a project repository) or `https://your-github-username.github.io/` (if you named the repository `your-github-username.github.io`).

## Further Development

- **Enhance UI/UX:** Improve the visual design in `style.css`. Consider using CSS frameworks (like Bootstrap, Tailwind CSS), adding animations, or implementing a more sophisticated design.
- **Add JavaScript:** Implement interactive elements using `script.js`, such as image carousels/lightboxes for the gallery, form validation, or dynamic content loading. 