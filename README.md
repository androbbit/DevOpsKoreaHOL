# Azure DevOps HOL

This is the source code for Azure DevOps HOL by taking an example of a documentation project.

The documentation can be hosted on any HTML repositories including your GitHub Pages, from the *gh-pages* branch.

This document has been edited as a part of hands-on tutorial.

The second edit has been done to test commit message.

## Running locally

1. Run `dotnet run -p generator/src/generator.csproj -- . "http://localhost:8000/" _site` to build the HTML files.
2. Run `./copy-assets.bash _site` to copy assets into the target directory.
3. Run `python3 -m http.server 8000 --directory _site/` (or whatever your favorite static http server is) to serve the website at port 8000.
4. Open `http://localhost/:8000` in your web browser to view the result.
