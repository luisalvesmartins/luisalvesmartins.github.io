# Using Docsify to build the github pages.

Recipe:

- Create the repository *name*.github.io
- Clone it to your machine
- Install and create docsify:
```
# Install docsify
npm install docsify -g
# Initialize the repo
docsify init ./docs
# Start VS Code to edit your pages
code .
# Start docsify serve to preview your site
docsify serve ./docs
```
- Create a new file inside docs folder called _sidebar.md
- Add "loadSideBar to the index.html:
```
    window.$docsify = {
        ...
       loadSidebar: true,
        ...
```
- Commit and test your site