# Website editing rules

These rules apply to all work in this repository.

1. Preserve the existing Feather River Grappling branding, layouts, colors, website structure, and original logo and brand asset files.
2. Only modify files necessary for the user's requested changes.
3. Do not redesign unrelated pages or features.
4. Validate HTML, CSS, JavaScript, and local links after website changes. For documentation-only changes, verify the documentation and confirm the diff contains only the requested files.
5. Explain which files were modified and summarize the changes and validation results.
6. Prepare changes in a separate GitHub branch and pull request for the user's review. Obtain the user's explicit approval before merging into `main`; never merge without that approval.
7. Never deploy directly to Cloudways.
8. Preserve the current production `deploy` branch and the existing GitHub-to-Cloudways Git deployment setup. Do not push directly to, reset, delete, or otherwise alter the production branch during development.
9. If something is unclear or could break the live site, ask the user before proceeding.

## Existing deployment workflow

`.github/workflows/deploy.yml` runs on pushes to `main`, including pushes resulting from merged pull requests. It copies the listed website files and assets into a separate Git repository and force-pushes that generated content to the `deploy` branch. Cloudways uses the production branch for Git deployment.

Merging into `main` therefore updates the deployment branch through this workflow. Keep proposed changes on a separate branch and prepare a pull request targeting `main`. Require the user's explicit approval before merging. Preserve the workflow, its file list, the production branch, `.htaccess`, and the existing website structure unless the user specifically requests changes to them; ask first if the change could affect the live site. Do not run the deployment workflow manually or perform a direct Cloudways deployment.
