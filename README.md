# Personal Site for GitHub Pages

This folder contains a static personal website starter that deploys to GitHub Pages and supports a custom domain.

## Files

- `index.html`: main page content
- `styles.css`: site styling
- `CNAME`: custom domain for GitHub Pages
- `.github/workflows/deploy.yml`: GitHub Actions deployment workflow

## Replace Before Publishing

1. Update the placeholder text in `index.html`.
2. Replace `example.com` in `CNAME` with your real domain.
3. Replace email, GitHub, and LinkedIn links in `index.html`.
4. Update the page title and meta description.

## Publish on GitHub Pages

1. Create a new GitHub repository, for example `yourusername.github.io` or `personal-site`.
2. Put these files in that repository.
3. Push the `main` branch.
4. In GitHub, open `Settings -> Pages`.
5. Under `Build and deployment`, ensure the source is `GitHub Actions`.
6. Wait for the workflow to finish.

## Connect Your Domain

For an apex domain like `example.com`:

- Create `A` records pointing to GitHub Pages:
  - `185.199.108.153`
  - `185.199.109.153`
  - `185.199.110.153`
  - `185.199.111.153`
- Add a `CNAME` record for `www` pointing to `yourusername.github.io`

For a subdomain like `www.example.com` only:

- Add a `CNAME` record pointing `www` to `yourusername.github.io`

## Final GitHub Settings

1. In the repo `Settings -> Pages`, set the custom domain to your domain if GitHub has not filled it automatically.
2. Enable `Enforce HTTPS` after DNS finishes propagating.

## Local Preview

Open `index.html` in a browser, or from PowerShell run:

```powershell
start .\index.html
```
