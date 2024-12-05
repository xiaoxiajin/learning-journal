# Dec 5, 2024

Learned how to apply a Flask backend to handle API requests, retrieve data, and respond to the frontend.

# Dec 4, 2024

## Learned how to deploy Angular projects to GitHub

### 1. Create a GitHub repository for your project.

### 2. Configure git in your local project

`git remote add origin https://github.com/your-username/your-project-name.git`
`git branch`
`git push origin main`

### 3. Create and check out a git branch named gh-pages.

`git checkout -b gh-pages`

### 4.`ng build --output-path docs --base-href /your_project_name/`

Note: delete any ssr and prerender part in angular.json, otherwise this could go wrong.
e.g.

```
          "builder": "@angular-devkit/build-angular:browser", //  "browser" instead of "application"
          "options": {
            "outputPath": "dist/angular-todo",
            "index": "src/index.html",
            "main": "src/main.ts",//"main" instead of "browser"
```

delete the following:

            "prerender": true,
            "ssr": {
               "entry": "src/server.ts"
            }

### 5. When the build is complete, make a copy of docs/index.html and name it docs/404.html.

Note: check the "base" in the index.html, make sure no local file path is included

### 6. Commit your changes and push.

### 7. On the GitHub project page->Settings->Pages gh-pages/docs->save

### 8. Click on the GitHub Pages link at the top of the GitHub Pages section to see your deployed application. The format of the link is https://<user_name>.github.io/<project_name>/.

ref: https://v11.angular.cn/guide/deployment

# Dec 1, 2024

with sensitive content, add the path to .gitignore in the root directory.

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

   1. Open a terminal in the project folder and `git init`
   2. `git add .`
   3. `git commit -m "Initial commit"`
   4. create repository
   5. `git remote add origin https://github.com/your-username/exchange-rate-tracker.git`
   6. `git push -u origin main`

# Nov 26, 2024

Pay attention to case sensitivity: File names and extensions must match exactly (e.g., .JPG ≠ .jpg). Otherwise, images that display correctly on the local Windows system may fail to load on GitHub.
