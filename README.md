# Portfolio

Accessibility and features added

- Skip link to jump to main content for keyboard users (top-left, visible on focus).
- High-contrast toggle (top-right). Click to switch to a high-contrast, color-friendly theme. Preference is saved in localStorage.
- Improved focus styles and :focus-visible for keyboard navigation.
- Reduced-motion respected (system preference) to disable animations.
- Contact form now saves drafts locally and stages submitted messages to localStorage (key: `nd-contact-list`). Submission announces status via an aria-live region.

How to test

1. Open `MyPortfolio.html` in a browser.
2. Press Tab to reveal the "Skip to main content" link and use it.
3. Use the "High contrast" button to toggle themes. Reload the page to confirm preference persists.
4. Fill and submit the contact form; the message will be saved locally. Open DevTools -> Application -> Local Storage to inspect `nd-contact-list`.

If you want additional changes (dark/light theme switch, server-side form handling, or more semantic markup), tell me which to prioritize.

---

Publishing this site

Option A — GitHub Pages (recommended if you have a GitHub account)
- Create a repository on GitHub and push this folder's contents to the repository.
- In the repository settings -> Pages, choose the `main` branch and the root folder (or `/docs` if you prefer). Save. GitHub Pages will publish a URL like `https://<your-username>.github.io/<repo>/` within a few minutes.

Option B — Netlify (quick, free, and supports direct drag & drop)
- Go to https://app.netlify.com/drop and drag the contents of this folder (all files) into the browser window. Netlify will upload and publish the site and give you a public URL instantly. No GitHub account required.

Option C — Vercel or other hosts
- You can also connect this folder to Vercel or other static hosts; they will build and publish similarly.

Notes
- I added `index.html` which redirects to `MyPortfolio.html`, so the site root loads correctly on hosts that expect an index file.
- If you want a custom domain, both GitHub Pages and Netlify support adding one in their settings.

If you want, I can create a clean Git history and push a new GitHub repo for you (I will need your permission to access/push to your GitHub account or you can run the commands I provide). Tell me which option you prefer and I will either:
- provide the exact git commands to push to a new repo you create, or
- walk you through the Netlify drag-and-drop steps and show how to share the public link.