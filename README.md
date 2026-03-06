# AMCC Static Site (Render Ready)

This repository is configured for deployment to Render as a static site.

## Included Deployment Config

- `render.yaml`: Render Blueprint config
- `index.html`: published directly from the repository root

## Deploy on Render (Blueprint)

1. Push this repo to GitHub, GitLab, or Bitbucket.
2. In Render, go to **New** -> **Blueprint**.
3. Select this repository and branch.
4. Keep the default Blueprint path (`render.yaml`) and deploy.

Render will create a static site service named `amcc-site` and publish from `.`.

## Manual Deploy (without Blueprint)

If you prefer creating the service manually:

- Service type: `Static Site`
- Build command: `echo "No build step required"`
- Publish directory: `.`

## Optional Next Steps

- Replace `name: amcc-site` in `render.yaml` with your preferred unique Render service name.
- Add a custom domain from your Render service settings after first deploy.
