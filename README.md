# Tanvi Garg – Portfolio

## Open in VS Code
1. VS Code → File → Open Folder → select this `tanvi-portfolio` folder.
2. Install the **Live Server** extension, then right-click `index.html` → **Open with Live Server**.
   (Or just double-click `index.html` to open it in a browser.)

## Where to edit
- `index.html` – the data block near the top (`<script id="data">`): profile, projects, banners, certificates.
- `css/style.css` – colours, 3D effects, layout.
- `js/app.js` – pages, banners, settings panel, popups.
- `images/` – profile photo, project images, certificate images. Put new images here and add the path (e.g. `images/projects/my-app.jpg`) in the data block.

## Dashboard (local)
Run the site with **Live Server** (http://127.0.0.1:5500). A **Dashboard** link appears in the menu.
- **Save changes** – keeps your edits in this browser only.
- **Save to project folder** – (Chrome or Edge) pick the `tanvi-portfolio` folder once; new images go into `images/` and the data block in `index.html` is updated.
- **Reset local changes** – forgets browser-only edits and reloads the data from `index.html`.
The Dashboard is hidden when the site is opened from a real website address.

## Put it on GitHub and Vercel
1. In VS Code open the Terminal in this folder and run:
   `git init` → `git add .` → `git commit -m "Portfolio"`
2. Create an empty repository on github.com, then run the two commands GitHub shows (`git remote add origin ...` and `git push -u origin main`).
3. On vercel.com choose **Add New → Project**, import the GitHub repository and press **Deploy**. No build settings are needed (it is a plain static site).

## Updating later
Run the site locally with Live Server, use the Dashboard, press **Save to project folder**, then in the terminal:
`git add .` → `git commit -m "Update portfolio"` → `git push`
Vercel redeploys automatically in a minute.

## Dashboard on the live website (only for you)
Visitors never see the Dashboard. It appears only in a browser where you have unlocked it once:
1. On github.com: profile photo → Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token. Repository access: **Only select repositories** → tanvi-portfolio. Permissions → Repository permissions → **Contents: Read and write**. Generate and copy the token (shown only once).
2. Open `https://your-site.vercel.app/#owner`. Enter `your-github-username/tanvi-portfolio`, then paste the token.
3. The page reloads and the Dashboard link appears. Use **Publish to website** to save changes. Vercel updates the site in about a minute.
The token is stored only in that browser. **Log out** in the Dashboard removes it. Never share the token.
