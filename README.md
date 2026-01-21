<<<<<<< HEAD
# mohalifabricator
Web Content
=======
# Mohali Aluminium Works — Website

This is a simple, static Bootstrap-based website for an aluminium windows & doors firm based in Phase 1, Mohali. It's designed to be beginner-friendly and easy to edit.

What you get:
- `index.html`, `about.html`, `services.html`, `gallery.html`, `contact.html`
- `assets/css/styles.css` — small custom CSS
- `assets/js/main.js` — tiny JS placeholder
- `assets/images/placeholder.svg` — placeholder images

Edit notes:
- Replace placeholder images in `assets/images/` with real photos (keep filenames or update paths in HTML).
- Update phone number and email in all pages.

Adding your own photos
- Place your production photos in `assets/images/`.
- If your camera produced a file name like `9999P8514-8514-190204155508-D5U3.jpg`, you can use it as-is — but for SEO it's better to rename it to a descriptive name, for example `mohali-fabrication-aluminium-door-1.jpg`.
- Make two sizes: a large version (1200–1600px wide) and a thumbnail (≈400px) for faster gallery loading.
- Update `gallery.html` or other pages to point to the exact filename you upload. The scaffold already references `assets/images/9999P8514-8514-190204155508-D5U3.jpg` as a sample.

Adding the photo you mentioned
- You said: `2025-10-27 at 17.23.02_51123c5c` — filenames with spaces and colons can break links on the web, so I sanitized it in the site to `2025-10-27_at_17.23.02_51123c5c.jpg` and added it to `gallery.html` as an example.
- Please place your image file in `assets/images/` with the exact filename `2025-10-27_at_17.23.02_51123c5c.jpg` OR rename it to a descriptive filename (recommended) and update the `src` in `gallery.html` accordingly.
- To rename and optimize the file locally, a good name would be `mohali-fabrication-aluminium-door-2025.jpg` and then create a thumbnail `mohali-fabrication-aluminium-door-2025-thumb.jpg`.

Open Graph & structured data
- After you push the site to GitHub Pages, update the OG image URLs in `index.html` to use your published absolute URL (example: `https://<username>.github.io/<repo>/assets/images/mohali-fabrication-aluminium-door-1.jpg`).
- The `index.html` includes a JSON-LD ImageObject for the main image — update the `contentUrl` to your final published image URL.

Publish on GitHub Pages (manual steps):
1. Create a new GitHub repository (for example `mohali-aluminium`).
2. Initialize git locally if not already:

   git init
   git add .
   git commit -m "Initial website"
3. Add the remote and push (replace `<YOUR-USERNAME>` and `<REPO>`):

   git remote add origin https://github.com/<YOUR-USERNAME>/<REPO>.git
   git branch -M main
   git push -u origin main
4. In your repository settings on GitHub, go to Pages and set the source to the `main` branch and `/ (root)` folder. Save.
5. After a few minutes, your site will be available at `https://<YOUR-USERNAME>.github.io/<REPO>/`.

If you'd like, I can help:
- Customize the copy and images
- Set up a contact form that sends emails
- Walk through creating the GitHub repo and publishing the site

Client-side admin (upload images directly to GitHub)
-------------------------------------------------
This project includes a static `admin.html` which uploads images directly to your GitHub repository using the GitHub Contents API. It does not require any server.

How it works
- Open `admin.html` (after you publish the site to GitHub Pages or open the file in a browser).
- Enter your GitHub owner (username or organization), repository name, branch (usually `main`) and a Personal Access Token (PAT) with `public_repo` scope for public repositories (or `repo` for private repos).
- Select an image and upload. The page will commit the file to `assets/images/` in your repository.

Create a Personal Access Token (PAT)
1. Go to https://github.com/settings/tokens -> Developer settings -> Personal access tokens -> Tokens (classic) -> Generate new token.
2. Give it a short note and select the `public_repo` scope for public repositories (or `repo` if your repo is private).
3. Generate and copy the token. Paste it into the Admin page when prompted. The token is used only in your browser session and is not stored by this site.

Notes and security
- Because uploads are performed using a GitHub token, do not share the token. The token is required only to commit files to your repository.
- After upload, GitHub Pages may take a minute to show the new image.
- If you prefer not to use a PAT, you can always upload images manually to the `assets/images/` folder using the GitHub web UI (drag-and-drop) or git locally.

Making the site available on GitHub Pages
---------------------------------------
Follow the "Publish on GitHub Pages" instructions above. After publishing, your site will be served at `https://<YOUR-USERNAME>.github.io/<REPO>/` and the gallery will load images from `assets/images/` automatically when you provide the repo info in the gallery UI.

>>>>>>> 7020c37 (Test)
