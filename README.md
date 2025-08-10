# INFOiYo Hugo Site

This is a Hugo-powered website using the [Fluidity](https://themes.gohugo.io/themes/hugo-theme-fluidity/) theme, which provides a modern, fluid, and responsive design.

![Fluidity Theme Screenshot](https://raw.githubusercontent.com/wayjam/hugo-theme-fluidity/main/images/tn.png)

## Features

- Fluent Design with [Tailwind CSS](https://tailwindcss.com/)
- Built-in Search (Google or PageFind)
- Code Highlighting
- Dark Mode
- Responsive Layout
- Archive Page

## Getting Started

1. **Install Hugo**  
   [Install Hugo](https://gohugo.io/getting-started/installing/) if you haven't already.

2. **Install Dependencies**  
   If using Hugo modules:
   ```bash
   hugo mod npm pack
   npm install
   ```

3. **Run the Site Locally**
   ```bash
   hugo server
   ```

## Configuration

- Site configuration is managed in `hugo.toml` (or `hugo.yaml`).
- For theme-specific options, see the [Fluidity theme documentation](https://github.com/wayjam/hugo-theme-fluidity) and the example config at `themes/hugo-theme-fluidity/exampleSite/hugo.yaml`.

## Creating Pages

- **About Page:**  
  Create `content/about.md`
- **Archives Page:**  
  Create `content/archives/_index.md`
- **Search Page:**  
  Create `content/search/_index.md`

## Deployment: Cloudflare Pages

You can deploy this Hugo site to [Cloudflare Pages](https://pages.cloudflare.com/) for free.

### 1. Push Your Site to a Git Repository

Push your project to GitHub, GitLab, or Bitbucket.

### 2. Create a New Project on Cloudflare Pages

- Go to [Cloudflare Pages](https://pages.cloudflare.com/) and create a new project.
- Connect your repository.

### 3. Set Build Settings

- **Framework preset:** Hugo
- **Build command:** `hugo`
- **Publish directory:** `public`
- **Environment variables:**  
  Add `HUGO_VERSION` and set it to your desired Hugo version (e.g., `0.128.0`).

### 4. (If Using Hugo Modules)

If your project uses Hugo modules, add the following environment variable:
- `HUGO_ENVIRONMENT=production`

And ensure your `go.mod` and `go.sum` files are committed.

### 5. Deploy

Click "Save and Deploy". Cloudflare Pages will build and deploy your site automatically on every push.

---

## License

This project uses the [MIT License](themes/hugo-theme-fluidity/LICENSE) via the Fluidity theme.
