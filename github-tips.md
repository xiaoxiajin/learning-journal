# Nov 30, 2024

1. Background of React and GitHub Pages Deployment:
   React projects require special deployment steps
   `npm run build` to generate static files for deployment.

   But copy the contents of client/build into the gh-pages branch's specified folder (such as employees-database), to solve structural issues in deployment.

2. Learning to Use the gh-pages Library:
   use the gh-pages library to automatically push the built files to GitHub Pages.
   use the `npm run deploy` command to deploy a React project to the gh-pages branch of GitHub repository.

3. Managing Git Branches and Files:
   Learned about the role of Git branches and how to manage and switch between branches, particularly the difference between main and gh-pages branches.

   check branches using `git branch`, ensuring correctness of files and commits.

# Nov 26, 2024

Pay attention to case sensitivity: File names and extensions must match exactly (e.g., .JPG ≠ .jpg). Otherwise, images that display correctly on the local Windows system may fail to load on GitHub.
