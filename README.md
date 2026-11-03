# M S Jahan Emon — Editorial Portfolio

A free, responsive, customizable personal portfolio for **GitHub Pages**. No build commands, paid hosting, coding environment, or external CMS required.

## Preview locally

Open `index.html` in a browser. For more reliable local preview you may run `python -m http.server 8000` from this folder and browse `http://localhost:8000`.

## Publish FREE with GitHub Pages

1. Create a free GitHub account if you don't already have one.
2. Create a **public** repository called `YOUR-GITHUB-USERNAME.github.io` (replace with your exact GitHub username). On GitHub Free, GitHub Pages for this workflow uses a public repository.
3. In the repository, select **Add file → Upload files**. Upload `index.html`, `style.css`, `app.js`, `data.js`, and the `assets/` folder if you have any images. Keep the files in the repository root.
4. Commit the changes.
5. Go to **Settings → Pages**, set **Build and deployment → Source: Deploy from a branch**, choose **main** and **/(root)**, and save.
6. Visit `https://YOUR-GITHUB-USERNAME.github.io/` once deployment completes. You can watch the deployment in the repository's Actions tab.

If you prefer a differently named repo, your URL will typically be `https://YOUR-GITHUB-USERNAME.github.io/REPO-NAME/` instead. The website is built to work at either URL.

## Edit the entire website later

Select **Edit Studio** at the top of the website. You can:
- Switch between warm light, dark, sand, and mist color themes.
- Switch editorial, gallery grid, and compact index project layouts.
- Change serif, classic, and sans-serif typography.
- Change accent color, name, homepage messaging, biography, and contact details.
- Edit/add/delete/reorder projects and control which projects are featured.
- Edit experience, writing links, and awards.

Choose **Save & preview** to save your changes in **this browser's local storage**. This does not publish changes for other visitors. When you want the changes to appear on the public website:

1. In Edit Studio, select **Export data.js**.
2. On GitHub, open the repository, select **Add file → Upload files**, and upload the exported `data.js`, choosing to replace the existing file (or open `data.js`, press the pencil icon, replace its contents, and commit).
3. Commit the change to `main`. The site then updates after Pages redeploys.

**Important:** The Edit Studio is client-side, and is visible to anyone who visits the portfolio. Visitors' edits affect only their own browsers; they cannot modify your GitHub repository. It is not a secure, authenticated admin console. Don't include secrets or confidential information in `data.js`.

If you edit the website in one browser but want to continue on another, export your `data.js` and import it using Edit Studio's **Import data.js** option.

## Add photos and original campaign material

Create an `assets` directory in the repository, upload your authorized images and use a relative image path such as `assets/nokia-launch.jpg` in the project's **Image** field. Avoid copying images from search without rights/permission. Project photos are intentionally not invented.

## Add videos and documents

The `projects` list inside `data.js` supports `links: [{"label":"Watch campaign film","url":"https://..."}]`. The page will display each available link. To link a CV, upload a PDF to the assets folder and set its path in `site.resume` (for now this is a data field reserved for future use).

## Structure

- `index.html` — website shell, fonts, and scripts
- `style.css` — all responsive layouts and visual styles
- `app.js` — rendering, navigation, and Edit Studio
- `data.js` — all editable public content, configuration, and project records
- `assets/` — user-supplied campaign images and personal photography

## Notes

- Placeholder content is deliberately marked **To be added** rather than falsely attributing outcomes or contributions.
- Personal street address and telephone number from the résumé are intentionally excluded.
- GitHub Pages supports a free SSL-enabled github.io address. A custom domain is optional and typically requires purchasing a domain separately.
- The editor changes most common design settings. For completely new page structures or interactions, `style.css`, `index.html`, and `app.js` are open and editable too.
