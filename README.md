# Dragon Ball Anime vs. Manga Progression Visualization

This repository hosts the public-facing visualization of the Dragon Ball anime and manga progression pace.

## How to Update This Webpage

This webpage is deployed using GitHub Pages from this `dbviz` repository. The source files for this visualization (including scripts and raw data) are maintained in a separate, private repository.

To update this public webpage after making changes in the private repository:

1.  **Ensure your private repository's `public/` directory is up-to-date** with the latest `index.html` and `dbmain.json` (and any other assets).
2.  **Navigate to your local clone of this `dbviz` repository.**
3.  **Copy the updated files** from your private repository's `public/` directory into the root of this `dbviz` repository.
    ```bash
    # Example (adjust paths as necessary):
    # Assuming 'dragonmap' is your private repo and 'dbviz' is this public repo,
    # and they are sibling directories:
    cp ../dragonmap/public/index.html .
    cp ../dragonmap/public/dbmain.json .
    # Add any other files from public/ if they exist
    ```
4.  **Commit and push the changes** to this `dbviz` repository:
    ```bash
    git add .
    git commit -m "Update visualization files"
    git push origin main # Or 'master'
    ```

GitHub Pages will automatically redeploy the updated content, usually within a few minutes.
