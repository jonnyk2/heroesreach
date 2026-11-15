# Heroes' Reach website

Static site for Heroes' Reach (heroesreach.com), served by GitHub Pages from `main` / root. No build step.

This repo holds only the public website. The game and its source are in a separate private repo and are never
published here. The files are a copy of the game repo's `website/` folder (minus `gen.mjs`).

Refresh after the game repo's `website/` changes (run from the game repo root):

    D=~/heroesreach-site; find $D -mindepth 1 -maxdepth 1 ! -name .git ! -name CNAME ! -name README.md -exec rm -rf {} + && cp -r website/. $D/ && rm -f $D/gen.mjs

then commit and push here.

Domains: `heroesreach.com` (this site) and `herosreach.com` (forwards to it). Studio: https://chaosvibe.com
