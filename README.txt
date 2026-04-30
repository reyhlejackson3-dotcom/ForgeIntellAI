# ForgeIntellAI Platform

## Your files
- `index.html` — platform home page
- `admin/index.html` — YOUR dashboard (bookmark this)
- `client/apex-roofing/estimate.html` — Apex Roofing demo (show this to prospects)

## How to go live (Netlify — free, no code needed)

1. Go to netlify.com and create a free account
2. Click "Add new site" → "Deploy manually"
3. Drag this entire `forgeintellai` folder onto the page
4. Netlify gives you a URL like `forgeintellai.netlify.app`
5. Done — your platform is live

## Adding a new client
Come back to the ForgeIntellAI chat and say:
"Add a new client — [Business Name], [industry], they need [system]"
We'll build their room and give you the new files to drag and drop.

## The kill switch
Go to admin/index.html → click "Pause access" on any client.
In the live version, their site goes dark instantly.

## To see the paused screen
Add `?paused=1` to any client URL, e.g.:
`yoursite.netlify.app/client/apex-roofing/estimate.html?paused=1`
