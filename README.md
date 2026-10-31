# Sachin Tyagi Website

A Next.js website for Sachin Kumar Tyagi with Home, About, Services, Media, and Contact pages.

## Requirements

Install these before starting:

- Node.js 20.9 or newer
- Git
- pnpm 12 or newer

Check your installed versions:

```bash
node --version
git --version
pnpm --version
```

## Download the website from GitHub

1. Open **VS Code**.
2. Open the VS Code terminal:
   - **Terminal → New Terminal**
   - Or use <kbd>Ctrl</kbd> + <kbd>`</kbd> on Windows/Linux, or <kbd>Control</kbd> + <kbd>`</kbd> on macOS.
3. Move to the folder where you want to save the project:

```bash
cd path/to/your/projects
```

4. Clone the repository:

```bash
git clone https://github.com/raadhegovinda/sachin-tyagi.git
```

5. Open the downloaded project in VS Code:

```bash
cd sachin-tyagi
code .
```

If the `code` command is not available, open the folder manually in VS Code using **File → Open Folder** and select `sachin-tyagi`.

## Install dependencies

Run this inside the `sachin-tyagi` project folder:

```bash
pnpm install
```

If pnpm is not installed, install it with Corepack:

```bash
corepack enable
corepack prepare pnpm@12.3.4 --activate
```

Then run the dependency installation again:

```bash
pnpm install
```

## Run the website locally

Start the Next.js development server:

```bash
pnpm dev
```

Open this URL in your browser:

```text
http://localhost:3000
```

The website includes these pages:

- `http://localhost:3000/`
- `http://localhost:3000/about`
- `http://localhost:3000/services`
- `http://localhost:3000/media`
- `http://localhost:3000/contact`

The development server supports hot reload, so changes made in VS Code appear automatically in the browser.

## Create a production build

To check the production version locally:

```bash
pnpm build
pnpm start
```

Then open:

```text
http://localhost:3000
```

Press **Ctrl + C** in the terminal to stop the running server.

## Update the website from GitHub

If you already cloned the project and want the latest changes:

```bash
cd sachin-tyagi
git pull origin main
pnpm install
pnpm dev
```

## Troubleshooting

### Port 3000 is already in use

Start the website on another port:

```bash
pnpm dev -- -p 3001
```

Then open `http://localhost:3001`.

### Dependencies are not working

Delete the installed dependencies and lockfile, then install again:

```bash
rm -rf node_modules
pnpm install
```

On Windows PowerShell, use:

```powershell
Remove-Item -Recurse -Force node_modules
pnpm install
```

### Git asks for authentication

Make sure you are signed in to GitHub and have permission to access the repository. You can also clone using GitHub Desktop and then open the downloaded folder in VS Code.

## Main commands

```bash
pnpm install   # Install dependencies
pnpm dev       # Run the local development server
pnpm build     # Create a production build
pnpm start     # Run the production build locally
```
