# Taco's Sniffari

A relaxed browser game starring Taco, a golden cocker spaniel with a nose for treats and silly treasures.

[Play Taco's Sniffari](https://tacos-sniffari.lauraawp.workers.dev/)

## How to play

- Move around the meadow with the arrow keys.
- Follow the scent clues and walk over treats to eat them.
- Press Space near a bra, shoe, or stick to pick it up. Press Space again to drop it.
- Find all three treats to finish the level and celebrate: "Well done Taco, good boy!"
- Select **Play again** for a fresh level with new treat and object positions.

There is no timer or losing. The game currently uses a keyboard.

## Run locally

Open `index.html` in a browser. No Node.js, installation, build step, or server is required.

## Deployment

Cloudflare Workers Static Assets hosts the game at the link above. `wrangler.jsonc` configures the `tacos-sniffari` deployment, and `.assetsignore` limits uploads to `index.html`.

To update Cloudflare, run `wrangler deploy` from this directory using an authenticated Wrangler CLI. This is a manual deployment; pushing to GitHub alone does not update Cloudflare. The game itself still needs no Node.js or server.

The [GitHub Pages mirror](https://laurawp-wise.github.io/tacos-sniffari/) serves the root of the `main` branch and updates automatically on pushes. The `.nojekyll` file keeps it a plain static site.

All game code and illustrations are contained in `index.html`. The game uses no external assets or services.
