# Jenna Mayfield — GIS Portfolio

A responsive, static GitHub Pages portfolio with a dark technical design. Built with plain HTML, CSS, and JavaScript: no build tools, paid hosting, or dependencies.

## Preview locally

Open `index.html` in your browser, or run `python -m http.server 8000` from this folder and visit http://localhost:8000.

## Customize before publishing

1. **Contact links:** Open `script.js`. Replace the empty values in `const contact={email:'',linkedin:'',github:''}` with your email and full LinkedIn/GitHub profile URLs. Links intentionally do not navigate until configured.
2. **Résumé:** Export your current résumé as a PDF and save it as `assets/resume.pdf`. In `index.html`, find `data-resume` and change it to `data-resume data-ready="true"`. The résumé link is intentionally inactive until you do this.
3. **Projects:** Update the four project descriptions to reflect your exact individual contributions. Replace the abstract CSS art with your own approved project maps or screenshots if desired. Avoid confidential client data.
4. **Skills:** Remove any tool that you don't want to claim. Experience levels vary.
5. **Website metadata:** Edit the title and description in `index.html` if needed.

### Replace a project visual with an actual map

Save an image at `assets/uwharrie-map.jpg`. In `index.html`, inside the appropriate `.project-art` element, insert `<img class="project-image" src="assets/uwharrie-map.jpg" alt="Habitat suitability map of Uwharrie National Forest">` and add to `styles.css`:

```css
.project-image{position:absolute;inset:0;width:100%;height:100%;object-fit:cover}
```

Place the image before the `.art-label` element. If necessary, remove the decorative art elements for that card.

## Publish to GitHub Pages (user or organization site)

1. Create a GitHub account at https://github.com if you don't already have one.
2. Create a **public** repository named **YOUR-USERNAME.github.io**, substituting your exact GitHub username.
3. Upload `index.html`, `styles.css`, `script.js`, the `assets` folder, and optionally `README.md` to the **root** of the repository. Commit the files.
4. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**. Select `main` and `/(root)`, then **Save**.
5. Wait for GitHub Pages to deploy. Open `https://YOUR-USERNAME.github.io/`.
6. If you use a differently named repository, its URL is usually `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`. Relative asset paths in this site support that too.

GitHub Pages documentation: https://docs.github.com/en/pages/quickstart

## Maintenance

To add a new project, duplicate one `<article class="project-card">` in `index.html`, edit its text and category, and add an approved image. Commit changes to `main`; GitHub Pages will redeploy.

## Privacy and attribution

- Don't upload private contact details, confidential client maps, internal SharePoint links, proprietary workflows, or data without permission.
- If using publicly sourced imagery, follow the source's license and provide appropriate credit.
- Current project visuals are original CSS/SVG abstract illustrations, not screenshots of your actual projects.
